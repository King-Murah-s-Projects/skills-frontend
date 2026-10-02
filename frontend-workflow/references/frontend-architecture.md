# Frontend Architecture

## Read the Existing Stack

Before choosing patterns, inspect the app's current stack:

- Framework and version.
- Router and rendering mode.
- Styling system and design tokens.
- UI primitives and icon library.
- Data fetching, cache, form, URL-state, and global-state tools.
- Test runner and browser verification setup.

Do not introduce a new library or state owner when the project already has a good local pattern.

## State Ownership

Name the owner of each state category:

- Remote or API-shaped data belongs in the data-fetching/cache layer.
- Shareable filters, sort, pagination, tabs, and selected records usually belong in the URL.
- Drafts, dialogs, dirty forms, transient selection, and local review state usually belong in component state.
- Global state is for cross-app session, identity, permissions, feature flags, or truly shared client state.
- Browser storage is scaffolding or cache unless the product explicitly treats it as authority.

Avoid storing the same fact in two places. When multiple pages read the same evidence, derive from one canonical boundary.

## Service and Contract Layer

For workflows with rules, create a service or integration layer that enforces them:

- Normalize and validate before writes.
- Enforce permissions, eligibility, allowed transitions, and no-op guards outside the UI.
- Use revision, etag, timestamp, or equivalent conflict checks when users act on opened detail.
- Keep mutations non-optimistic when decisions must be preserved as evidence.
- Keep drafts intact after validation, permission, network, or conflict errors.
- Make errors distinguishable enough for the UI to show the right recovery path.

## Static and Backend Boundaries

Respect the project's delivery model. If the app is static-export or frontend-only, do not add server behavior, route handlers, server actions, middleware, or backend code unless the user explicitly authorizes that scope.

When a future backend is planned, shape demo services like future asynchronous APIs so they can be replaced cleanly.

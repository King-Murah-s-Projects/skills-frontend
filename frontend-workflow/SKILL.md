---
name: frontend-workflow
description: Build, review, or extend frontend applications with a product-aware workflow covering design fit, state ownership, accessible UI, service boundaries, tests, rendered checks, and handoff.
metadata:
  short-description: Frontend workflow
---

# Frontend Workflow

Use this skill for substantive frontend work: building a page, app, dashboard, workflow, design system component, client-side prototype, or product UI. It applies across projects. Let the current codebase, product domain, and user request decide the final implementation details.

## First Pass

Before editing, inspect the project:

- Read local instructions such as `AGENTS.md`, `CLAUDE.md`, `README.md`, design docs, architecture notes, and handoff/progress files when they exist.
- Identify the framework version from package files and local docs. If local instructions warn that a framework version differs from common knowledge, read the relevant installed documentation before editing.
- Inspect the closest completed page, component, or workflow. Prefer the local pattern over a new abstraction.
- Check git status. Preserve unrelated user changes.

## References

Read only the references relevant to the task:

- For product language, domain fit, and UI copy, read [references/product-and-copy.md](references/product-and-copy.md).
- For architecture, state ownership, service boundaries, and data evidence, read [references/frontend-architecture.md](references/frontend-architecture.md).
- For design, layout, accessibility, and interaction patterns, read [references/interface-method.md](references/interface-method.md).
- For tests, rendered verification, design review, and handoff, read [references/verification-and-handoff.md](references/verification-and-handoff.md).

## Operating Principles

- Build the real workflow, not a decorative landing page, unless the user asked for a landing page.
- Match the product type. Operational tools should feel quiet, dense, scannable, and repeatable. Consumer, portfolio, game, and marketing work can be more expressive when the domain calls for it.
- Put permissions, validation, eligibility, and conflict handling in the data/service layer when the workflow has business rules. UI hiding is not enough.
- Keep shareable state in the URL, server-shaped data in the project's data-fetching layer, and temporary drafts in local component state unless the codebase already has a different accepted owner.
- Use existing design tokens, UI primitives, icon libraries, and component conventions before adding new ones.
- Prefer truthful empty, partial, and missing-evidence states over invented data or optimistic claims.

## Implementation Shape

For workflow-style frontend work, aim to complete one coherent slice:

1. Contracts, types, pure rules, and validation.
2. API-shaped service behavior or integration calls.
3. UI with complete states and accessible interactions.
4. Focused tests for risky logic, permissions, edge cases, and evidence.
5. Rendered checks at representative desktop and mobile widths.
6. A concise handoff that states what works, what was verified, and what remains.

Skip or compress steps when the task is small, but do not skip a step that carries real product, accessibility, data, or regression risk.

## Finish Criteria

Do not call the work complete until the user-facing behavior, state ownership, error handling, accessibility basics, responsive layout, tests or rationale for not testing, rendered checks where practical, and affected docs or notes are accounted for.

If a required check cannot run, say so plainly. Do not claim an interaction passed if browser automation could not perform it.

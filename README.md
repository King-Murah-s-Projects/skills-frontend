# skills-frontend

Reusable Codex skill for frontend work.

## Skill

This repository contains:

- `frontend-workflow/` - a Codex skill for building, reviewing, and extending frontend applications with a product-aware workflow.

The skill captures a frontend method for:

- understanding the product and local codebase before editing;
- matching the interface to the domain;
- keeping state ownership clear;
- using existing design tokens, primitives, and patterns;
- enforcing workflow rules in services or contracts, not only the UI;
- building accessible responsive states;
- verifying with tests, rendered checks, design review, and a clear handoff.

## Install Globally

Copy the skill folder into your global Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R frontend-workflow ~/.codex/skills/frontend-workflow
```

Start a new Codex chat or refresh the skill catalog. Then use:

```text
$frontend-workflow
```

or ask naturally for substantive frontend work. The skill allows implicit invocation.

## Install For One Project

Copy the skill folder into a project's local skills directory:

```bash
mkdir -p .agents/skills
cp -R frontend-workflow .agents/skills/frontend-workflow
```

This keeps the skill available to that project without changing the global Codex setup.

## Use

Example prompt:

```text
Use $frontend-workflow to build the new settings page. Follow the existing design system and verify it at desktop and mobile widths.
```

The skill is intentionally framework-neutral. It tells Codex to inspect the current project, follow local conventions, and use the installed framework docs when a version-specific warning exists.

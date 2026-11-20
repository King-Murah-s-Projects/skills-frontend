# skills-frontend

Reusable frontend skills for Codex and Claude Code.

## Skill

This repository contains:

- `frontend-workflow/` - a skill for building, reviewing, and extending frontend applications with a product-aware workflow.

- `dashboard-onboarding/` - a skill for designing and reviewing dashboards, home screens, empty states, and onboarding flows. Based on Mobbin's dashboard study and the "Onboarding That Clicks" talk. Limits of those sources are in `dashboard-onboarding/references/sources.md`.

`frontend-workflow` captures a frontend method for:

- understanding the product and local codebase before editing;
- matching the interface to the domain;
- keeping state ownership clear;
- using existing design tokens, primitives, and patterns;
- enforcing workflow rules in services or contracts, not only the UI;
- building accessible responsive states;
- verifying with tests, rendered checks, design review, and a clear handoff.

## Install Globally

Codex:

```bash
mkdir -p ~/.codex/skills
cp -R frontend-workflow dashboard-onboarding ~/.codex/skills/
```

Claude Code:

```bash
mkdir -p ~/.claude/skills
cp -R frontend-workflow dashboard-onboarding ~/.claude/skills/
```

Both read the same `SKILL.md`. The `agents/openai.yaml` file is only used by Codex and is ignored by Claude Code.

Start a new chat or refresh the skill catalog. In Codex use `$frontend-workflow` or `$dashboard-onboarding`. In Claude Code use `/frontend-workflow` or `/dashboard-onboarding`, or ask naturally.

or ask naturally for substantive frontend work. The skill allows implicit invocation.

## Install For One Project

Copy the skill folder into a project's local skills directory:

```bash
mkdir -p .agents/skills
cp -R frontend-workflow dashboard-onboarding .agents/skills/
```

This keeps the skill available to that project without changing the global Codex setup.

## Use

Example prompts:

```text
Use $dashboard-onboarding to review this home screen and fix the empty first-run state.
```

```text
Use $frontend-workflow to build the new settings page. Follow the existing design system and verify it at desktop and mobile widths.
```

The skill is intentionally framework-neutral. It tells Codex to inspect the current project, follow local conventions, and use the installed framework docs when a version-specific warning exists.

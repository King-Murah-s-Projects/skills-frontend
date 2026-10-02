# Verification and Handoff

## Tests

Scale tests to risk:

- Pure validation, formatting, and state-machine rules should have focused unit tests.
- Service-layer permissions, eligibility, conflicts, idempotency, and persistence should have focused tests.
- Search, filters, sort, pagination, and stable tie-breakers need tests when they drive user workflows.
- Exports need tests for full matching data, not only visible rows, and for spreadsheet safety when relevant.
- UI tests are useful when behavior cannot be trusted through contracts and services alone.

Use the project's existing test runner and naming conventions.

## Rendered Checks

For visible UI changes, run or perform rendered checks when practical:

- Representative desktop width.
- Wide desktop width when the app supports dense layouts.
- Mobile width around 390px.
- Populated, empty, filtered-empty, loading, error, submitting, success, permission-denied, and stale/conflict states that apply to the task.
- Keyboard focus, dialog labels, focus restoration, and critical action activation.
- Horizontal overflow, clipped text, overlap, and console errors.

Do not claim a rendered interaction passed unless it was actually performed.

## Design Review

When a Better Design, visual, accessibility, or spacing review is available and relevant:

- Run it against rendered states.
- Fix critical, serious, and real moderate issues.
- Record false positives when they are caused by a deliberate local pattern.
- State unavailable tools or incomplete measured checks honestly.

## Handoff

Finish with a concise report:

- What changed.
- The workflow behavior.
- Role or permission rules.
- Evidence, audit, or persistence model.
- Files changed.
- Tests, lint, typecheck, build, and browser results.
- Design review findings and fixes.
- Known limitations and exactly what remains.

Update project documentation only when the change affects it. Do not churn unrelated docs.

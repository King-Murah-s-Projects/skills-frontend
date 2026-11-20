---
name: dashboard-onboarding
description: Design or review dashboards, home screens, and onboarding flows. Use when building or critiquing a dashboard, an analytics or admin home screen, an empty state, a first-run or signup flow, a tour, or release-notes UX.
metadata:
  short-description: Dashboard and onboarding design
---

# Dashboard and Onboarding

Use this for screens a person sees first and often: dashboards, home screens, empty states, signup and first-run flows, tours, and "what's new" surfaces. It pairs with `frontend-workflow`. That skill covers how to build. This one covers what the screen should say and when to teach.

## The two ideas

1. A dashboard is a clean surface between the user and the mess. It interprets data, picks what comes first, and leaves things out. Showing everything is the failure mode.
2. Onboarding is not the first five minutes. It runs for the life of the product. The best onboarding is a good first screen and a quick win, not a tour.

They agree on one thing: the first screen should teach. They pull in opposite directions on one thing: dashboards leave things out, onboarding fills empty states. Resolve it like this: show less, but never show nothing.

## Pick the reference

- Building or reviewing a dashboard or home screen: read [references/dashboard-design.md](references/dashboard-design.md).
- Building or reviewing signup, first-run, empty states, tours, nudges, or release notes: read [references/onboarding.md](references/onboarding.md).
- Both apply on most first-login screens. Read both.
- To review an existing screen, run the checklist in [references/review-checklist.md](references/review-checklist.md).

## Before designing

- Name the one thing the user must know within three seconds of landing. If you can't, the screen isn't ready.
- Name the user's likely emotional state on arrival (anxious after a drop, proud after a win, lost on day one).
- Check the project for an existing dashboard or onboarding pattern. Match it before inventing one.

## Rules of thumb

- Put the verdict before the chart. Put the "why" next to the number.
- Name important metrics. "Streak" and "Readiness Score" beat "Consecutive days active."
- Detail lives one click away, not on the first screen.
- Never ship an empty first screen. Use sample data, a template, or a pre-filled first step.
- Teach in context at the moment of need. Avoid next-next-next tours.
- Ask for the minimum up front. Split long asks and defer the rest.
- Notify only when it matters to the user, never on a schedule.

## Evidence and honesty

The source material is a design study and a conference talk, not controlled experiments. Treat the guidance as strong defaults, not laws. Do not quote the numbers in `references/sources.md` as proof of what works. Mobbin's data measures what designers save, not what end users do. If a recommendation matters, test it with the project's own users or analytics.

## Finish

State which screens you changed or reviewed, which rules drove each decision, and what you could not verify. If you could not render the screen, say so.

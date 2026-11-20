# Onboarding

Source: Martin Dabrowski, "Onboarding That Clicks", HelloStavanger 2025. See `sources.md`.

## Definition

The design path that turns first-time participants into successful repeat users across the product's lifetime. It is a continuous conversation, not a one-time event.

## First win

- Get the user a real result in under five minutes, in about three to five steps.
- Do not show an empty dashboard. Use sample data, a template, or pre-filled fields so the surface is populated on arrival.
- Make it safe. Give a sandbox with no big consequences and room to fail and retry.
- Show clear success, then offer the next action as an option, not a requirement ("Report created. Invite a teammate.").
- Contrast: heavy signup, then an empty screen, then heavy setup leads to low confidence and a weak day-two return.

## Do you need onboarding at all?

Decide in this order:
1. Is it forced by compliance or critical info (KYC in fintech)? Then make it purposeful and short.
2. Is the interaction novel or complex? Then use contextual onboarding.
3. Otherwise, improve the base UI. A good first screen teaches most of what a tour would.

Avoid generic walkthroughs. Use onboarding only where it unlocks value.

## Lessons from games

- Teach by playing, in a safe space where failure is cheap (the first Super Mario screen introduces hero, foe, reward, and power-up).
- Make progress tangible with a visible path and an early reward. Treat roles (admin, support) as guided paths.
- Rich tooltips: color and icons for key info, requirements and progress shown, relevant actions embedded (Diablo).
- Teach in context at the moment of need (a locked gate tells you to find a blue key).
- Let the user create identity early, with a live preview. Invested users come back.
- Games have clear win states, safe failure, and telemetry-driven tuning. Copy the telemetry habit: find where users drop, then fix that step.

## Diagnose with models, as guides

- Fogg (B = MAP): behavior needs motivation, ability, and a prompt. If motivation is high and users still fail, cut the ask. Example: split a 10-question form into 5 now and 5 later. Use for one specific action.
- COM-B: check capability (do they know how), opportunity (can they do it, for example upload the CSV), then motivation. Use for a multi-step flow that fails somewhere.
- Adoption curve: innovators tolerate rough edges, early adopters want to be early, the early majority wants proof, the late majority wants strong onboarding and support, laggards move only when forced. Onboarding needs change along this curve.

## Tactics

- Personalize lightly: one or two signup questions to route the path.
- Let people try before they sign up.
- Micro-roles and quick do-it-yourself steps. Remember progress.
- Start progress bars at 20 to 25% by pre-filling from SSO (name, email). It nudges completion. This is a known effect, but the talk cites no study. Use it honestly: only count real, completed fields.
- Keep help one click away with sample data to practice on, so the user never has to leave and search.
- Earn badges. Do not spam them.
- Force tours and pop-ups only when needed for the task at hand.
- Notifications and nudges only when useful to the user, not on a schedule.

## Long-term

Onboarding continues after day one: role-based learning, "users like you did X next" suggestions, seasonal challenges for mature products, personalized changelogs mapped to role and workflow.

For release notes, do not publish a static list. Adobe's "Try it now" opens a working file with steps that reproduce the preview, which taught the new features better than patch notes.

## Examples

Good: Adobe's try-it patch notes, Miro's templates (OKR template with video and contents), Squarespace's short visual signup that ends in a first site.
Weak: Azure (too many steps for a simple task), Google AI Studio (labels like "structured outputs" do not explain themselves, and richer tooltips would teach), click-next guided tours (few finish them; users need to try things first).

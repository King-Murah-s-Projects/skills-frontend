# Dashboard design

Source: Mobbin, "What good dashboard design looks like" (Rebekah Bek). See `sources.md`.

## Job of a dashboard

The word comes from the board on a carriage that blocked mud. The job is the same: put a clean surface between the user and the mess. "Most dashboards show you the data. The best ones almost protect you from it."

## Principles

### 1. The first screen says what the product is
About 1 in 5 apps use the dashboard as the home screen. If the first screen could belong to any product, it is wasting its one chance.
- Shopify Live View: a globe of live visitors. It encodes a feeling, not only a metric.
- Front: a weekly heatmap of support volume. Darker means busier. Readable in three seconds.
- Navattic: named companies with visit counts. The dashboard is the proof of purchase.

### 2. Read the data for the user
Put the interpretation beside or above the number.
- Fey annotates a chart drop with the event behind it (earnings, news) so the "why" shows before the user asks.
- Origin puts a daily market brief next to the portfolio chart.
- Runna decides the order a post-run user sees data in: summary, effort rating, milestone, then laps.
Design for the emotional state: reassurance after a loss, celebration after a win.

### 3. Give metrics a vocabulary
A named metric is easier to remember, share, and care about.
- Duolingo "streak" implies momentum and risk.
- Oura "Readiness Score" folds several signals into one verdict.
- Apple's three rings became everyday speech.
Prefer one named score with drill-down over a wall of raw figures.

### 4. Conclusion before chart
Lead with a plain sentence. Linktree says "your clicks jumped to 27 from zero" above the chart. Binance puts an AI-written verdict over its Fear and Greed chart. Amplitude flags anomalies so the user reviews findings instead of scanning. Label generated text as generated.

### 5. Leave things out
Blank space is part of the design.
- Plausible: five stats, one chart, two columns, every panel links deeper.
- Revolut: a balance, three buttons, and a plain "Transactions will appear here" state.
- Anti-pattern: more charts, more metrics, more tabs, and a deep menu before the user finds last week's traffic.
AI can generate a dense dashboard in seconds. The hard part is deciding what to cut.

### 6. Find the one number that keeps the user
Ask what single figure makes someone return (lifetime earnings in a cashback app, streak in a language app). Make it prominent and keep clutter away from it.

## Do
- State the first-glance message before choosing components.
- Encode feeling where it fits the domain.
- Pair every key number with a reason, trend, or verdict.
- Name the top metrics.
- Keep depth one click away.

## Don't
- Fill all available space.
- Add panels because the data exists.
- Make the user hunt through navigation for a basic question.
- Ship a first screen that is empty. See `onboarding.md`.

## Fit to the product
For operational tools, quiet and dense can be right, but the first-glance message and the verdict still apply. For consumer products, lean on named metrics and emotion.

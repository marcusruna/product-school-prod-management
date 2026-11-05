# GTM Launch Plan, StreamLine (B2C)

| Field | Value |
|---|---|
| Feature | A1, Spotlight Curated Rail: Hand-picked homepage rail that bypasses the algorithm |
| Goal | Engagement |
| Launch tier | M, Targeted |

## Goal & Audience
- **Goal:** Engagement, The reason for my choice is because our target audience has been struggling to stay engaged to the platform due to the overwhelming amount of choices offered and decisions they need to make to pick and watch one movie. The new spotlight feature is aimed to resolve that issue to highlight curated picks of movies for the view in order to keep them engaged longer.
- **Target audience:** Wanderers: 41% of StreamLine’s subscriber base, averaging 1.1 sessions/week and $8.40 monthly LTV, with 61% of viewing from Trending and only 18% from curated content. Within them, the priority is long-tenured subscribers (the Overwhelmed Veteran) who reach the homepage, scroll for up to twenty minutes without finding anything, and leave the app. Spotlight-exposed Wanderers show 22 points less churn, the largest improvement of any segment.

## Launch Tier
- **M, Targeted**, Reach: Wanderer-pattern accounts only. Power Users see the rail lower on the page, and a holdout group gets nothing. Revenue: Indirect but high-value, because it targets long-tenured subscribers drifting toward churn. It isn’t proven until the 30+ minute session share moves. Risk of silence: High for this segment. She has mostly stopped opening the app, so a silent ship leaves the rail invisible to the people it was built for. Anything bigger than M would contaminate the holdout, draw Power Users’ attention to a change designed to be low-key for them, and overpromise an MVP.

## Channels
1. **Owned: Long-tenured subscribers still have a verified email address on file, and email reaches her in the evening without her opening the app. Send one message to lapsed Wanderers in the treatment group only, timed around 6 pm: “Our editors picked 10 titles for tonight.” Each title deep-links straight to its title page, so she reaches Play in two taps. The holdout group is suppressed so the metric stays clean.**
2. **Owned: A lapsed user often still has the app installed even if she never opens it, and a push lands on her lock screen without her having to come to the app. Send one push per week, on the day the rail refreshes, to the treatment group only, deep-linking into the Spotlight rail. It’s capped at once a week, because a lapsed user who’s spammed turns notifications off for good.**
3. **Paid: Upload a hashed list of treatment-group emails to social and video platforms so that only those subscribers see the ad. That reaches her where she still spends evenings, with no spillover to Power Users or the holdout. Keep the budget small and capped, to match an M launch. Earned media is held back on purpose: press coverage would contaminate the holdout and draw Power Users’ attention to the change. It’s the first thing to add if the metric moves and we scale up to L.**

## Enablement & Assets
Support/CS need an FAQ and reply macros for three questions: “Why do I (or don’t I) see Spotlight?” (the answer covers segments and the holdout without calling it an experiment), “How are the picks chosen?” (“by our editors, not an algorithm”), and “Can I change it?” (not in V1). Editorial needs a weekly refresh runbook and a style guide for one-liners: write about the title, never “because you like [genre].” Sales gets a short note explaining why Watch Party and Offline aren’t in this release.

## Ownership, Budget & Timeline
- **Ownership & budget:** PRD, experiment design & ship/iterate/kill decision: [Your name], PM
Rail build (FR1–FR7) within the 3-week sprint: [Name], Lead Engineer, with one supporting engineer
Weekly Spotlight list (8–10 titles + one-liners) and data-file updates: [Name], Editorial Lead
Instrumentation, Wanderer baseline pull, A/B assignment & Day 14 / Day 30 reads: [Name], Data Analyst
Power User guardrail monitoring & rollback call: [Your name], PM, alerted by the analyst
In-app launch messaging (rail header, any home-screen intro): [Name], Product Marketing
- **Timeline:** Phase 1: Beta (weeks 1–5). Weeks 1–3: build the rail, instrument tracking, pull the Wanderer baseline, run moderated prototype sessions (target: 80% press Play within 60 seconds). Weeks 4–5: run the 14-day A/B test, 50/50 within Wanderers and Power Users, with no peeking before Day 14.

## Success Metrics
- **Metrics:** Lagging confirmation: Wanderer Month 1 retention vs. holdout. Retention isn’t the goal; it’s how we confirm the engagement lasts.
- **Bad signal to watch for:** High rail views, low plays. Wanderers see the rail but don’t pick from it. That’s a curation–audience mismatch: the editors’ picks don’t appeal to people who watch 61% Trending. Fix the selection, not the placement.
- **Likely post-launch decision:** Iterate. Wanderers currently watch only 18% curated content and 61% Trending, so an editor-picked rail starts against their habits. The most likely result is a positive lift in 30+ min sessions that falls short of the +8 pt goal.

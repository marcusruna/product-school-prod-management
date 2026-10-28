# Roadmap, PRD & Prototype (Module 4)

## Your strategic anchors
- **Persona (M2), who are you solving for?:** The Overwhelmed Veteran: a long-tenured subscriber who once used StreamLine as her default evening entertainment but now behaves like a Wanderer. Her goal is to open the app and confidently find something worth her evening. Confirmed friction: she browses without starting anything, and when she does start something, she doesn’t trust it enough to stay.
- **Primary success metric (M3), your leading indicator:** Share of Wanderer sessions reaching 30+ minutes after engaging with Spotlight. It’s a leading indicator that moves before churn does. Month 1 retention is the lagging confirmation.
- **Moment of misery (M2), the specific friction blocking the goal:** She opens the app, scrolls for about twenty minutes, and closes it without watching anything. She ends up putting on a DVD instead. The catalog’s size, which should be a reason to stay, has become a reason to give up. Marcus adds the trust dimension: the recommendations treat him as a genre (“I’m not a genre, I’m a person”), so he has stopped believing the app can surface anything good.
- **Guardrail metric (M3), what must not drop or break:** Power User sessions/week (currently 4.8×) and churn. Power Users already watch 58% curated content, and Spotlight must not cannibalize or disrupt the segment that already works.

## Scan the backlog & set a human baseline
- **My instinctive “quick wins” before touching the AI (2 to 3 feature IDs + why):** A1 – Spotlight Curated Rail. This is the simplest version of the whole Spotlight idea. A homepage rail is a UI pattern StreamLine almost certainly already has, and hand-picking titles means no new algorithm or model to build, only an editorial process. It comes straight from M2 UXR, so there’s a user need behind it. It’s arguably the MVP everything else builds on.

A3 – Hidden Gem Badge. This is cheap to build: a rule like “rating above X, view count below Y” applied to metadata you already have, then shown as a visual badge. It’s backed by M3 data, and it directly serves what Spotlight is for, which is surfacing good content people are missing.

A6 – Spotlight Digest Email. This uses existing email infrastructure and comes from M3 retention findings, so it targets a metric leadership cares about. One caveat: “personalised” adds effort. A v1 could send the same three editorial picks to everyone, which keeps it a quick win.

## Audit, override & decide
- **Where did you override the AI? (feature + old vs. new score + why):** A2 “Why You’ll Love This”: Effort 3 → 2, Major Project → Quick Win. I descoped it from AI-generated reasons to curator-written one-liners on Spotlight Rail titles. M2 interviews showed the trust problem is about being treated as a genre (Marcus: “I’m not a genre, I’m a person”), so a human-written reason fits that problem better than an AI one. Most evening viewing happens on TV, where there is no hover.
- **Did the AI over-value a Sales/Eng request your M2 interviews don’t support?:** No. It scored all three at Value 1 (A8 Watch Party, A10 Offline, both from Sales; A9 Filters, from Engineering). That matches M2: none of the interviewees described a group-viewing or connectivity problem. If anything, A9 is a negative for this persona, since adding more filters adds to the choice overload that caused the Moment of Misery. I’m keeping all three in Cut.
- **Did it underweight something your M3 cohort/funnel data strongly supports?:** A5 Personalized Spotlight Queue (M3 Cohort): Value 2. The AI dismissed it as “the algorithm again,” but my cohort data shows otherwise. I’m raising Value to [3] and placing it in Later, because Effort 4 still doesn’t fit this sprint. I’d revisit it once A1 shows whether curation rebuilds trust.

## Generate your interactive roadmap
- **My “Now” lane (this sprint), the 2 to 3 quick wins I’ll build first:** A1: Spotlight Curated Rail and A2: "Why You'll Love this" Label
- **What I cut, and the “no” I’m protecting the scope from:** A8: Watch-Party (Spotlight), A9: Advance Filter Engine, and A10: Offline Download (Spotlight)
- **Prototype/roadmap screenshot link (paste into your deliverables):** https://claude.ai/artifact/M8yUcSRML8jyjhBuGaCcnF

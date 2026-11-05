# PRD & Prototype Sprint (Module 4)

## Pick & scope with MoSCoW
- **The “Now” feature I’m scoping (name + one-line core description):** A1, Spotlight Curated Rail: Hand-picked homepage rail that bypasses the algorithm
- **My finalized Must-Haves (after overriding the AI):** MUST HAVE (Sprint 1)
A fixed, hand-ordered homepage rail with no algorithmic ranking or re-sorting. Every viewer sees the same titles in the editor’s order, which is the “bypasses the algorithm” requirement itself and the direct answer to Marcus’s “I’m not a genre.”
A hard cap of 8–10 titles. A curated rail with 40 titles brings back the twenty-minute scroll, so the small size is what makes this a decision instead of a browse.
Placement on the first screen of the home page, with no scrolling needed. Her misery starts the moment the app opens, and a rail she has to scroll to find just adds to the scroll.
A tile that opens the existing title page and plays. Reuse the current tile component. If she can’t get from the rail to watching in one or two clicks, the rail is a list, not a fix.
A minimal way for editors to set the list, such as a config file or a single admin field holding ordered title IDs, deployable without an app release. Without this there is no curation. A full CMS is explicitly excluded.
TV and web only. Evening viewing is where the Moment of Misery happens, and the scope stops there. Mobile reuses whatever comes for free from the shared component.
- **What I demoted from Must → Should/Won’t, and why:** N/A

## Generate your Simplified PRD
- **One thing my PRD makes explicit that a vague brief would have missed:** A vague brief would say “bypass the algorithm” and leave it there. My PRD makes that testable: titles appear in the editor’s exact order with no re-ranking, the rail is capped at 10, and every reason line is pulled word for word from the editor’s file. These rules keep a developer from adding smart ordering or AI blurbs, which would bring back the genre-labelling Marcus rejected (“I’m not a genre, I’m a person”).

## Prompt-to-prototype sprint
- **Where did the prototype reveal a gap in my PRD logic? (what I had to update):** Five gaps, briefly:

Cap vs watched — Don’t backfill past the 10th when a title is hidden.
30:00 vs finished — Hitting 30:00 should count as finished for the rail, not only on leave.
“No scroll” vs swipe — No vertical scroll to find Spotlight; horizontal swipe is OK (make that explicit).
Detail vs speed — Spotlight tile → Play in one tap; detail stays optional.
Empty editor fields — No note → no reason copy; toast/tag don’t invent an editor line.
- **My prototype, as a link or a screenshot (publish or share from your tool; in Lovable that is Share → Share Preview, in Bolt Publish → Web. No share URL? Screenshot the working flow):** https://turbo-mandolin-ykw8o24.tmp.now/

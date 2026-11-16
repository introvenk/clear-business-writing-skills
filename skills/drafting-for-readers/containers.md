# Container Recipes

Each container inherits from its canonical parent (Report or Email) unless it is canonical itself. Only guidance beyond the core `SKILL.md` recipe is listed here. Where a container has none, that's stated explicitly rather than left blank.

## Report (canonical)
Optimizes for: a story that ends in a recommendation (Bernoff ch. 24). Full ROAM block. The front-loading lives in the title and executive summary: a reader who reads only those gets the conclusion. The body is the story: setup (the problem), analysis, then "tie everything together; then tell the reader what to do." A report without recommendations is incomplete. Don't hedge there.
- **Title:** descriptive and memorable, not a label ("Saving journalism in the digital era", not "Innovation"). A subtitle can carry the description.
- **Executive summary** (over ~10 pages): the story in brief, as if answering someone who asked about it at a bar. Use the most intriguing names, numbers and findings, not a section-by-section digest. Rewrite it from scratch with every draft.
- Use tables where items share a parallel structure. Move methodology and footnotes to end matter.
- Use a specific filename ("Q4 sales analysis", not "Report v6").

## RFC / ADR / design doc (inherits: report)
Optimizes for: options, tradeoffs, a recommendation that commits. Unlike a general report, state the recommendation in the first section. Engineering readers decide from it. If you had a bias going in (e.g. you favored one option before the analysis), say so up front (ch. 10). It reads as more credible, not less. *Beyond the book:* state the condition under which you'd reverse the recommendation.

## Incident postmortem (inherits: report)
Optimizes for: timeline, cause, prevention, with no blame-hedging. A cause is a causal claim, so make it the way ch. 10 says:
- State the cause and any bias.
- Cite the supporting evidence, with numbers in context.
- Evaluate competing explanations.
- Say how to test the conclusion.
- Say what to do about it.

Don't assert correlation as cause. State the cause as your best current understanding unless it's confirmed. *Beyond the book:* mark every reconstructed timestamp you haven't verified against logs as `(approx.)`.

## Email (canonical)
Optimizes for: speed to the ask (ch. 21). **100–250 words.** Response rates start dropping past 100. One topic per email. Send only to people who must act. Cc as few as possible, never Bcc.
- **Subject line:** states the content and, where possible, the ask ("July sales exceed quota by 20%", not "Some thoughts"). It becomes the thread's heading. Rewrite it after the body.
- **First substantive sentence:** a one-sentence summary that tells the whole story. No apology, no warm-up.
- **Body:** who I am (if needed), what's happening, what it means, then what you should do.
- **End:** the call to action with a deadline, more specific than the subject line ("Please send me an estimate by tomorrow").
- No tables (they render poorly), exclamation points, emojis or profanity.

## Escalation (inherits: email)
Optimizes for: ask + deadline. Never hand someone above you a problem without a recommendation (ch. 21). State what you need decided, your recommended option, and the deadline. *Beyond the book:* say who decides and what happens if the deadline passes.

## Status / leadership update (inherits: email)
Optimizes for: what changed and what the reader must do. Going upward, write more briefly and lead with the recommendation or decision you need. Going downward to staff, keep it under 400 words and to one topic, and state bad news up front (ch. 21).

## Standup / cadence (inherits: email)
Optimizes for: delta only. No recipe beyond the general one. The RED-phase baseline found the model already leads with the actual change unprompted, so there is no ritual-recitation failure to correct.

## Review & feedback (inherits: email)
Optimizes for: specific + respectful. Criticize the document, never the person. Only comment on sections you were actually given. Don't praise or critique content you weren't shown, even when a plausible-sounding compliment would fit. For full reviews, use `diagnosing-drafts`.

## Blog post (canonical)
Optimizes for: hook → insight. Under ~750 words. Title must intrigue and be easy to reference. Clarity beats keyword-stuffing. When you're given the outcome (what happened, what changed, what broke) but not the process, don't invent the process to fill in the narrative. Invented details include a week-by-week phase breakdown, a named internal artifact, an impact figure, or a specific detection story. They sound confident and they're exactly what this skill exists to catch. State what you actually know and stop. A shorter true account beats a longer plausible one.

## Social post (canonical)
Optimizes for: insight per unit attention (ch. 22). No more than 3–4 sentences, front-loaded, with a link and, where possible, a graphic.

## Press release (canonical)
Optimizes for: news over hype (ch. 23). Readers are anyone who can spread the word, not just journalists. Strip jargon, superlatives and stilted quotes. What's left is facts plus the company speaking directly to the reader: essentially a post saying "we did this, and here's why." Bracket every fact you don't have (investor quotes, prior funding totals, customer names, boilerplate) rather than inventing a plausible version. Flag the bracketed list for sign-off before distribution.

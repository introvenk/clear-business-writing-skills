# Container Recipes

Each container inherits from its canonical parent (Report or Email) unless it is canonical itself. Only guidance beyond the core `SKILL.md` recipe is listed here — where a container has none, the general recipe is the whole recipe, and that's stated explicitly rather than left blank.

Status / leadership update is intentionally not listed below — see `team-communications`, which already owns that container.

## Report (canonical)
Optimizes for: evidence → recommendation. Full ROAM block. Lead with the recommendation, then the evidence — not the reverse. Title: descriptive and memorable, not a label ("Saving journalism in the digital era", not "Innovation"); a subtitle can carry the description. Over ~10 pages: add an executive summary that is the report's story in brief — the most intriguing names, numbers, findings — not a section-by-section digest. Write it with every draft. Use a specific filename ("Q4 sales analysis", not "Report v6").

## RFC / ADR / design doc (inherits: report)
Optimizes for: options, tradeoffs, a recommendation that commits. State a specific recommendation in the first section, with the condition under which you'd reverse it. If you have a personal bias going in (e.g. you favored one option before the analysis), say so directly rather than writing around it — this reads as more credible, not less.

## Incident postmortem (inherits: report)
Optimizes for: timeline, cause, prevention — no blame-hedging. Mark every reconstructed timestamp you haven't verified against logs as `(approx.)`. State the cause as your best current understanding unless it's actually confirmed.

## Email (canonical)
Optimizes for: speed to the ask. **Target: under 250 words.** Subject line states the content ("July sales exceed quota by 20%", not "Some thoughts") — it becomes the thread's heading; rewrite it after the body. Opening sentences: your objective and the action you want. Rest of the email justifies it; no warm-up narrative.

## Escalation (inherits: email)
Optimizes for: ask + deadline + consequence. State what you need decided, by whom, by when, and what happens if it isn't decided in time. No container-specific guidance beyond the general recipe — the RED-phase baseline showed no failure here.

## Standup / cadence (inherits: email)
Optimizes for: delta only. No recipe beyond the general one. The RED-phase baseline found the model already leads with the actual change unprompted when given an undifferentiated fact list — there is no ritual-recitation failure to correct.

## Review & feedback (inherits: email)
Optimizes for: specific + respectful. Criticize the document, never the person. Only comment on sections you were actually given — don't praise or critique content you weren't shown, even when a plausible-sounding compliment would fit the context.

## Blog post (canonical)
Optimizes for: hook → insight. Under ~750 words. Title must intrigue and be easy to reference; clarity beats keyword-stuffing. When you're given the outcome (what happened, what changed, what broke) but not the process, don't invent the process to fill in the narrative — a week-by-week phase breakdown, a named internal artifact, an impact figure, or a specific detection story are exactly the kind of confident-sounding invented detail this skill exists to catch. State what you actually know and stop there; a shorter true account beats a longer plausible one.

## Social post (canonical)
Optimizes for: insight per unit attention. No container-specific guidance beyond the general recipe — the RED-phase baseline showed no failure here.

*Sourcing note: this recipe rests partly on inference from adjacent chapters rather than a directly-verified chapter — see the spec's Source verification status table.*

## Press release (canonical)
Optimizes for: news over hype. Readers are anyone who can spread the word, not just journalists. Strip jargon, superlatives, and stilted quotes; what's left is facts plus the company speaking directly to the reader — essentially a post saying "we did this, and here's why." Bracket every fact you don't have — investor quotes, prior funding totals, customer names, boilerplate — rather than inventing a plausible version, and flag the bracketed list for sign-off before distribution.

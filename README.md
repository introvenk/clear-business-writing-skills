# Clear Business Writing Skills

[![claude-code](https://img.shields.io/badge/claude--code-blue)](https://github.com/topics/claude-code)
[![claude-skills](https://img.shields.io/badge/claude--skills-blue)](https://github.com/topics/claude-skills)
[![business-writing](https://img.shields.io/badge/business--writing-green)](https://github.com/topics/business-writing)
[![technical-writing](https://img.shields.io/badge/technical--writing-green)](https://github.com/topics/technical-writing)
[![engineering-management](https://img.shields.io/badge/engineering--management-orange)](https://github.com/topics/engineering-management)
[![writing](https://img.shields.io/badge/writing-green)](https://github.com/topics/writing)
[![documentation](https://img.shields.io/badge/documentation-lightgrey)](https://github.com/topics/documentation)
[![ai-agent-skills](https://img.shields.io/badge/ai--agent--skills-purple)](https://github.com/topics/ai-agent-skills)

Three [Claude Code](https://claude.com/claude-code) skills for engineering-management
business writing, derived from Josh Bernoff's *Writing Without Bullshit* and built with
TDD discipline: no guidance was written until a no-guidance baseline test actually
demonstrated the failure it addresses.

## Skills

### `drafting-for-readers`
Drafting help for RFCs/ADRs/design docs, reports, incident postmortems, review feedback,
emails, escalations, standup/cadence updates, blog posts, social posts, and press
releases. A positive recipe, not a prohibition list — states what good output *is* rather
than listing what to avoid. Its central rule, "never invent specificity," exists because
baseline testing found language models silently fabricate names, causes, commitments, and
narrative detail more often and more consistently than any other failure tested.

Not for status/leadership updates — pair it with a status-update-specific skill if you
have one (e.g. `team-communications`).

### `diagnosing-drafts`
Reviews an existing draft — someone else's or your own — for clarity problems: meaning
ratio, passive voice, jargon, hedging, buried leads, unsourced numbers. Diagnoses and
suggests a fix; doesn't rewrite over the author's voice.

### `improving-writing-culture`
For team-level problems: writing standards, document templates, review processes, and
diagnosing why an organization's documents are consistently unclear. Addresses the system
around the writing, not any single document.

### `communicating-clearly`
Applies the same clarity principles to real-time conversational replies instead of
authored documents — invoke it explicitly to tighten, shorten, or de-hedge a response
mid-conversation.

## Install

```
/plugin marketplace add https://github.com/introvenk/clear-business-writing-skills
/plugin install clear-business-writing@clear-business-writing
```

## How this was built

Each container recipe traces back to an actual observed failure, not a predicted one.
27 no-guidance baseline runs were tested across 11 document types before any skill
content was written; `drafting-for-readers` was then re-tested with the skill present to
confirm the fabrication behavior it targets was actually corrected. Guidance was dropped
for predicted failures (hedging, buried leads, non-committal recommendations) that never
showed up in testing, and the one dominant unpredicted failure — invented specificity —
became the skill's central rule instead.

## License

MIT

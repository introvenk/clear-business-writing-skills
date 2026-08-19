# Meaning Ratio

**Method:** meaning ratio = meaningful words ÷ total words. A word is meaningful if removing it would remove information the reader needs — not just anything that "sounds important."

Below 70%: bullshit territory. Around 80%+: readable. This is a judgment heuristic, not a metric to optimize — a technical RFC with dense but necessary jargon can carry more real information than its raw ratio suggests. Use it to flag suspicious passages, not to score a whole document.

## Worked example

**Before** (30 words):
> "At this point in time, it is important to note that, going forward, we will be looking into the possibility of potentially exploring a migration to a new vendor solution."

Meaningful words: *migration*, *new*, *vendor* — 3 of 30. Ratio: 10%. Nearly every other word is throat-clearing ("at this point in time," "it is important to note that," "going forward," "looking into the possibility of potentially exploring," the vague trailing "solution") that could be deleted without losing information.

**After** (6 words):
> "We're evaluating a new vendor migration."

Meaningful words: *evaluating*, *new*, *vendor*, *migration* — 4 of 6. Ratio: 67%. Every word in the compressed version carries information the original also had — the original just buried it under 24 extra words.

## How to apply it
Read a passage. Cross out words that could be deleted without losing anything the reader needs to know. If more than 30% of the passage disappears, flag it as bullshit-heavy and propose the compressed version directly — don't just report a percentage back to the author.

---
name: drafting-for-readers
description: Use when drafting any business document for an engineering-management audience — reports, RFCs, ADRs, design docs, postmortems, review feedback, emails, escalations, status or leadership updates, standup or daily/cadence updates, blog posts, social posts, or press releases — before or while writing the first draft.
---

# Drafting for Readers

## Overview
Every piece of business writing exists to save the reader time. Draft with the reader's payoff in view, not your own process. Source: Bernoff, *Writing Without Bullshit*.

## Iron Imperative
Before writing, ask: what does the reader need to decide or do, and what's the fastest path to it? Treat their time as more valuable than yours.

## ROAM
**R**eaders (who exactly?), **O**bjective (what will they know or believe after?), **A**ction (what will they do next?), i**M**pression (what will they think of you?). Then compress it into one **target sentence**: *"After reading this, [readers] will realize [objective], so they will [action] and think of me as [impression]."* Cut anything that doesn't serve it. Infer before drafting, and re-check before revising. Tier by container (see `containers.md`):
- **Full block** (RFC, postmortem, report, press release): write all four plus the target sentence.
- **One line** (email, escalation, status update, review & feedback, blog): state the target sentence only.
- **Silent** (standup, social): infer, don't surface.
- **Any tier:** if reader or objective can't be inferred, ask. Don't assume.

## Point, support it, then stop
State the point first: conclusion, then reasoning, so a reader who stops early still gets it. Write the title/subject line before drafting and rewrite it after. If that's all they read, it should still say something useful. Support it. Stop. Don't restate the point, and don't add a closing summary paragraph the reader didn't ask for.

## Recommend, don't just describe
If the reader has to act, tell them what to do. Address them as "you." Writing upward, stay respectful but still recommend. A problem handed over without a recommendation, or a report that ends without one, is incomplete (ch. 9, 21, 24).

## Numbers (ch. 10)
- Compare every number to something familiar or to its history. Never give a growth rate without its base.
- Show at most three significant digits, and no more precision than you actually have. Keep "percentage points" distinct from "%".
- Cite each statistic's source and date. Before using it, check who produced it, how, from what sample, and how old it is.
- A claim that X caused Y needs evidence, competing explanations ruled out, and a way to test it.

## Reveal structure (ch. 11)
Anything over ~300 words needs visible structure:
- **Headings:** descriptive, following the reader's order (problem → options → recommendation), at most two levels.
- **Lists:** bullets for three or more parallel items, numbers for a sequence. "Firstly" or "on the other hand" in prose means it wants to be a list.
- **Tables:** use one when items share parallel attributes. Not in email.

## Long documents: plan before prose (ch. 14)
For anything report-sized, draft a **fat outline** first: headings plus a mix of draft text, descriptions of what goes there, and placeholders for missing facts. Get the structure agreed (with the user, or against ROAM) before writing full prose.

## Handing over a draft (ch. 18)
When you return a draft for review, say what you're unsure of, what kind of feedback you want (structure or wording), and what isn't worth the reviewer's time. No apologies or justifications. When feedback comes back, take each edit one of three ways: accept it, fix what it revealed some other way, or reject it for a stated reason. When revising, prefer cutting and rearranging to adding.

## Never invent specificity
If a name, cause, commitment, number or reviewed-content detail isn't in your source material, don't manufacture one. Flag it explicitly with a bracketed placeholder or an inline "to be confirmed". This covers:
- **people** you weren't given names for
- **causes or attribution** you weren't given a reason for
- **commitments made on someone else's behalf**
- **claims of having reviewed content you weren't shown**

This applies in long-form writing too. An invented project-phase breakdown or impact figure is as fabricated as an invented name, even though it reads as narrative. (This rule comes from baseline testing of model output, not from the book.)

See `containers.md` for the recipe per document type.

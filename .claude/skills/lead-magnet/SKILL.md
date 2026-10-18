---
name: lead-magnet
description: Designs and writes a free lead magnet that gets the right people to raise their hand and leads naturally to the main offer. It picks one narrow problem, chooses a format that takes under 10 minutes to use (checklist, cheat sheet, template, swipe file, short guide, scorecard or quiz outline, calculator spec), writes 5 title options and the outline, then writes the full finished content, plus the opt-in page headline and bullets and the delivery email. Use it when the user wants a freebie, an opt-in offer, or a way to collect leads or grow an email list. Triggers include "lead magnet", "freebie", "free guide", "free checklist", "free download", "opt-in", "something to give away", "grow my email list", "collect emails", "cheat sheet", "scorecard" and "quiz".
---

# Lead magnet

Produces one complete free resource, ready to publish: the strategy, 5 titles, the full content, the opt-in page brief and the delivery email.

## Before you start

1. Open every file in `business/` and read the `status:` line in its frontmatter. If any file says `status: empty`, stop and tell the user: "Your business files are not set up yet. Type `/setup` first, then run `/lead-magnet` again." Write nothing else.
2. If a file says `status: draft`, continue, and mention in the hand-off that the lead magnet rests on unconfirmed facts.
3. Read these business files:
   - `business/01_BUSINESS.md`: "Positioning" (who you do not want), "What makes us different", and "Language and market" (the language of every deliverable).
   - `business/02_AUDIENCE.md`: "Dream customer" (awareness level), "Pains", "Dream outcome", "What they have tried", "What holds them back", "Language bank", "Best customer ever".
   - `business/03_VOICE.md`: "Tone", "How we address the reader", "Words we use", "Words we never use", "Writing samples".
   - `business/04_OFFER.md`: "Main offer", "Guarantee", "Other offers" (look for an existing free offer), "Customer journey", "Main call to action".
   - `business/05_PROOF.md`: all of it. It is the only source of results, numbers and client stories.
   - `business/06_RULES.md`: all of it, especially "Legal and industry rules". It wins over everything else.
4. Read these knowledge files if they exist. If one is missing, skip it and rely on the core principles below.
   - `knowledge/Lead_Magnets.md`
   - `knowledge/Hooks_And_Headlines.md`
   - `knowledge/Messaging_Psychology.md`
5. Look in `output/lead-magnets/` for earlier work. If one already covers the same problem, ask whether to improve it or make a new one.

## Ask only what is missing

Ask at most 3 questions, all in one message, and only for what the request and the business files do not answer. If nothing is missing, skip this step.

1. "Do you already have material for this, like a process you walk clients through, a checklist you use, or notes on the mistakes you see most? Paste it, or say no and I will draft from your business files."
2. "Any format you prefer? (a) checklist, (b) cheat sheet, (c) template, (d) short guide, (e) scorecard or quiz, (f) you pick"
3. "How will people get it? (a) a PDF or document, (b) a page on your website, (c) not sure yet"

If "Other offers" in `04_OFFER.md` already lists a free offer, do not ask what to make. Start from that one.

## Core principles

- Specific beats broad. "The 7 point checklist before you send your first invoice" beats "The complete guide to running a business". One person, one problem, one result.
- Solve a problem they feel now. Pick a pain the dream customer already names in their own words, not one you think they should have. Their phrasing from the "Language bank" goes in the title.
- A quick win builds trust. The reader should get one small, real result within a day. That result is what makes them believe the paid offer will work too.
- Lead to the offer, never replace it. Solve one slice of the problem completely and make the rest of the problem visible. If it solves everything, nothing is left to buy. If it solves nothing, nobody trusts the offer.
- The name sells the download. Most people decide on the title alone. Name a specific outcome, a specific number of items, or a specific person.
- Deliver what the title promises. If it says 9 mistakes, there are 9. If it says 10 minutes, it takes 10 minutes. Be generous with usefulness, not with length.
- Short and usable beats long. Under 10 minutes to read or fill in. Checklists, templates and cheat sheets get used. Long ebooks get saved and forgotten.
- Attract buyers, filter out the rest. The topic should appeal to people who can buy the main offer and bore the people "Positioning" says you do not want.
- The next step feels obvious. The end bridges from the quick win to the bigger problem and gives one call to action, the main one.
- No claims beyond `05_PROOF.md`. Any example that is not a real client story is clearly labeled as an example. Missing proof becomes `[ADD PROOF: what is needed]`.

## Steps

1. Check "Other offers" in `04_OFFER.md`. If a free offer is listed, use its name, format and problem as the starting point. If it breaks a principle above (too broad, too long, unrelated to the main offer), keep it, and propose a narrower version next to it rather than replacing it silently.
2. Pick the problem. List 3 candidates from "Pains" and the "Language bank". For each, answer yes or no: felt now, fully solved by the main offer, and a quick win possible in under 10 minutes. Choose a candidate with three yes answers. Then write one sentence: "This helps [dream customer] [quick win], so they can [next result], which [main offer] delivers in full."
3. Pick the format that fits the problem:
   - Checklist: steps people forget or do in the wrong order.
   - Cheat sheet: reference facts they look up again and again.
   - Template: something they must write, plan or fill in.
   - Swipe file: examples they can copy and adapt, all written for this business.
   - Short guide: a process that needs a little explanation.
   - Scorecard or quiz outline: "where do I stand?" questions with a result.
   - Calculator spec: a problem that is really a number.
   Say in one sentence why this format fits.
4. Write 5 title options, each with a short subtitle and an angle label (Pain, Outcome, Curiosity, Proof, Contrarian, Identity, Mistake, Speed). No more than two share an angle. Recommend one and say why.
5. Write the outline: the sections or items in order, with one line on what each delivers.
6. Write the full content, finished and ready to paste into a document:
   - Short guide: up to about 1,500 words, with a short intro, numbered sections and one action per section.
   - Checklist: every item, each with a one line why or how.
   - Cheat sheet: every entry, grouped, fits on one or two pages.
   - Template: every field with fill-in instructions, plus one filled-in example marked as an example.
   - Swipe file: every example complete, with a line on when to use it.
   - Scorecard or quiz: all questions and answer options, the scoring, 3 result bands, and what each band means and should do next.
   - Calculator spec: inputs, the formula in plain words, outputs, how to read the result, and one worked example with made-up inputs marked as an example.
7. End the content with a next step: one or two sentences that name what the reader just fixed and what is still open, then the main call to action worded exactly as in `04_OFFER.md`.
8. Write the opt-in page brief for `/landing-page`: headline, subheadline, 3 to 5 bullets that each promise one concrete thing inside, button text, and one line under the form.
9. Write the delivery email for `/email`: 3 subject lines with angle labels, preview text, and a body under 120 words with the link, one tip for using the resource today, and a short line on what comes next.
10. Run the quality check, fix every failure, then save.

## Output format

Template headings stay in English so other skills can find the sections. Everything the audience will read is written in the language from "Language and market".

```markdown
---
type: lead-magnet
date: YYYY-MM-DD
format: [checklist, cheat sheet, template, swipe file, short guide, scorecard, calculator spec]
language: [from 01_BUSINESS.md]
---

# Lead magnet: [recommended title]

## Strategy
Dream customer: [from 02_AUDIENCE.md]
Problem it solves: [one sentence, in their words]
Quick win: [what they can do or know within a day]
Why it leads to the main offer: [one sentence]
Format and why: [one sentence]
Time to use: [minutes]

## Title options
1. [Angle]: [Title]. [Subtitle]
2. [Angle]: [Title]. [Subtitle]
3. [Angle]: [Title]. [Subtitle]
4. [Angle]: [Title]. [Subtitle]
5. [Angle]: [Title]. [Subtitle]
Recommended: [number], because [reason]

## Outline
1. [section or item]: [what it delivers]

## Full content
[The complete lead magnet with its own headings, ready to paste into a document]

### Next step
[Bridge to the bigger problem, then the main call to action]

## Opt-in page brief (for /landing-page)
Headline: [text]
Subheadline: [text]
Bullets:
- [one concrete thing inside]
Button text: [text]
Under the form: [text]

## Delivery email (for /email)
Subject lines:
1. [Angle]: [subject]
2. [Angle]: [subject]
3. [Angle]: [subject]
Preview text: [text]
Body:
[under 120 words, with [LINK TO LEAD MAGNET]]

## Open placeholders
- [every bracket left in the file]
```

## Quality check

Run `.claude/skills/review/CHECKLIST.md` on everything in the file and fix every failure before saving. Never save with a failure in section 1 (Truth) or section 2 (Rules). Then check these lead magnet specifics:

- The content delivers exactly what the recommended title promises, including any number in it.
- It takes under 10 minutes to read or fill in.
- It solves one problem fully and does not give away the whole main offer.
- Every example that is not from `05_PROOF.md` is labeled as an example.
- The next step and the opt-in page use the same call to action, worded as in `04_OFFER.md`.
- Every opt-in bullet points to something that is actually in the content.

## Save

Save to `output/lead-magnets/YYYY-MM-DD_slug.md`, using today's date and a short slug from the recommended title, for example `first-invoice-checklist`. If the file already exists, add `-2` to the slug.

## Hand-off

Tell the user, in the language they wrote in:

1. The file path and the recommended title.
2. Every open placeholder, as a list, with what is needed to fill it (the download link is always one until the file is hosted).
3. How to publish it: paste the "Full content" section into any document or design tool and export it as a PDF, or put it on a web page.
4. An offer to add it to "Other offers" in `business/04_OFFER.md`, so other skills know it exists. Do not change that file without a yes.
5. If any business file was `status: draft`, say which, and that the lead magnet should be checked once it is confirmed.
6. What to run next:
   - `/landing-page` to build the opt-in page from the brief.
   - `/email` to finish the delivery email and add a short follow-up sequence that leads to the main call to action.
   - `/content` to promote it with a comment keyword in short form videos.
   - `/ads` to promote it with paid traffic once the opt-in page is live.

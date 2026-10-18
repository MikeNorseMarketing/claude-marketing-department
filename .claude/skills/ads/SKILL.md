---
name: ads
description: Writes paid ads for the business described in business/, in three modes. Hooks gives a bank of 15 to 20 opening lines across at least 5 labeled angles. Static ads gives 3 to 5 complete Meta ads (primary text, headline, description, image idea), with an optional Google Search mode. Video scripts gives 3 scripts of 30 to 60 seconds with alternative hooks and on screen notes. Every claim comes from business/05_PROOF.md, and every ad points to one call to action. Use it when the user wants ad copy, hooks, headlines, primary text or a video ad script. Trigger phrases include "write ads", "ad copy", "hooks", "ad headlines", "Meta ads", "Facebook ad", "Instagram ad", "Google Search ads", "video ad script", "UGC script" and "new ad angles".
---

# Ads

Produces ready to paste ad copy in one of three modes: a hook bank, complete static ads, or video ad scripts.

## Before you start

1. Open the frontmatter of every file in `business/` (01 to 06). If any file has `status: empty`, stop and tell
   the user: "Your business files are not set up yet. Type `/setup` first, then run `/ads` again." Write nothing.
2. A file with `status: draft` can be used. Note which files were drafts so you can mention it in the hand-off.
3. Read these business files in full:
   - `business/01_BUSINESS.md` for positioning, "What makes us different", "Origin story" and "Language and market"
   - `business/02_AUDIENCE.md` for "Dream customer" (including awareness level), "Pains", "Language bank" and "What holds them back"
   - `business/03_VOICE.md` for "Tone", "How we address the reader", "Words we never use" and "Writing samples"
   - `business/04_OFFER.md` for "Main offer", "Price", "Guarantee", "Other offers" and "Main call to action"
   - `business/05_PROOF.md`, the only allowed source of numbers, results, names and quotes
   - `business/06_RULES.md`, which wins over everything else
4. Read these if they exist and skip them quietly if not: `knowledge/Hooks_And_Headlines.md`,
   `knowledge/Ad_Scripting.md`, `knowledge/Messaging_Psychology.md`. The core principles below are enough without them.
5. Look in `output/pages/` and `output/lead-magnets/` for the page or freebie the ad sends people to, and in
   `output/ads/` for earlier ads, so you build on them instead of repeating the same angles.
6. Write every ad in the language set under "Language and market" in `01_BUSINESS.md`, even if the user talks
   to you in another language.

## Ask only what is missing

Ask at most 3 short questions, all in one message, and only for what the request and the files do not answer.

1. Which mode? (a) hooks, (b) static ads for Meta, (c) Google Search ads, (d) video ad scripts.
2. Where does the ad send people? (a) the main call to action in `04_OFFER.md`, (b) a free offer from
   "Other offers", (c) a specific page, paste the link or the file name.
3. Who will see it? (a) cold, people who have never heard of the business, (b) warm, people who follow you,
   visited the site or are on the list, (c) both.

For Google Search, replace question 3 with: "Which 1 to 3 search phrases should these ads show up for?"
If the user says "just go", use the main call to action, write for a cold audience, and say so in the hand-off.

## Core principles

- **The hook decides everything.** People decide in the first line, or the first 3 seconds of a video, whether
  to keep going. Spend most of your effort there. Write more hooks than you need and keep the best.
- **Specific beats clever.** A number, a timeframe, a named situation or a quote from the language bank does
  more than any adjective. "Profit per job by the 10th" beats "better financial clarity".
- **Match the awareness level** in `02_AUDIENCE.md`. Unaware: open with a story or a symptom they recognize.
  Problem aware: name the pain in their own words. Solution aware: show why this approach beats what they
  tried. Product aware: lead with the offer, the proof and the guarantee. Most aware: the offer and the next step.
- **One ad, one idea, one call to action.** One pain, one promise, one proof point, one thing to do. If an ad
  needs two ideas, it is two ads.
- **The ad must match the page.** The promise, the key words and the offer in the ad must show up at the top
  of the page it links to. A click that lands somewhere unexpected is a wasted click. Flag any mismatch.
- **Cold and warm are different ads.** Cold readers need a reason to care and a small next step, often the free
  offer. Warm readers already know you, so lead with proof, the offer and a direct call to action.
- **Claims come only from `05_PROOF.md`.** If an ad needs proof that is not there, write
  `[ADD PROOF: what is needed]` instead of inventing it. Note which proof item each ad uses.
- **Follow platform policy.** Never call out a personal attribute of the viewer ("Are you in debt?",
  "Unhappy with your weight?"). No before and after images or copy that implies a guaranteed result. No
  sensational health or money claims. No fake buttons, fake notifications or fake screenshots in image ideas.
- **Undershoot for skeptical or wealthy readers.** Use a typical result instead of the best one and state it
  plainly. A smaller claim that is believed sells more than a bigger one that is doubted.
- **Write it to be said out loud.** Short sentences, everyday words, the reader address from `03_VOICE.md`.
  If a line sounds like a brochure, rewrite it.

## Steps

1. Run "Before you start", ask the missing questions in one message, and wait for the answers.
2. Write a short private brief: the awareness level, the destination and what it promises, 3 to 5 pains from
   the language bank, the dream outcome, the biggest objection, and the proof items you may use with the
   section each one comes from.
3. Pick the angles from Pain, Curiosity, Proof, Contrarian, Identity, Story and Transformation. Use Urgency
   only if `04_OFFER.md` or the user names a real deadline or a real limit.
4. Write the chosen mode:
   - **Hooks.** 15 to 20 opening lines grouped by angle, at least 5 angles, no more than 4 hooks per angle.
     Each hook must work as the first line of a static ad and as the first spoken words of a video. Keep most
     under 12 words. Star your top 3 and give one line on why for each.
   - **Meta static ads.** 3 to 5 complete ads, each with an angle label, and no angle used more than twice.
     Each ad has a short primary text under 125 characters (this is what shows before "See more"), a long
     primary text of 80 to 200 words that runs hook, problem, what changes, proof, call to action, a headline
     under 40 characters, a description of about 30 characters (often hidden on phones, so never put the key
     point there), and an image idea.
   - **Google Search ads.** 10 to 15 headlines under 30 characters, 4 descriptions under 90 characters, and two
     path fields of up to 15 characters each. Google combines them in any order, so every line must make sense
     alone and next to any other. Use the search phrase in at least 3 headlines and the call to action in at
     least 2. Label each headline with its angle.
   - **Video scripts.** 3 scripts, each with a different angle, 30 to 60 seconds long (about 75 to 150 spoken
     words). Structure: hook in the first 3 seconds, explain the hook, who we are and why listen, proof, call to
     action. The hook must land in what is said, what is shown and the text on screen at the same time. Give
     each script 3 alternative hooks with angle labels, and notes on what to show for every part.
5. Count the characters of every limited field, spaces included, and write the count in brackets after it.
   Cut anything over the limit. Recount any line within 3 characters of the limit.
6. Compare the ads with the destination page. If the page is missing or promises something else, note it.
7. Run the quality check below and fix every failure.
8. Save the file and hand off.

## Output format

Use this template. Include only the section for the chosen mode, and delete the instruction text in brackets.

```markdown
# Ads: [short name]

Date: YYYY-MM-DD
Mode: [Hooks | Meta static | Google Search | Video scripts]
Audience: [cold | warm | both], awareness level: [from 02_AUDIENCE.md]
Sends to: [page, link or file]
Call to action: "[exact wording from 04_OFFER.md]"
Language: [from 01_BUSINESS.md]

## Hooks

### Pain
1. [hook]
2. [hook]

### Curiosity
3. [hook]

[at least 5 angle groups, 15 to 20 hooks in total, numbered straight through]

Top 3: #[n] because [one line], #[n] because [one line], #[n] because [one line]

## Ad 1: Pain

Primary text, short ([n] characters):
[text]

Primary text, long:
[text]

Headline ([n] characters): [text]
Description ([n] characters): [text]
Image idea: [what the image shows, any text on it, format 1:1 or 4:5]
Proof used: [05_PROOF.md > section > item, or none]

## Google Search

Search phrases: [phrases]
Headlines:
1. (Pain) [text] ([n])
Descriptions:
1. [text] ([n])
Paths: /[path one]/[path two]

## Script 1: Story, about [n] seconds

| Part | Spoken | On screen |
|---|---|---|
| Hook, 0 to 3 s | [words] | [visual and text overlay] |
| Explain the hook | [words] | [visual] |
| Who we are and why listen | [words] | [visual] |
| Proof | [words] | [visual] |
| Call to action | [words] | [visual and text overlay] |

Alternative hooks:
1. (Curiosity) [hook]
2. (Proof) [hook]
3. (Contrarian) [hook]
Proof used: [05_PROOF.md > section > item, or none]

## Open placeholders
- [ADD PROOF: ...]

## Notes
- Message match: [ok, or what to change on the page]
```

## Quality check

Run every item in `.claude/skills/review/CHECKLIST.md` on the finished ads and fix what fails. Sections 1 and 2
are blocking, so never save ads that fail them. Then check these ad specific points:

- Every limited field is under its limit and shows its character count.
- No hook, headline or image idea calls out a personal attribute or implies a guaranteed result.
- Two modes are exceptions to the "3 to 5 variants" rule in section 5. The hook bank has 15 to 20 hooks, at
  least 5 angles and no more than 4 hooks per angle. Google Search has 10 to 15 headlines spread over at
  least 4 angles. Meta static ads and video scripts follow the normal rule.
- Each ad has one idea and one call to action, worded the same way as in `04_OFFER.md`.

## Save

Save to `output/ads/YYYY-MM-DD_slug.md`, using today's date and a slug of 2 to 5 lowercase words joined by
hyphens that names the mode and the topic, for example `output/ads/2026-03-14_meta-static-job-costing.md`.
If that file already exists, add `-v2` (or the next number) instead of overwriting it.

## Hand-off

Tell the user, in a few short lines:

- The file path, the mode, and how many hooks, ads or scripts it holds.
- Your top pick and why, in one sentence.
- Every open placeholder, such as `[ADD PROOF: ...]` or a missing link, and which business file would fill it.
- Any business file that was still `status: draft`, and any message match problem with the destination page.
- A testing tip: run at least 3 different hooks against each other before changing anything else in the ad.
- What to run next: `/landing-page` if the destination page does not exist or does not match the ads,
  `/lead-magnet` if the ads promote a freebie that does not exist yet, `/email` for the follow up after
  people sign up, and `/review` for a second check after the user edits anything.

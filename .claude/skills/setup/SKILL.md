---
name: setup
description: Interviews the user about their business and writes the six files in business/ that every other skill reads (business, audience, voice, offer, proof, rules). Run this first, before any other skill. Can read the user's website to draft answers, can pause and continue later, and can update a single file. Use when the user says setup, set up, get started, onboard me, fill in my business, update my business files, or types /setup, /setup continue, or /setup offer (or another file name).
---

# Setup

Produces the six business files in `business/`. Everything the marketing department writes later is built on
these answers, so this is the most important 20 to 30 minutes in the whole folder.

## Before you start

1. Read `CLAUDE.md` and all six templates in `business/`. Each template has a frontmatter `status`
   (`empty`, `draft` or `confirmed`) and sections with a short explanation, an example from a made-up company,
   and a `[placeholder]`.
2. Work out which mode you are in:
   - **All files empty:** full setup. Start at "Welcome".
   - **Some files empty, some not, or the user typed `/setup continue`:** continue. Say which files are done,
     then start at the first block whose file is still `empty`.
   - **The user named a file or topic** (for example `/setup offer` or "update my proof"): update mode. Run only
     that block, show the changes, and save that one file.
   - **All files filled and no file named:** ask whether they want to update one file or start over. Never
     start over without a clear yes.

## Welcome

Say this in your own words, short:

- You will ask questions in six short blocks: business, audience, offer, proof, voice, rules.
- It takes about 20 to 30 minutes. Each file is saved as soon as its block is done, so they can stop any time
  and type `/setup continue` later.
- Short answers are fine. "I don't know" is fine too. You will never make anything up to fill a gap.
- If they have a website, you can read it first and draft answers, so they mostly confirm and correct.

Then ask for the website URL (or "no website").

## Website head start (optional)

If they give a URL, read the homepage with your web fetch tool, plus up to three linked pages that look useful
(about, services or pricing, reviews or testimonials). Use what you find to draft answers for blocks 1 to 5.

- Show each draft at the start of its block and ask "What's wrong or missing?" instead of asking every question.
- Website text describes how the business sees itself, not how customers talk. Never put website copy in the
  language bank in `02_AUDIENCE.md` as if it were a customer quote.
- Testimonials found on the website can go in `05_PROOF.md`, marked "From website, confirm permission".
- If a page cannot be read, say so and continue with questions.

## The interview

One block at a time. Ask the questions of a block together in one message, numbered, so the user can answer in
one reply. Use multiple choice where the template allows it (awareness level, reader address, tone, language).
If an answer is vague ("great service", "quality"), ask once for a concrete example, then move on.

**Block 1, your business** (writes `01_BUSINESS.md`)
1. Business name, website, and where you operate.
2. What do you sell? Explain it like you would to a friend.
3. Who do you not want as a customer?
4. Why did you start this business? The real moment, not the market gap.
5. What do you do that the alternatives don't?
6. Which language should all marketing be written in, which country or region do you sell in, and which currency?

**Block 2, your dream customer** (writes `02_AUDIENCE.md`)
1. Describe your dream customer: role, age range, situation, income or company size.
2. What frustrates them most when they come to you? Use their words if you remember them.
3. What does life look like for them after working with you?
4. What have they tried before, and why didn't it work?
5. Why do they put off buying, and what are they afraid will go wrong?
6. Tell me about your best customer ever: before, after, and why they were the best.
7. How aware are they? (Unaware of the problem / Know the problem / Know solutions exist / Know you / Ready to buy)
8. Any exact quotes from customers you can paste (emails, reviews, things said on calls)?

**Block 3, your offer** (writes `04_OFFER.md`)
1. Your main offer: name, what is included, who it is for, how and when it is delivered.
2. The price, or the range and what changes it. Do you show it publicly?
3. Do you have a guarantee? Give the exact wording, or say none.
4. Anything free, cheaper, or premium besides the main offer?
5. What happens step by step from first contact to result?
6. The one thing you want people to do (book a call, buy, sign up), and the link.

**Block 4, your proof** (writes `05_PROOF.md`)
Explain first: only what goes in this file can ever appear in the copy, so more real proof means better copy.
1. Paste your best testimonials, word for word, with name and context. Can the names be used publicly?
2. Results with real numbers (before and after), and where each number comes from.
3. Numbers that show volume or experience (customers served, years, ratings), with source and date.
4. Certifications, memberships, awards, press.

**Block 5, your voice and look** (writes `03_VOICE.md`)
1. Pick the tone that fits best, then add your own words: (Direct and practical / Warm and personal /
   Expert and calm / Bold and energetic / Something else).
2. Should copy say "you", "we and you", or stay neutral?
3. Words you like to use, and words you never want to see.
4. Two or three brands or people whose writing you like.
5. Paste three to five sentences you wrote yourself and like (an email, a post, anything).
6. Brand colors (hex codes if you have them, otherwise describe them), fonts, and a link to your logo.
   "Pick later" is fine.

**Block 6, your rules** (writes `06_RULES.md`)
1. Is your industry regulated (health, finance, legal, real estate, supplements, income claims, other)?
   What can't you say?
2. Anything your marketing must never say or promise?
3. Anything it must always do (a disclaimer, a phrase, a call to action wording)?
Keep the five fixed rules in the template unless the user gives a clear reason to remove one.

## Writing each file

Write the file right after its block, before starting the next block.

1. Start from the template. Keep every heading and the short explanation under it.
2. Replace each `[placeholder]` with the user's answer, in their words where possible.
3. **Delete every "Example:" line and example block.** The examples are from a made-up company. If one is left
   in, other skills will treat it as a fact about this business.
4. Anything the user did not know becomes `[Not known yet]`. Never guess.
5. Write only what the user told you, or what their website says. You may tidy the wording, but do not add
   rules, policies, claims, reasons, calls to action or explanations they did not give. The fixed rules in
   `06_RULES.md` are the only exception, and they stay as they are.
6. Write the content in the business's language from Block 1, except the headings, which stay as they are.
7. Set the frontmatter to `status: draft` and `last_updated:` today's date (YYYY-MM-DD).
8. Tell the user in one line that the file is saved, then move to the next block.

## Finish

1. Show a short summary per file: three bullets each, plus any `[Not known yet]` gaps.
2. Ask: "Is anything wrong or missing?" Fix what they point out.
3. When they confirm, set `status: confirmed` in all six files.
4. Point out the gaps that will hurt the copy most, usually proof and customer quotes, and that they can
   add them any time with `/setup proof` or `/setup audience`.
5. Suggest a first task, picked from what they told you:
   - No lead magnet yet: `/lead-magnet`
   - Has an offer and a call to action: `/landing-page`
   - Runs or wants to run ads: `/ads`
   - Has a list but rarely emails it: `/email`
   - Posts on social media: `/content`

## Rules for this skill

- Never invent a fact, number, quote, or name. Gaps stay as `[Not known yet]`.
- Point out gaps, never forecast results. Say "a guarantee would give the copy more to work with", not
  "a guarantee would lift conversion a lot".
- Write plainly in your messages too: "20 to 30 minutes", not "20–30", and no em dashes.
- Never overwrite a file that has `status: confirmed` without asking first.
- Keep it moving. If the user seems tired, offer to stop and say `/setup continue` picks up where they left off.

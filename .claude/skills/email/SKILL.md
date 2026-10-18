---
name: email
description: Writes complete email sequences for the business described in business/, ready to paste into any email tool. Three types. A welcome sequence for people who download a lead magnet (the default, 5 emails over about 7 days that deliver the freebie, build trust and lead to the main call to action). Nurture or newsletter emails with one idea each. A 3 email re-engagement sequence for an old list. Every email gets send timing, 3 subject lines with angle labels, preview text, body, one call to action and an optional P.S. Use it when the user wants emails, an email sequence, welcome emails, a nurture or drip sequence, a newsletter, an autoresponder, or a way to wake up an old list. Trigger phrases include "write emails", "email sequence", "welcome sequence", "nurture emails", "newsletter", "drip", "autoresponder", "follow up emails" and "re-engage my list".
---

# Email

Produces a full email sequence with timing, subject lines, preview text and finished bodies, ready to paste.

## Before you start

1. Open the frontmatter of every file in `business/` (01 to 06). If any file has `status: empty`, stop and tell
   the user: "Your business files are not set up yet. Type `/setup` first, then run `/email` again." Write nothing.
2. A file with `status: draft` can be used. Note which files were drafts so you can mention it in the hand-off.
3. Read these business files in full:
   - `business/01_BUSINESS.md` for "Company", "Origin story", "What makes us different" and "Language and market"
   - `business/02_AUDIENCE.md` for "Dream customer" (including awareness level), "Pains", "Dream outcome",
     "What they have tried", "What holds them back", "Language bank" and "Best customer ever"
   - `business/03_VOICE.md` for "Tone", "How we address the reader", "Words we never use" and "Writing samples"
   - `business/04_OFFER.md` for "Main offer", "Guarantee", "Other offers", "Customer journey" and "Main call to action"
   - `business/05_PROOF.md`, the only allowed source of numbers, results, names and quotes
   - `business/06_RULES.md`, which wins over everything else
4. Read these if they exist and skip them quietly if not: `knowledge/Lead_Nurture.md`,
   `knowledge/Messaging_Psychology.md`, `knowledge/Hooks_And_Headlines.md`. The core principles below are
   enough without them.
5. Look in `output/lead-magnets/` for the freebie the welcome sequence delivers, and in `output/emails/` for
   earlier sequences, so new emails do not repeat the same stories.
6. Write every email in the language set under "Language and market" in `01_BUSINESS.md`, even if the user
   talks to you in another language.

## Ask only what is missing

Ask at most 3 short questions, all in one message, and only for what the request and the files do not answer.

1. Which type? (a) welcome sequence after a lead magnet download (default), (b) nurture or newsletter emails,
   (c) re-engagement for an old list.
2. Then the one detail that type needs:
   - Welcome: which lead magnet, and what is the download link? Check "Other offers" in `04_OFFER.md` and
     `output/lead-magnets/` first. If no lead magnet exists, offer to run `/lead-magnet` first, or continue
     with a placeholder.
   - Nurture: how many and how often? (a) 4 emails, one a week (default), (b) 8 emails, one a week,
     (c) 8 emails, twice a week.
   - Re-engagement: how long since this list got an email, and will people who never click really be removed
     at the end? (a) yes, remove them, (b) no, keep them.
3. Who signs the emails? (a) the founder, give the name, (b) someone else, give the name, (c) the company name.
   If you already used up your questions, write `[SENDER NAME]` and list it as a placeholder.

## Core principles

- **One idea per email.** One story, one lesson or one point. If you have two good ideas, you have two emails.
- **Every email has one job.** Write the job down before you write the email (deliver, teach, prove, answer an
  objection, invite). Everything in the email serves that job and ends in one call to action. The link may
  appear twice, but it always goes to the same place.
- **Give before you ask.** The first emails are pure help. The main offer comes after the reader has gotten
  something useful, and the ask grows step by step through the sequence.
- **Look like a person wrote it.** Plain text, a real name in the From field, no heavy design, no stack of
  images, signed by a person. It should read like an email from someone the reader knows.
- **Subject lines make opening easy.** Clear, short (under 50 characters so it fits on a phone), and paid off in
  the first lines of the body. No clickbait the email does not deliver on, no ALL CAPS, no "Re:" tricks. The
  preview text adds to the subject line and never repeats it.
- **Short paragraphs.** One to three sentences each, with white space between. Most people read on a phone.
- **Use the business's own material.** Stories come from "Origin story" and "Best customer ever", pains and
  phrases from the "Language bank", results only from `05_PROOF.md`. Specific details make an email feel real.
- **Invite replies.** Ask one simple question in the first email. Replies tell you what readers care about and
  tend to help your emails land in the inbox.
- **No fake urgency.** A deadline, a price change or "last chance" only appears if it is real and written in
  `04_OFFER.md` or given by the user.
- **Respect consent.** Only email people who agreed to hear from the business. Every email needs a working
  unsubscribe link and the sender details your market requires, which your email tool usually adds. If the user
  mentions a bought or scraped list, stop and tell them not to send to it.

## Steps

1. Run "Before you start", ask the missing questions in one message, and wait for the answers.
2. Plan the sequence and write the overview table first. Use these defaults unless the user asks otherwise:
   - **Welcome, 5 emails over 7 days.** Day 0 right after signup: deliver the freebie, say where to start in it
     and what the next emails bring, ask one reply question. Day 1: one quick win from the freebie they can do
     today. Day 3: a story from "Origin story" or "Best customer ever" showing why "What they have tried" fails,
     with a soft mention of the main offer. Day 5: one result from `05_PROOF.md` and the biggest objection from
     "What holds them back", answered. Day 7: a clear invitation to the main call to action, what happens after
     they click (step 1 of "Customer journey"), and the guarantee only if `04_OFFER.md` has one.
   - **Nurture or newsletter.** Each email takes a different idea type: a pain from the language bank and what
     to do about it, a common belief that is wrong (Contrarian), a customer story from `05_PROOF.md`, one how to
     step, a behind the scenes look, an objection answered. Each ends with the main call to action in one calm
     sentence, or with a reply question if the user wants pure value emails.
   - **Re-engagement, 3 emails over 7 days.** Day 0: an honest check in that admits the silence, plus the most
     useful thing the business has (the lead magnet or a strong tip), and a click to stay subscribed. Day 3: the
     best value email you can write, ending with the main call to action. Day 7: a short last email. Say people
     who do not click will be removed only if the user confirmed they will be.
3. For each email, pick the material before writing: which pain, story, quote or proof item it uses, and note
   the proof item with the section it comes from.
4. Write each email: 3 subject lines with different angles (for example Curiosity, Benefit, Pain, Story, Proof,
   Direct, Contrarian), preview text of 35 to 90 characters, the body, one call to action, and a P.S. only if it
   adds something (restating the call to action or a small extra detail). Keep most bodies at 100 to 250 words
   and the delivery email under 120 words.
5. Set the timing. Days count from the trigger (signup, or the first send for nurture and re-engagement). Send
   the delivery email immediately. For the rest, suggest a time that fits the audience in `02_AUDIENCE.md`, such
   as early morning for business owners or evening for people who work daytime jobs, and call it a starting
   point to test.
6. Read the whole sequence in order. Each email must make sense on its own, because people miss emails, and
   together they must build toward the call to action without repeating the same story or proof.
7. Run the quality check below and fix every failure.
8. Save the file and hand off.

## Output format

Use this template. Repeat the email block for every email, and delete the instruction text in brackets.

```markdown
# Emails: [sequence name]

Date: YYYY-MM-DD
Type: [Welcome | Nurture | Re-engagement]
Who gets it: [the trigger, for example "downloaded [lead magnet name]"]
Main call to action: "[exact wording from 04_OFFER.md]" [link]
Sender: [name shown in the From field]
Language: [from 01_BUSINESS.md]

## Sequence overview

| # | Send | Job of this email | Call to action |
|---|---|---|---|
| 1 | Day 0, right after signup | Deliver the freebie | Open the download |
| 2 | Day 1, [time] | [job] | [call to action] |

## Email 1: [short name]

Send: Day [n], [suggested time, reader's time zone]
Subject lines:
1. (Curiosity) [subject]
2. (Benefit) [subject]
3. (Direct) [subject]
Preview text: [text]

Body:

[greeting]

[short paragraphs, one idea]

[call to action line with link]

[sign off]
[sender name]

P.S. [optional]

Proof used: [05_PROOF.md > section > item, or none]

## Open placeholders
- [LINK: download link for the lead magnet]

## Setup notes
- Paste each email as plain text and set the delays in your email tool.
- Check that the unsubscribe link and sender details are switched on.
```

## Quality check

Run every item in `.claude/skills/review/CHECKLIST.md` on the whole sequence and fix what fails. Sections 1 and
2 are blocking, so never save emails that fail them. Then check these email specific points:

- Each email has one idea, one job and one call to action. In a welcome sequence, emails 1 and 2 may use a
  small action (open the freebie, reply). From email 3 on, use the main call to action from `04_OFFER.md`,
  worded the same way every time.
- Each email's 3 subject lines use 3 different angles, and the opening lines pay off every one of them.
- Preview text adds something new and is not a copy of the subject line.
- No deadline, removal warning or "last chance" appears unless it is real.

## Save

Save to `output/emails/YYYY-MM-DD_slug.md`, using today's date and a slug of 2 to 5 lowercase words joined by
hyphens that names the type and the topic, for example `output/emails/2026-03-14_welcome-job-profit-checklist.md`.
If that file already exists, add `-v2` (or the next number) instead of overwriting it.

## Hand-off

Tell the user, in a few short lines:

- The file path, the type, and the plan in one line (for example "5 emails, Day 0 to Day 7").
- Every open placeholder, such as `[LINK: ...]`, `[SENDER NAME]` or `[ADD PROOF: ...]`, and which business
  file or link would fill it.
- Any business file that was still `status: draft`.
- Setup reminders: plain text, the delays from the overview table, unsubscribe link on, and for an old list,
  send to a small part of it first and remove bounced addresses before sending to the rest.
- What to run next: `/lead-magnet` if the freebie does not exist yet, `/landing-page` for the opt-in page,
  `/ads` to bring people to that page, `/content` to turn nurture emails into posts, and `/review` for a
  second check after the user edits anything.

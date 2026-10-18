---
name: content
description: Plans and writes organic social content for the business. By default it produces a 30 day content plan (pillars, posting days, format and hook for every post) plus 7 ready-to-record short form video scripts for Reels, TikTok and Shorts, each with a caption. On request it writes LinkedIn or Instagram posts, outlines a carousel, or turns one long video transcript into many pieces. Use it when the user wants organic content, a posting schedule, video ideas or captions. Triggers include "content plan", "content calendar", "what should I post", "short form scripts", "Reels", "TikTok", "Shorts", "video ideas", "captions", "LinkedIn post", "Instagram post", "carousel", "repurpose this video" and "turn this transcript into posts".
---

# Content

Produces organic content that builds trust with the dream customer and moves them toward the lead magnet and the main offer. Default deliverable: a 30 day plan plus 7 short form scripts with captions.

## Before you start

1. Open every file in `business/` and read the `status:` line in its frontmatter. If any file says `status: empty`, stop and tell the user: "Your business files are not set up yet. Type `/setup` first, then run `/content` again." Write nothing else.
2. If a file says `status: draft`, continue, and mention in the hand-off that the content rests on unconfirmed facts.
3. Read these business files:
   - `business/01_BUSINESS.md`: "What makes us different", "Origin story", and "Language and market" (the language of every deliverable).
   - `business/02_AUDIENCE.md`: all of it, especially "Dream customer" (awareness level), "Pains", "Dream outcome", "What holds them back" and "Language bank".
   - `business/03_VOICE.md`: "Tone", "How we address the reader", "Words we use", "Words we never use", "Writing samples".
   - `business/04_OFFER.md`: "Main offer", "Other offers" (look for a free offer), "Main call to action".
   - `business/05_PROOF.md`: all of it. It is the only source of results, numbers and client stories.
   - `business/06_RULES.md`: all of it. It wins over everything else.
4. Read these knowledge files if they exist. If one is missing, skip it and rely on the core principles below.
   - `knowledge/Content_Engine.md`
   - `knowledge/Hooks_And_Headlines.md`
   - `knowledge/Messaging_Psychology.md`
5. Look in `output/lead-magnets/` for a finished lead magnet to promote, and in `output/content/` for earlier plans. Do not reuse hooks from a plan made in the last 30 days.

## Ask only what is missing

Ask at most 3 questions, all in one message, and only for what the request and the business files do not answer. If nothing is missing, skip this step.

1. "Where do you post? (a) Instagram Reels, (b) TikTok, (c) YouTube Shorts, (d) LinkedIn, (e) several of these"
2. "How many days a week can you post and keep it up for a month? (a) 3, (b) 5, (c) every day"
3. "Who is on camera? (a) the founder, (b) someone on the team, (c) nobody, voice over with screen or b-roll"

Do not ask which mode. Use the default unless the request names posts, a carousel or a transcript. In repurpose mode, if no transcript was pasted, ask for it and wait. If there is no free offer, do not ask about one: the ask posts point to the main call to action and the hand-off suggests `/lead-magnet`.

## Core principles

- The first 3 seconds decide reach. The on-screen text and the first spoken line name a specific pain, result or surprise for this audience. Never open with a greeting, a name, or "in this video".
- Show, do not claim. A demo, a real example, a screen recording, a before and after, or a look behind the scenes beats any adjective. If it cannot be shown or proven, cut it.
- One idea per piece. Each post makes one point and stops. A second point is a second post.
- Use the audience's own words. Build hooks from the "Language bank" in `02_AUDIENCE.md`. A real customer phrase beats a clever line.
- Give much more than you ask. About 4 in 5 posts teach, show or tell a story and ask for nothing beyond a follow. About 1 in 5 asks for something: comment a keyword for the lead magnet, or the main call to action. Never two ask posts in a row.
- Every pillar connects a pain from "Pains" to something the main offer solves. Content that entertains people who will never buy is wasted effort.
- Consistency beats volume. A plan the user can keep for 30 days beats an ambitious one they drop in week two. Posting days follow the capacity they gave.
- Repurpose winners. One strong idea can become a video, a carousel and a text post. Leave room in weeks 3 and 4 to remake the two best performers from weeks 1 and 2.
- The caption adds a new angle. It never repeats the video. It adds a detail, the story behind the point, or a question for the comments, then repeats the ask.
- Match awareness. Unaware and problem aware audiences need the problem named before any solution. Product aware audiences need proof and the offer.
- No claims beyond `05_PROOF.md`. Results, client stories and numbers come only from that file. Where a post needs proof that does not exist, write `[ADD PROOF: what is needed]`.

## Steps

1. Pick the mode from the request: default plan, posts, carousel or repurpose.
2. Define 3 to 4 content pillars. For each, write the pain or goal from `02_AUDIENCE.md` it speaks to and how it leads to the main offer.
3. Set the ask. If "Other offers" in `04_OFFER.md` or `output/lead-magnets/` has a free offer, choose one short comment keyword in the deliverable language. Otherwise the ask is the main call to action, worded exactly as in `04_OFFER.md`.
4. Build the 30 day calendar. Spread the posting days to match the user's capacity. Give every post a pillar, a format (Short video, Carousel, Text post, Image post, Story) and a hook. Tag each post Value, Follow, Lead magnet or Main CTA. Count the posts, make about one in five an ask, and rotate the pillars.
5. Pick the 7 strongest short video ideas from the calendar and write a full script for each with the template below. Keep each 20 to 60 seconds. At about 2.5 spoken words per second, that is 50 to 150 spoken words.
6. Label the main hook with its angle, then write 2 alternative hooks with different angles (Pain, Outcome, Curiosity, Proof, Contrarian, Identity, Mistake, Story). No more than two of the three hooks share an angle.
7. Write a caption for each script that adds a new angle and ends with the ask.
8. For posts, carousel or repurpose mode, use the matching template under "Output format" instead of steps 4 to 7.
9. Run the quality check, fix every failure, then save.

Repurpose mode: read the whole transcript and list every idea that stands on its own (a story, a mistake, a how-to step, a strong opinion, a quotable line). Keep the speaker's own words where they work. Note timestamps if the transcript has them.

## Output format

Template headings stay in English so other skills can find the sections. Everything the audience will read is written in the language from "Language and market".

```markdown
---
type: content
mode: 30-day-plan
date: YYYY-MM-DD
platforms: [from the user]
language: [from 01_BUSINESS.md]
---

# Content plan: [start date] to [end date]

## Pillars
| # | Pillar | Pain or goal it speaks to | How it leads to the offer |
|---|---|---|---|

## The ask
Lead magnet keyword: [WORD] for [lead magnet name], or "none yet"
Main call to action: [exactly as in 04_OFFER.md]

## 30 day calendar
| Day | Date | Pillar | Format | Hook | Ask |
|---|---|---|---|---|---|

## Short form scripts

### Script 1: [working title]
Pillar: [name] | Length: [20 to 60] seconds | Ask: [Value, Follow, Lead magnet or Main CTA]

On-screen text (0 to 3 s): [8 words or fewer]
Spoken hook ([Angle]): [one sentence]

| Beat | Spoken | On screen |
|---|---|---|
| 1 | [line] | [what to show] |
(3 to 5 beats)

Call to action: [spoken line, for example "Comment WORD and I will send you the checklist"]

Alternative hooks:
1. [Angle]: [hook]
2. [Angle]: [hook]

Caption:
[2 to 6 short lines with a new angle, then the ask]

(Scripts 2 to 7 follow the same layout.)

## Open placeholders
- [every bracket left in the file]
```

Posts mode: for each post, write the hook with its angle, the body (LinkedIn up to about 200 words, Instagram up to about 120), the ask, and 2 alternative hooks with angle labels. Deliver 3 to 5 posts unless the user asked for a number.

Carousel mode: slide 1 is the hook (8 words or fewer). Slides 2 to 8 carry one point each, with the slide text and a note on the visual. The last slide holds the ask. Add 2 alternative cover hooks with angle labels and a caption.

Repurpose mode: 5 short video clips (start and end timestamp, on-screen text, hook, why it works alone), 3 text posts, 1 carousel outline and a caption for each clip, all in the formats above.

## Quality check

Run `.claude/skills/review/CHECKLIST.md` on everything in the file and fix every failure before saving. Never save with a failure in section 1 (Truth) or section 2 (Rules). Then check these content specifics:

- Every script runs 20 to 60 seconds when read aloud at a normal pace.
- On-screen opening text is 8 words or fewer and makes sense with the sound off.
- About 1 in 5 posts asks for something, and no two ask posts are back to back.
- No caption repeats the first line of its video.
- Every hook could only be about this business and this audience. If a competitor could post it unchanged, rewrite it.
- The comment keyword is the same everywhere it appears.

## Save

Save to `output/content/YYYY-MM-DD_slug.md`, using today's date and a short slug that names the job, for example `30-day-plan`, `linkedin-posts-pricing`, `carousel-first-hire` or `repurpose-webinar`. If the file already exists, add `-2` to the slug.

## Hand-off

Tell the user, in the language they wrote in:

1. The file path.
2. What is inside: the pillars, the posting days, the number of posts, and the comment keyword if there is one.
3. Every open placeholder, as a list, with what is needed to fill it.
4. A practical note: replies to keyword comments are sent by hand or with a DM automation tool, and the follow-up should go out the same day.
5. If any business file was `status: draft`, say which, and that the content should be checked once it is confirmed.
6. What to run next:
   - `/lead-magnet` if there is no free offer yet, so the ask posts have something to give away.
   - `/email` to write the sequence that follows up the people who comment the keyword.
   - `/ads` after two weeks of posting, to turn the best performing videos into ads.
   - `/review` on any post edited by hand before it goes out.

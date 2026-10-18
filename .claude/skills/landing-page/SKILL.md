---
name: landing-page
description: "Writes and builds a landing page for the business. Delivers the copy as a markdown file with 3 to 5 labeled headline variants at the top, plus the finished page as one self-contained HTML file that opens in any browser and can be published without code. Handles three page types, a booking or sales page that sends visitors to the main call to action (the default), an opt-in page for a lead magnet, and a simple one-page website for a service business. Use when the user asks for a landing page, sales page, booking page, opt-in page, squeeze page, signup page, lead capture page, one-page website or homepage, or wants to turn the offer into a page they can publish."
---

# Landing page

Produces the copy for one landing page (markdown) and the built page (one HTML file), both saved in `output/pages/`.

## Before you start

1. Open every file in `business/` and read the `status:` line in its frontmatter. If any file says `status: empty`, stop. Tell the user: "The business files are not filled in yet. Type `/setup` first, then ask for the page again." Do not write anything.
2. If a file says `status: draft`, continue, and name the draft files in the hand-off.
3. Read these business files in full:
   - `business/01_BUSINESS.md`: "Company", "What we sell", "Positioning", "Origin story", "What makes us different", "Language and market"
   - `business/02_AUDIENCE.md`: "Dream customer" (for the awareness level), "Pains", "Dream outcome", "What they have tried", "What holds them back", "Language bank", "Best customer ever"
   - `business/03_VOICE.md`: every section, especially "How we address the reader", "Words we never use", "Writing samples" and "Brand look"
   - `business/04_OFFER.md`: "Main offer", "Price", "Guarantee", "Other offers", "Customer journey", "Main call to action"
   - `business/05_PROOF.md`: every section. This is the only allowed source of proof.
   - `business/06_RULES.md`: every section. These rules win over this skill.
4. Read these knowledge files if they exist. Skip any that are missing, the principles below are enough.
   - `knowledge/Hooks_And_Headlines.md` (headline variants)
   - `knowledge/Messaging_Psychology.md` (problem, outcome and objection sections)
   - `knowledge/Lead_Magnets.md` (opt-in pages only)
5. For an opt-in page, look for the lead magnet in `output/lead-magnets/` and under "Other offers" in `04_OFFER.md`.
6. Read `.claude/skills/review/CHECKLIST.md` now, so you write to it instead of fixing afterwards.

## Ask only what is missing

Page type: if the user does not name one, build (b) a booking or sales page and say so in one line. Do not ask.

Then ask at most 3 short questions in one message, and only for things the request and the business files do not answer. If nothing is missing, skip this step.

1. Where will most visitors come from? (a) cold ads, people who do not know you yet (b) your email list, followers or referrals (c) not sure, use the awareness level in `02_AUDIENCE.md`
2. Opt-in page only, if no lead magnet is found: Which free resource is this page for? (a) one you already have, tell me its name and what is in it (b) none yet, run `/lead-magnet` first (c) write the page now with a placeholder name
3. Only if "Main call to action" in `04_OFFER.md` has no link, or for an opt-in page: (a) here is the link or the form embed code (b) build it now, I will add it later

## Core principles

- **One page, one job.** Every button uses the same text and the same link from "Main call to action" in `04_OFFER.md`. No menu and no links that lead away. Only the one-page website gets a short menu, and it links to sections on the same page.
- **The top of the page answers three things on a phone screen:** what this is, who it is for, and what to do next. The first button is visible without scrolling.
- **Headline test.** It names this audience's problem or outcome in concrete terms. If a competitor could put it on their page unchanged, rewrite it.
- **Length follows awareness and price.** Cold or problem aware readers and higher prices need the problem, proof and objections before the ask. Most aware readers need the offer, price and button near the top. Opt-in pages stay short, one to two phone screens.
- **Open with their problem, not your company.** Use wording from the "Language bank" so the reader recognizes their own situation. Talk about the business only after the reader feels understood.
- **Every included item earns a "so you can".** List what the offer contains, and next to each item say what it changes for the reader.
- **Proof sits next to the claim it supports** and comes only from `05_PROOF.md`. Use a person's name only if the file says permission is yes. Language bank quotes shape the wording, they are never shown as testimonials.
- **Answer the biggest fear before the button.** Take objections and inertia from "What holds them back" and answer them with facts from `04_OFFER.md`. If the files do not hold the answer, write `[ANSWER NEEDED: ...]` instead of inventing a policy.
- **Lower the risk honestly.** Quote the guarantee word for word if one exists. If "Guarantee" says None, leave it out and never hint at "risk free". Instead, explain plainly what happens after the click, using the customer journey.
- **The button says what they get,** in the words of the main call to action. Never "Submit", "Learn more" or "Click here".
- **Mobile first and fast.** Single column, short paragraphs, large text and tap targets, no heavy images, no scripts.

## Steps

1. Run "Before you start" and "Ask only what is missing".
2. Settle the brief in four lines for yourself: page type, awareness level, the reader's main pain in their words, and the one call to action with its link.
3. Collect the raw material: the language bank quotes you will use, every proof item that fits, the included items and price from `04_OFFER.md`, the customer journey steps, the top objections, and the guarantee text (or None).
4. Write 3 to 5 headline variants, each with a subheadline and a labeled angle (Pain, Outcome, Proof, Curiosity, Contrarian, Identity). No more than two share an angle. Use a Proof headline only if `05_PROOF.md` has a result to put in it. Pick one and write one sentence on why it fits this awareness level.
5. Write the page copy in the language from "Language and market", section by section, in this order:
   - **(b) Booking or sales page:** hero (headline, subheadline, button), the problem in their words, what changes, the offer and what is included (show the price only if "Price" says it is shown publicly), proof, how it works (3 to 5 steps from "Customer journey", step one is the call to action), FAQ built from the objections, guarantee (only if one exists), final call to action.
   - **(a) Opt-in page:** hero that names the free resource and the result it gives, 3 to 5 bullets on what is inside, the form, one proof item if one fits, a short "this is for you if" list, and one line on what arrives and when.
   - **(c) One-page website:** header with the company name and an in-page menu, hero, who it is for and who it is not for (from "Positioning"), services (from "What we sell"), what makes us different, proof, how it works, the origin story, FAQ, final call to action, footer with the company name and contact details or `[ADD: contact details]`.
6. Place a button after the hero, after the offer or services, after the proof and at the end. On long pages, add one after the FAQ.
7. Run the checklist on the copy and fix every failure (see "Quality check").
8. Build the HTML file from the final copy, following the HTML rules in "Output format". The text on the page must match the markdown copy exactly.
9. Check the HTML before saving: the `<style>` block is complete with every rule closed, every call to action uses the exact link, every placeholder shows on the page, there are no external scripts, and no element has a fixed width wider than a phone.
10. Save both files (see "Save"), then open the HTML in the default browser:
    - macOS: `open "output/pages/YYYY-MM-DD_slug.html"`
    - Windows (PowerShell): `Start-Process "output\pages\YYYY-MM-DD_slug.html"`
    - Linux: `xdg-open "output/pages/YYYY-MM-DD_slug.html"`

    If the command fails, give the user the path to open by hand.

## Output format

### The copy file (markdown)

```markdown
---
type: landing-page
page_type: booking | opt-in | website
date: YYYY-MM-DD
language: [from "Language and market"]
call_to_action: "[button text]" links to [link]
built_page: output/pages/YYYY-MM-DD_slug.html
---

# [Page name]

## Headline variants

1. [Angle]: [Headline]
   Subheadline: [Subheadline]
2. [Angle]: [Headline]
   Subheadline: [Subheadline]
3. [Angle]: [Headline]
   Subheadline: [Subheadline]

Chosen: [number], because [one sentence on why it fits the awareness level].

## Page copy

### Hero
Headline: [chosen headline]
Subheadline: [chosen subheadline]
Button: [call to action text]

### [Section name]
[Copy]

[One block per section, in the order from step 5. Write every button as "Button: [text]".]

## Open placeholders

- [ADD PROOF: ...] in [section]
- [ADD LINK: ...] in [section]

## Notes

- Written for awareness level: [level]
- Colors and fonts: [from "Brand look" in 03_VOICE.md, or neutral fallback because "Brand look" was empty]
```

### The built page (HTML)

One file, no build step, opens with a double click.

- Starts with `<!DOCTYPE html>` and `<html lang="...">` set to the business language. Includes `<meta charset="utf-8">`, the viewport meta tag, a `<title>` and a `<meta name="description">` written from the copy.
- All CSS sits in one `<style>` tag in the `<head>`. No CSS or JavaScript frameworks and no external scripts. The FAQ uses `<details>` and `<summary>`, which need no script.
- Colors and fonts come from the "Brand look" table in `03_VOICE.md`, set once as CSS variables at the top of the style block (`--primary`, `--accent`, `--bg`, `--text`, `--heading-font`, `--body-font`). Values still in square brackets count as empty. If the table is empty, use a neutral palette (background #FFFFFF, text #1A1A1A, primary #1F2937, accent #2563EB, system font stack) and tell the user.
- A Google Fonts `<link>` is allowed for fonts named in "Brand look". Otherwise use the system font stack. No other external files except the logo.
- Mobile first: base styles for phones, `min-width` media queries for larger screens. Body text at least 17px with a line height around 1.6, text columns no wider than about 680px, buttons at least 48px tall and full width on phones.
- Contrast: body text and button text reach at least 4.5 to 1 against their background. If a brand color is too light for white text, put dark text on it or use a darker shade, and say so.
- Every call to action is `<a class="button" href="[link from 04_OFFER.md]">` with the same text. If there is no link yet, use `href="#ADD-CTA-LINK"` and list it as a placeholder.
- No stock photos. Use the image at "Logo URL" if there is one, otherwise the company name as text. Where an image would help, use a box with a dashed border and a label such as `[IMAGE: photo of the owner at work]`. Simple CSS shapes and color blocks are fine for decoration.
- Placeholders cannot be missed: wrap each one in an element with `class="placeholder"`, styled with a bright yellow background, a dashed red border and bold text. Right after `<head>`, add an HTML comment that lists every open placeholder.
- Semantic structure: one `<h1>`, an `<h2>` per section, `<header>`, `<main>`, `<section>` and `<footer>`, alt text on every image.
- Put `<!-- Paste your analytics or ad pixel code here -->` just before `</head>`.
- Opt-in pages: a simple form with a labeled email field, an optional first name field, and a submit button with the call to action text. Put this comment directly above the form:
  `<!-- To connect this form: in your email tool, create a signup form and copy its embed code or its form action URL. Either replace this whole <form> with the embed code, or paste the action URL into action="" and change each name="" to the field names your tool uses. Test it with your own email address before you publish. -->`
  Add a privacy policy link in the footer, or `[ADD LINK: privacy policy]`.

## Quality check

Run every section of `.claude/skills/review/CHECKLIST.md` on the copy, then these page checks:

- Every button has identical text and the identical link.
- The text in the HTML matches the markdown copy word for word.
- No number, result or name appears that is not in `05_PROOF.md`, including in the headline variants you did not choose.
- The price, if shown, is written exactly as in `04_OFFER.md` and follows "Always do" in `06_RULES.md`.
- Every placeholder is in square brackets, styled as a placeholder in the HTML, and listed under "Open placeholders".

Fix every failure. Do not save copy that fails section 1 or 2 of the checklist.

## Save

- Copy: `output/pages/YYYY-MM-DD_slug.md`
- Built page: `output/pages/YYYY-MM-DD_slug.html`

Use today's date and a short lowercase slug with hyphens that names the page, for example `booking-page` or `checklist-optin`. Both files share the same name. If a file with that name already exists, add `-2` to the slug instead of overwriting.

## Hand-off

Tell the user, in short lines:

1. Both file paths, and that the page is open in their browser.
2. The chosen headline and its angle, and that the other variants are at the top of the markdown file.
3. Every open placeholder and what is needed to fill it. For missing proof, offer to add real results to `business/05_PROOF.md` once they have them.
4. Whether the colors and fonts came from "Brand look" or the neutral fallback, and any contrast adjustment you made.
5. What to connect before going live: the call to action link, the form on opt-in pages, and their analytics or pixel code.
6. How to publish without code:
   - Netlify Drop: put the file in an empty folder, rename it `index.html`, and drag the folder onto app.netlify.com/drop. It gives a live link right away. A free account keeps the site online and lets them connect their own domain.
   - Website builder: add an HTML or custom code block and paste the whole file. If the builder only accepts body content, paste the `<style>` block plus everything inside `<body>`, and put the font link in the site's header settings.
7. What to run next: `/ads` to send traffic to the page, `/email` for the follow-up (a nurture sequence after an opt-in, reminders and follow-up after a booking), or `/review` for a second, stricter read. If an opt-in page has no lead magnet yet, run `/lead-magnet` first.

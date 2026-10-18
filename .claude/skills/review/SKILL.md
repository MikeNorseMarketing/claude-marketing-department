---
name: review
description: "Runs a strict quality check on any piece of marketing copy before it goes out, whether it is an ad, a landing page, an email, a social post or video script, or a lead magnet. Writes a report with a clear verdict, every blocking problem quoted with a fixed version, notes on voice and selling, and the three changes that would help most. Checks every claim against the business files and flags any number, result or name that cannot be traced to the proof file, even when it sounds plausible. Use when the user says review, check this, quality check, proofread, is this ready, can I publish this, before I send this, audit this copy, look over the latest, or wants a second opinion on copy they wrote or another skill produced."
---

# Review

Produces a review report with a verdict ("Ready" or "Fix before using") and, if the user approves, a fixed copy saved as a new `-v2` file.

## Before you start

1. Open every file in `business/` and read the `status:` line in its frontmatter. If any file says `status: empty`, stop. Tell the user: "The business files are not set up yet, so there is nothing to check the copy against. Type `/setup` first." Do not review anything.
2. If a file says `status: draft`, continue, and say in the report that checks against draft files are less certain.
3. Read these files:
   - `.claude/skills/review/CHECKLIST.md`: the list you run, every section and every item.
   - `business/01_BUSINESS.md`: "Language and market", "Positioning", "What makes us different"
   - `business/02_AUDIENCE.md`: "Dream customer" (for the awareness level), "Pains", "What holds them back", "Language bank"
   - `business/03_VOICE.md`: "Tone", "How we address the reader", "Words we use", "Words we never use", "Writing samples"
   - `business/04_OFFER.md`: "Main offer", "Price", "Guarantee", "Customer journey", "Main call to action"
   - `business/05_PROOF.md`: every section. Every claim is checked against this file.
   - `business/06_RULES.md`: every section, and the "Never say" list word by word.
4. Read the knowledge file that fits the type, if it exists. Skip any that are missing, the checklist and the principles below are enough.
   - Ad: `knowledge/Hooks_And_Headlines.md` and `knowledge/Ad_Scripting.md`
   - Landing page: `knowledge/Hooks_And_Headlines.md` and `knowledge/Messaging_Psychology.md`
   - Email: `knowledge/Lead_Nurture.md`
   - Content: `knowledge/Content_Engine.md`
   - Lead magnet: `knowledge/Lead_Magnets.md`

## Ask only what is missing

Ask at most 3 short questions in one message, and only for what the request does not answer. If nothing is missing, skip this step.

1. If no input was given: What should I review? (a) the latest file in `output/` (b) a file path (c) paste the text here
2. If the type is unclear: What is it? (a) ad (b) landing page (c) email (d) social post or video script (e) lead magnet
3. Ads and posts only, if unclear: Where will it run? (a) paid ads (b) organic social (c) both

## Core principles

- **Strict on numbers.** Every number, percentage, time frame, count, price, review score, client name and result must trace to `05_PROOF.md`, and prices to `04_OFFER.md`. Sounding plausible is not enough. A real number that was rounded up, combined, extrapolated or turned into "about" fails too. So do vague volume claims like "hundreds of clients" or "most of our customers" when the file has no matching number.
- **Implied promises count.** Wording that states an outcome as certain ("you will", "get X in 30 days") is a promise. A guarantee worded even slightly stronger than in `04_OFFER.md` fails.
- **Quote, do not describe.** Every issue quotes the exact words, so the user can find them with search.
- **Every blocking issue gets a fix.** The fixed version is ready to paste, in the business's language and voice, and passes the checklist itself. If the fix needs proof that does not exist, it uses `[ADD PROOF: ...]`.
- **The verdict is binary.** "Ready" only when sections 1 and 2 pass and no placeholder is left. Anything else is "Fix before using". Voice and selling issues alone do not block, but they are listed.
- **Judge against this business, not your own taste.** Compare the voice with "Tone" and "Writing samples" in `03_VOICE.md`. Do not rewrite a style that matches the samples just because you would write it differently.
- **Prioritize.** Group a repeated problem into one note with every location ("em dash used 6 times, in lines 3, 8 and 14 ..."). End with the 3 changes that would help most, ranked by risk first, then by effect on response.
- **Read everything that ships.** Subject lines, preview text, buttons, form labels, text in images, captions, alt text, link targets and unused headline variants are all part of the copy.
- **Never touch the original.** Fixes go in a new `-v2` file, and only after the user says yes.

## Steps

1. Find the input.
   - A file path: read the file.
   - Pasted text: use it exactly as given.
   - "The latest": find the newest file in `output/`, skipping review reports, and tell the user which file you picked.
     - macOS or Linux: `find output -type f \( -name "*.md" -o -name "*.html" \) ! -name "*-review.md" -exec ls -t {} + | head -n 1`
     - Windows (PowerShell): `Get-ChildItem output -Recurse -File -Include *.md,*.html | Where-Object { $_.Name -notlike "*-review.md" } | Sort-Object LastWriteTime -Descending | Select-Object -First 1 -ExpandProperty FullName`
   - A landing page has two files with the same name. Review the `.md` copy, and open the `.html` too, to check the links, that placeholders are visible, and that its text matches the copy.
2. Detect the type from the folder (`output/ads/`, `output/pages/`, `output/emails/`, `output/content/`, `output/lead-magnets/`) or from the content. If it is still unclear, ask question 2.
3. Build a claims list. Go through the text line by line and list every number, name, quote, result, review score, time frame, price, guarantee-like phrase, superlative ("the best", "the only", "the fastest") and claim about competitors or the market. For each one, find the line in `05_PROOF.md` or `04_OFFER.md` that supports it, or mark it "not found".
4. Run checklist section 1 (Truth) and section 2 (Rules) using the claims list and `06_RULES.md`. Every failure becomes a blocking issue.
5. Run sections 3 (Voice), 4 (Sounds human), 5 (Selling) and 6 (Delivery), plus the checks for the type:
   - Ad: the hook works in the first line or the first 3 seconds, no personal attribute call-out, 3 to 5 labeled variants, and the ad matches the page it sends people to if that page is in `output/pages/`.
   - Landing page: the top answers what it is, who it is for and what to do next, one call to action with the right link everywhere, the biggest objection answered, a guarantee only if one exists.
   - Email: subject line and preview text are specific and honest (no fake "Re:", no false urgency), one call to action per email, it reads like one person writing to one person.
   - Content: the first line earns the second, it fits the platform, the call to action is soft and points to the real offer.
   - Lead magnet: it gives one quick, real win, it fits the problem the main offer solves, and it leads naturally to the main call to action.
6. Write a fixed version for every blocking issue. Then run sections 1 to 4 of the checklist on your own fixes.
7. Decide the verdict, write the report in the format below, and save it.
8. Show the user the verdict, the blocking issues and the top 3 changes, then ask: "Do you want me to apply these fixes? I will save them as a new file and leave the original as it is."
9. If the user says yes, write the full fixed version and save it as a new file with `-v2` in the name (`-v3` if a `-v2` already exists). For a landing page, save both the `.md` and the `.html` as `-v2`. Run the checklist on the new version and tell the user what still needs them, such as open placeholders.

## Output format

Write the report in the language set in "Language and market". Quotes stay word for word as they appear in the copy.

```markdown
# Review: [file name, or "pasted text"]

Date: YYYY-MM-DD
Reviewed: [path, or "pasted text"]
Type: [ad | landing page | email | content | lead magnet]
Business files: [all confirmed | drafts: list them]

## Verdict: [Ready | Fix before using]

[One or two sentences on why.]

## Blocking issues

### 1. [Short name] (Truth | Rules)
- Quote: "[exact words from the copy]"
- Why it fails: [the checklist item or rule, and what is wrong]
- Fixed version: "[ready to paste]"

[One block per issue. If there are none, write "None."]

## Open placeholders

- [placeholder] in [where]

## Claims check

| Claim in the copy | Source | Status |
|---|---|---|
| "[claim]" | 05_PROOF.md, [section] | Traced |
| "[claim]" | not found | Flagged |

## Voice and sounds human

- "[quote]". Problem: [what is wrong]. Try: "[rewrite]"

## Selling

- [Notes on the headline or hook, benefits, awareness match, call to action, objection handling and variants]

## The 3 changes that would improve it most

1. [The change, and why it matters]
2. [The change, and why it matters]
3. [The change, and why it matters]

## Checklist result

| Section | Result |
|---|---|
| 1. Truth | [Pass, or Fail with the number of issues] |
| 2. Rules | [Pass, or Fail with the number of issues] |
| 3. Voice | [Pass, or notes] |
| 4. Sounds human | [Pass, or notes] |
| 5. Selling | [Pass, or notes] |
| 6. Delivery | [Pass, or notes] |
```

## Quality check

Run sections 1 to 4 of `.claude/skills/review/CHECKLIST.md` on every fixed version in the report and rewrite any that fail. A fix that invents a number or adds a dash is worse than no fix. Then confirm:

- Every blocking issue has a quote, a reason and a fixed version.
- Every claim from step 3 is in the claims table, and nothing marked "Traced" is missing from `05_PROOF.md` or `04_OFFER.md`.
- The verdict follows the rule: "Ready" only with zero blocking issues and zero open placeholders.

## Save

- A reviewed file: save the report next to it as `<same name>-review.md`. For example, `output/ads/YYYY-MM-DD_spring-ads.md` gets `output/ads/YYYY-MM-DD_spring-ads-review.md`. For a landing page, use the name without the extension.
- Pasted text: `output/YYYY-MM-DD_short-name-review.md` with today's date, for example `output/YYYY-MM-DD_welcome-email-review.md`.
- If the report file already exists, add `-2` before `.md` instead of overwriting.
- Fixed versions, only after approval: the same folder and name as the original plus `-v2`, for example `output/ads/YYYY-MM-DD_spring-ads-v2.md`. For pasted text, use the folder for its type, for example `output/emails/YYYY-MM-DD_welcome-email-v2.md`.

## Hand-off

Tell the user, in short lines:

1. The verdict and the number of blocking issues.
2. The path to the report.
3. The 3 changes that would help most, one line each.
4. Open placeholders and what is needed to fill them. If proof is missing, ask whether they have a real result, and offer to add it to `business/05_PROOF.md`. Never change a business file without asking.
5. The offer to apply the fixes as a `-v2` file, or, if they already said yes, the path to the new file.
6. What to do next. If "Ready", publish it or move on to the next piece (a page usually needs `/ads` to bring traffic and `/email` to follow up). If "Fix before using", apply the fixes and run `/review` again on the `-v2` file.

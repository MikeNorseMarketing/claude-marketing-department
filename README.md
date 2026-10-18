# Claude Marketing Department

A free Claude Code setup that works like a small marketing department. Answer questions about your business
once. Then write landing pages, ads, emails, content and lead magnets that sound like you, built on proven
direct response principles.

Made by Mike Haugen at Norse Marketing. Watch the full walkthrough on YouTube:
[youtube.com/@immikehaugen](https://www.youtube.com/@immikehaugen)

## What you need

- A paid Claude plan (Pro or Max). The free plan does not include Claude Code.
- Claude Code. Claude Code installs everything else for you.

## Setup

**1. Open your terminal.**
Mac: press `Cmd` and `Space`, type Terminal, press Enter.
Windows: press the Windows key, type PowerShell, press Enter.

**2. Install Claude Code.** Paste one line:

```bash
# Mac
curl -fsSL https://claude.ai/install.sh | bash
```

```powershell
# Windows (PowerShell)
irm https://claude.ai/install.ps1 | iex
```

When it's done, close the terminal and open a new one.

**3. Start Claude and log in.**

```bash
claude
```

The first time, your browser opens so you can log in with your Claude account.

**4. Let Claude do the rest.** Paste this prompt into Claude Code:

```text
Install Git if I don't have it. Then download github.com/MikeNorseMarketing/claude-marketing-department to my Desktop, and tell me the exact command to open Claude Code in that folder.
```

Claude asks before it runs anything. Say yes. On a Mac you may get a popup to install developer tools,
click Install. On Windows you may be asked for permission, click Yes.

**5. Open the folder and run setup.** Type `/exit`, paste the command Claude gave you, then type:

```text
/setup
```

Setup interviews you about your business (about 20 to 30 minutes) and writes your business files.
You can stop any time and continue later with `/setup continue`.

Already use Git? This does the same thing:

```bash
git clone https://github.com/MikeNorseMarketing/claude-marketing-department.git
cd claude-marketing-department
claude
```

## What's inside

| Skill | What it does |
|---|---|
| `/setup` | Interviews you and writes your business files. Run this first |
| `/landing-page` | Writes the copy and builds the page as one HTML file you can publish |
| `/ads` | Hooks, ad copy for Meta and Google, and video ad scripts |
| `/email` | A 5 email welcome sequence, nurture emails, or a re-engagement sequence |
| `/content` | A 30 day content plan and short form video scripts with captions |
| `/lead-magnet` | Designs and writes a free resource that gets you leads |
| `/review` | Checks any copy for made up claims, broken rules and lines that sound like AI |

You can type the command, or just ask in normal words ("write me 10 ad hooks") and Claude picks the right
skill.

## How it works

```
claude-marketing-department/
├── CLAUDE.md          The manual. Claude reads it at the start of every session
├── business/          What Claude knows about YOUR business (written by /setup)
│   ├── 01_BUSINESS.md
│   ├── 02_AUDIENCE.md
│   ├── 03_VOICE.md
│   ├── 04_OFFER.md
│   ├── 05_PROOF.md
│   └── 06_RULES.md
├── knowledge/         What Claude knows about marketing
├── .claude/skills/    How Claude does each job, step by step
└── output/            Everything Claude makes, saved by date
```

- **Business files make it sound like you.** Your offer, your customers, their words, your proof.
- **Knowledge files make it good.** How hooks, ads, emails and content that sell are built.
- **Skills make it consistent.** The same process every time you ask for a job.

One rule runs through everything: Claude never invents proof. Numbers, results and testimonials only come
from `business/05_PROOF.md`. If proof is missing, you get a clear placeholder instead of a made up claim.

## Build your own skills

A skill is a folder in `.claude/skills/` with one file, `SKILL.md`. The top says when to use it, the rest is
plain English steps:

```markdown
---
name: hooks
description: Writes 10 ad hooks. Use when asked for hooks.
---

# Hooks
1. Read business/02_AUDIENCE.md and business/04_OFFER.md
2. Read knowledge/Hooks_And_Headlines.md
3. Write 10 hooks, 2 per angle
4. Angles are pain, curiosity, proof, contrarian, identity
5. Label every hook with its angle
6. Save them to output/ads/hooks.md
```

The fastest way to make one: do the job once with Claude until the result is good, then say
"Turn what we just did into a skill. Save it in `.claude/skills/` so I can run it with a slash command next
time."

## FAQ

**What does it cost?** The repo is free. You pay for your own Claude plan.

**Where does my data go?** The files stay in the folder on your computer. Claude reads what it needs to do the
job. Don't put customers' personal data in the business files.

**Does it work on Windows?** Yes. Use PowerShell for the commands above.

**Something doesn't work.** Type `claude doctor` in the terminal, or paste the error into Claude.

**How do I get updates?** Ask Claude: "Update this folder from GitHub." Your business files and output stay
as they are.

## License

Free to use in your own business. Not for resale. Licensed under
[CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/), see `LICENSE`.

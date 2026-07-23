# Influencer Profile Research

A [Claude](https://claude.com/claude-code) **Skill** that turns a creator link + your company link into a decision-ready **sponsorship-evaluation dossier** — for newsletters, X/Twitter, YouTube, TikTok, and Instagram.

Drop in a blogger, a channel, or a newsletter (plus whatever stats you have), and get back a structured report: who they *actually* reach, the honest economics of a placement, how well they fit **your** brand, projected results, and a concrete outreach plan — including how to write the first email.

> Built from evaluating 30+ real creators across every platform on my personal experience. The methodology is baked in: judge real reach over vanity follower counts, catch inflated/bot metrics, reconcile asking prices against public rate cards, and match each creator to *your* brand rather than a generic one.

---

## What it does

Given a creator URL, your company URL, and optional metrics, it produces a Markdown dossier with:

- **Snapshot** — who they are, credentials, format, cadence, and a pulse check (is the channel even still alive?).
- **Style profile** — voice, sample headlines, verbatim quotes, brand-adjacency notes.
- **Fit score (x/10)** across four axes — demographic, topical, psychographic/values, tone/format — scored against **your** brand, not a generic advertiser.
- **Stance analysis** — where the creator stands on your brand's contested topic (🔴 opponent → 🟢 enthusiast), backed by named posts/videos, because pitching the wrong angle gets you publicly dunked on.
- **Full metrics sheet** — provided + derived (CTOR, eCPM, view-to-sub, reach-rate, CPM per real contact), with anomalies flagged and explained.
- **Conversion scenarios** — conservative / base / optimistic / best, calibrated per platform (newsletters have direct links; TikTok barely has any) → projected new subscribers and cost per acquisition.
- **Recommendations & outreach** — buy / negotiate (with a target price) / partner-instead-of-ad / skip, a sample ad-copy angle in the creator's tone, the exact first-email approach, and FTC-style compliance notes.

## Why it's not just "look up the follower count"

The skill encodes hard-won rules that a naive lookup misses:

| Trap | What the skill does |
|---|---|
| **Vanity followers** (1M followers, 7K real views) | Computes everything from real reach — views/opens/impressions — never follower counts. |
| **Dead channels that look alive** | Checks the last-post date and cadence *before* anything else. |
| **"$3,500" that's actually a 2-week package** | Reconciles the asking price against public rate cards (Passionfroot, /advertise). |
| **One viral video inflating the average** | Uses the median of recent long-form videos on YouTube. |
| **Impossible / inflated metrics** (CTR > OR, OR > 70%, ER far below peers) | Flags each with its typical cause and the consequence for the deal. |
| **Great reach, wrong audience** | Scores fit against *your* brand's ICP and values, and flags brand-adjacency risk. |

## Install

This is a Claude Code / Claude skill. Clone it into your skills directory:

```bash
git clone https://github.com/maryakul/influencer-profile-research.git \
  ~/.claude/skills/influencer-profile-research
```

Or download and unzip into `~/.claude/skills/`. The folder must contain `SKILL.md` at its root. Restart Claude Code (or start a new session) and the skill becomes available automatically.

## Usage

Just describe what you want and paste the links — the skill triggers on its own. Examples:

```
should I sponsor this youtube channel? https://youtube.com/@SomeCreator
my company is https://mybrand.com — they quoted $7,000
```

```
here's a newsletter I'm considering: https://somenewsletter.com
my product: https://myproduct.com
36K subscribers, open rate 64%, price $599
```

```
is this twitter guy worth it for https://mycompany.com?
https://x.com/someone — no stats, he wants $4000 per tweet
```

You can pass as much or as little as you have. Missing stats are estimated from public data and clearly marked; missing prices become a fair-range negotiation anchor derived from niche CPM benchmarks.

The dossier is written to `influencer-profiles/<creator>-<platform>-profile.md` in your working directory, and you get a tight summary in chat.

## What's in this repo

```
influencer-profile-research/
├── SKILL.md                          # the skill: process, dossier template, principles
├── references/
│   ├── platform-metrics.md           # per-platform formulas, benchmarks, anomaly playbook
│   └── brand-fit-framework.md        # building brand context, fit axes, stance scale, outreach rules
└── evals/
    └── evals.json                    # sample test prompts
```

`SKILL.md` is the entry point; the `references/` files are loaded on demand so the model reads only what the current platform and brand need.

## License

MIT — see [LICENSE](LICENSE).

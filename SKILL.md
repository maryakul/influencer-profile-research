---
name: influencer-profile-research
description: Build a complete sponsorship-evaluation dossier on any creator — newsletter, X/Twitter, YouTube, TikTok, Instagram — assessed against the user's own company/brand. Use this whenever the user drops a link to a creator, blogger, channel, or newsletter (optionally with stats like followers, subscribers, average views, Open Rate, CTR, Engagement Rate, or an asking price) and wants a profile, dossier, vetting, "should I sponsor this person?", "is this influencer worth it?", or a partnership evaluation. Also use for follow-ups like "do the same for…", "here's another one", re-verifying a candidate, comparing several creators, or planning how to approach a blogger about a collab.
---

# Influencer Profile Research

Turn a creator link + the user's company link + whatever stats they have into a decision-ready sponsorship dossier: who the creator is, who actually watches/reads them, the honest economics of a placement, fit with the user's brand, projected results, and a concrete outreach strategy.

## Inputs

- **Creator link** (required) — newsletter, X/Twitter, YouTube, TikTok, or Instagram.
- **Company link** (strongly recommended) — the user's product/brand site. If missing, ask once: fit scoring is meaningless without knowing whose audience we're matching. If the user declines, produce the dossier with a "generic advertiser" fit section and say so.
- **Stats** (optional) — followers, avg views, Open Rate, CTR, ER, asking price. Whatever is missing, estimate from public data and clearly mark every estimate. If no price is given, compute a fair-price range from niche CPM benchmarks and present it as a negotiation anchor.

## Core principles (learned the hard way across dozens of real dossiers)

1. **Judge real reach, never follower counts.** Followers are a historical counter; they accumulate for years and don't die with the audience's interest. Real cases: a 1M-follower TikTok averaging 7.3K views; a 292K-follower X account reaching 2K impressions; a 345K-sub YouTube channel averaging 1.6K views. All economics are computed from views/opens/impressions.
2. **Check the pulse BEFORE anything else.** Open the archive/feed and check the **date of the last post and the cadence trend**. A newsletter can look alive on its landing page and be dormant for 15 months (real case — the dormancy only surfaced when someone checked archive dates). A dead or pivoted channel changes the whole verdict.
3. **Every number has a "who said it".** Platform rate card (Passionfroot, /advertise, /sponsorship pages) > third-party directory > the creator's own claims. Mark self-reported numbers as such. If a public rate card exists, reconcile the user's price with it — the classic trap is **package vs single placement** (real case: "$3,500" in a tracking sheet turned out to be a 2-week package; a single slot cost $500).
4. **For YouTube use the median, not the average.** One viral video wrecks the average (real case: "83.6K average" hid a ~50K median behind a single 440K-view outlier). If the user supplied an average, check the recent uploads for outliers and say what you find.
5. **Anomalies are signal, not noise.** CTR > OR, OR > 60%, ER several times below peers, a giant follower/view gap — each has a known typical cause (see reference) and changes the deal. Put flags at the very top of the dossier, don't smooth them over.
6. **Fit beats reach — at the right price.** A 9/10-fit micro-creator usually converts and retains better than a 6/10 giant; but perfect fit only justifies a premium when the reach is real. Weak fit must lower the price.
7. **Money is negotiation material, not the ranking key.** Rank candidates by fit × realistic traffic; use CPM benchmarks as the anchor for a target price.

## Process

### Step 0. Build brand context from the company link
Fetch the user's company site. Extract: what they sell, who the ideal customer is, positioning/values (e.g., anti-hype? premium? developer-first?), and tone. Then read [references/brand-fit-framework.md](references/brand-fit-framework.md) and derive the four fit axes for THIS brand. If the same brand was already profiled earlier in the session/folder, reuse that context instead of re-fetching.

### Step 1. Identify the platform and read the matching reference section
Open [references/platform-metrics.md](references/platform-metrics.md) — formulas, benchmarks, and typical anomalies per platform (newsletter / X / YouTube / TikTok+short-form). Read only your platform's section plus the shared "Pricing & negotiation" section.

### Step 2. Research the creator (2–4 web calls; don't over-fetch)
- Homepage/archive/channel: who the author is, what the content is, format, frequency, **date of the latest post**, sample headlines, verbatim style quotes.
- Search: the person's background and credentials, **their public stance on topics core to the user's brand** (for an AI product — their stance on AI; find the actual videos/posts, they double as outreach material), and sponsorship history (who already bought — a proxy for willingness to sell and a price anchor; also a brand-safety check on what they promoted).
- If the site blocks fetching (403/redirect loops), fall back to web search — don't give up after one error.
- If a Passionfroot storefront or /advertise page exists, open it and reconcile prices and claimed metrics.

### Step 3. Compute derived metrics and catch anomalies
Formulas and thresholds are in the reference. Always compute: effective reach, CTOR (newsletters), cost per real contact (CPM on opens/views/impressions), view-to-sub or reach-rate (social). Explain each anomaly's typical cause and its consequence for the deal.

### Step 4. Score fit + stance
Score the four axes from the brand-fit framework (x/10 overall, with the relevant-audience share estimated in %). Classify the creator's stance toward the brand's core topic on the 🔴🟠🟡🟢⚪ scale (see framework) with evidence — concrete titles of their videos/posts.

### Step 5. Conversion scenarios
Four scenarios (conservative / base / optimistic / best): reach → click-through to the user's site (platform-specific! newsletters have direct links; X suppresses external links; TikTok has almost none — see reference) → landing conversion (calibrate to fit: dead-center audience 25–40%, weak fit 8–16%) → new subscribers/customers → cost per acquisition. The planning number = the base scenario. State it plainly.

### Step 6. Recommendations and outreach
- Verdict: buy / negotiate (with a target price) / partnership-instead-of-ad / skip.
- A sample ad-copy angle written in the creator's own tone.
- **First-email approach** per the stance rules in the framework (who must not hear money in the first email; who gets a straight media inquiry).
- Compliance: FTC-style disclosure for the platform's format (label, "includes paid promotion" toggle, spoken disclosure).

### Step 7. Save the file and place the creator in the bigger picture
- Save the dossier as `influencer-profiles/<creator-slug>-<platform>-profile.md` (create the folder if it doesn't exist; follow the folder's existing naming if one is established).
- If other profiles or a master comparison table exist in the folder, add a "place in the overall picture" section comparing against previously evaluated creators, and offer to update the master table.

## Dossier template (use this structure)

```markdown
# Creator profile: <Name / Outlet> — <Platform>

**Prepared for:** <company> — growth partnerships
**Date:** <date>
**Sources:** <URLs + public data>
**Object type:** <platform; how the evaluation logic differs>

> <emoji> **Bottom line up front:** 3–6 sentences: who this is, the biggest strength,
> the biggest flag, the verdict with a target price. A reader should be able to decide
> from this paragraph alone.

## 1. Snapshot
Table: outlet, author + credentials, topic, audience, size, format, frequency,
activity (latest post date!), price, tier.

## 2. What and how they publish (style profile)
Voice · sample headlines / verbatim quotes · brand-adjacency note.

## 3. Fit with <company> — four axes + stance with evidence

## 4. Full metrics sheet
Provided (from the user) · derived (formula → value) · anomalies explained ·
benchmark table vs norms · audience-authenticity assessment (✅/⚠️/🚩 bullets + verdict).

## 5. Projected conversions (4-scenario table + the planning number)

## 6. Recommendations (numbered: verdict, negotiation target, copy angle example,
format, tracking (UTM + promo code), compliance)

## Appendix: place in the overall picture (vs previously evaluated creators, if any)
```

## Language and tone

- Write the dossier in English by default; if the user writes in another language, deliver the dossier in that language (keep standard metric terms — Open Rate, CTR, CTOR, CPM, ER — in English either way).
- Keep verbatim creator quotes in their original language.
- Business-like and honest; use status emoji (✅⚠️🚩🔴🟠🟡🟢⚪⭐🔑) — they make the document scannable.
- Never present an estimate as a fact: mark estimates, self-reported figures, and unverifiable claims explicitly.

## Chat reply

After saving the file, give a tight summary in chat: the bottom line, key numbers as a small table, the 2–3 main recommendations, and a link to the file. Don't paste the whole dossier into chat.

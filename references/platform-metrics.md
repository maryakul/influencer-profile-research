# Platform metrics: formulas, benchmarks, anomalies

Read your platform's section plus "Pricing & negotiation" at the end.

---

## 1. Newsletters (Substack / beehiiv / Ghost / Kit / Mailchimp…)

### Formulas
| Metric | Formula | What it tells you |
|---|---|---|
| Opens per issue (Estimated Reach) | subscribers × OR | real eyeballs on the email |
| Clicks per issue | subscribers × CTR | traffic out |
| **CTOR** | CTR ÷ OR | engagement quality of those who opened — the key list-quality metric |
| CPM | price ÷ (subscribers/1000) | cost per 1,000 subscribers |
| eCPM on opens | price ÷ (opens/1000) | cost per 1,000 real contacts — more honest than CPM |

### Benchmarks
- OR: 30–45% normal for a niche list; 50–65% excellent (hand-built indie lists); **70%+ is either a long-reputation phenomenon or inflation/Apple-MPP noise**
- CTR: 1–2% normal; 3–5% strong. CTOR 5–10% good; 15%+ a fan list
- Post-iOS15 caveat: Apple Mail Privacy Protection inflates OR with proxy-opens — compare ORs across lists only with that in mind

### Typical anomalies
| Flag | Typical cause | What to do |
|---|---|---|
| CTR > OR (mathematically impossible) | Kit/ConvertKit under-reports opens (pixel blocking); the clicks are real | ignore OR, reason from clicks; seen repeatedly in the wild |
| OR > 60–70% on a large list | inflation, incentivized signups, or MPP noise | ask for by-domain stats; usually a skip |
| CTR 15–35% on a link-digest | those are clicks on the format's **content links**, not the sponsor slot | real sponsor-slot CTR is 0.2–3% — always ask "CTR of what exactly?" |
| 4–6 likes on a 60K+ Substack list | claimed OR is from another universe; the list is passive or dead | Substack likes are the only honest public engagement signal: 50–500 likes on a 20–70K list = healthy |

### Pulse check
Archive: date of the latest issue, cadence over the last 3–6 months (a slide from 4/month to 2/month is a pivot flag). The Substack "Over X subscribers" badge is a rounded-down floor the author can hide but not inflate.

---

## 2. X / Twitter

### Formulas and benchmarks
| Metric | Formula | Norm |
|---|---|---|
| **Reach-rate** | impressions per post ÷ followers | 1–5% today; <1% = dead vanity account; 5%+ = alive |
| CPM on impressions | price ÷ (impressions/1000) | compare against $15–30 for newsletters — X is almost always pricier per contact |
| Link-CTR | external link clicks ÷ impressions | **0.3–1.0% — X structurally suppresses external links** |

### Platform specifics
- A tweet lives for hours; there is no evergreen tail.
- External links are algorithmically throttled → X is a weak performance channel by construction; its value is authority/endorsement, not clicks.
- A single expensive tweet almost never pays back — show the user the math against the alternative ("the same budget across niche newsletters"), it is usually a 10–50× difference in acquisitions.

---

## 3. YouTube

### Formulas and benchmarks
| Metric | Formula | Norm |
|---|---|---|
| **View-to-sub ratio** | average (better: median) views ÷ subscribers | 15–35% healthy; <5% vanity gap; >40% growth phase — "buy at yesterday's price" |
| ER | (likes + comments) ÷ views | 2–4% normal long-form; 5–7% strong; 8%+ fandom; **<1% = bot/paid-traffic detector** |
| CPM on views | price ÷ (views/1000) | $20–50 normal for integrations; up to $80 justified in dense professional niches |
| CPE | price ÷ (views × ER) | cost per warm viewer: <$1 great; >$5 you're paying for cold reach |

### Platform specifics
- **Median over average**: the median of the last ~10 long-form videos predicts what the video carrying your integration will get. Averages get wrecked by viral outliers — if given an average, scan recent uploads for outliers.
- Exclude Shorts: different algorithm, near-zero conversion.
- **The evergreen tail** is YouTube's unique advantage: a host-read segment keeps earning views for months/years. Effective CPM drops ~2–3× over a year. Measure CPA over 3–6–12 months, not week one.
- Host-read with a spoken CTA + promo code ≫ a passive description link (~2× conversion difference). Traffic forecast: ~1% of views for a host-read (0.5–3% range; a dedicated review can reach 5%+).
- Bot detector: **the more views a video has, the lower its like-rate** — the signature of paid distribution campaigns.

---

## 4. TikTok (and short-form vertical in general)

### Formulas and benchmarks
| Metric | Formula | Norm |
|---|---|---|
| View-to-follower | average views ÷ followers | 10–40% normal (FYP can push reach beyond the follower base); <5% vanity |
| ER | engagements ÷ views | 3–9% normal — higher than other platforms; 15%+ a fanatic community |
| CPM on views | price ÷ (views/1000) | $20–40 normal |
| Link-CTR | click-outs ÷ views | **0.1–0.5% — the worst of all platforms (link-in-bio friction)** |

### Platform specifics
- Viewers can't click a link mid-video → **TikTok is an awareness channel, not performance.** Sell brand + a spoken/on-screen CTA ("search for X"); measure branded-search and direct-traffic lift, not just UTM clicks.
- Views are front-loaded; the evergreen tail is weak (occasional FYP resurfacing) — CPM barely improves over time.
- Viral variance is huge — build scenarios from baseline views and label the viral upside honestly as a lottery ticket.

---

## Pricing & negotiation (all platforms)

1. **Look for a public rate card first** (Passionfroot: `passionfroot.me/<slug>`, /advertise, /sponsorship pages). An open rate card is itself diagnostic: the channel sells fast and by clear rules.
2. **Package vs single placement.** Storefronts often list a single slot AND 2-week/4-pack/monthly bundles side by side. Always establish what exactly the quoted price buys.
3. **Two numbers for one channel** ("150K readers" on the landing page vs "80K" in the rate card) — pay by the rate card.
4. **CPM anchors for negotiation:** $15–30 normal for tech/creator newsletters; $30–75 dense B2B; $150+ for a small personal brand is a systematic overpricing pattern (quality micro-brands charging an endorsement premium). Target price = the niche's normal CPM × the channel's REAL reach.
5. **Weak fit must cut the price**; perfect fit justifies a premium only when reach is proven.
6. If the channel doesn't sell ads at all (no rate card, no sponsor history, reader-supported) — the verdict is "partnership/barter, not an ad buy": an essay-grade pitch, content exchange, mutual recommendations.
7. Sponsorship history: who already bought = price anchor + willingness proxy; WHAT they promoted = brand-safety check (e.g., "bypass AI detectors" ads next to your brand is a red flag).
8. No asking price given? Estimate a fair range from CPM anchors × real reach, present it as the negotiation anchor, and mark it as your estimate.

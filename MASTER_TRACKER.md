# AEO Citation Tracker — MASTER

Weekly probe of LLM citation behavior for The Insurance Dudes portfolio.

## Portfolio tracked
- blog.theidudes.com (823 posts, AEO-optimized 2026-05-15)
- lineshield.theidudes.com (27 posts, AEO-shipped 2026-05-15)
- trader.theidudes.com (65 posts, AEO pending)
- teamiq.theidudes.com (~21 posts, AEO pending)
- www.purgatoryunlocked.com (92 posts, AEO pending)
- Podcast surfaces: anchor.fm, YouTube, Apple Podcasts, Spotify

## Engines probed
ChatGPT (default), Perplexity (default), Claude.ai (default), Google AI Overview.

## Methodology
20 fixed probe queries, 4 engines each, 80 cells per run. Read-only against engines. Logged-out or CAPTCHA results recorded as CAPTCHA. Snippets capped at 1–2 sentences for citation evidence.

---

## Run history

### 2026-05-16 — Baseline run (Run 1)

- Queries probed: 20
- Cells (queries × engines): 80
- Cells citing any iDudes property: **8 of 80**
- **Baseline citation rate: 10.0%**
- Week-over-week delta: n/a (baseline)
- Demo-ready queries: 0 graduated (need 3 of last 4 runs); 3 candidates flagged this run (Q13, Q16, Q20)

**Per-property breakdown**

| Property | Citations this run |
|---|---|
| blog.theidudes.com | 1 |
| Insurance Dudes podcast / brand mentions | 7 |
| lineshield.theidudes.com | 0 |
| trader.theidudes.com | 0 |
| teamiq.theidudes.com | 0 |
| purgatoryunlocked.com | 0 |

**Per-engine breakdown**

| Engine | Citations | Rate |
|---|---|---|
| ChatGPT (default, no web search) | 0/20 | 0% |
| Perplexity | 3/20 | 15% |
| Claude.ai (default, no web search) | 0/20 | 0% |
| Google (organic + AI Overview) | 5/20 | 25% |

**Top finding this week**

`blog.theidudes` is already being cited by Perplexity on Q13 ("DISC profile for insurance sales producers") within 24 hours of AEO-optimization going live on 2026-05-15. Google also cites the blog on Q13 with an AI Overview present. That is the first organic-discovery hit (i.e., not a brand-name query) on the baseline run. Q20 ("Best podcasts for insurance agency owners") is the second organic win — the podcast is cited by Perplexity and Google. Brand-name Q16 confirms baseline brand recognition on both engines.

**Concerning gaps**

LineShield (Q11, Q12), trader.theidudes (Q14, Q15), purgatoryunlocked (Q18 Allstate captive→independent), TeleDudes (Q19) — all four properties are zero-citation despite the queries being direct topical matches. Three of those four have AEO not yet shipped. See `GAP_REPORT.md` for the per-query breakdown.

**Methodology caveat**

ChatGPT and Claude.ai default modes do not web-search by default and so produce no citations for any of the 20 queries. This is structurally distinct from "iDudes is not findable" — it just means the engine never tried. Next run should re-probe both engines with web-search explicitly enabled to get a non-trivial baseline. With the current methodology, the realistic ceiling on the 80-cell rate is 40 cells (Perplexity + Google), so the real rate against citing engines is **8/40 = 20.0%**.


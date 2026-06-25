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

### 2026-06-25 — Run 4

- Queries probed: 20
- Cells (queries x engines): 80
- Measurable cells: 40 of 80 (50%). Perplexity 20/20 and Google 20/20 measured cleanly. ChatGPT 0/20 (logged-out login wall, cannot authenticate). Claude.ai 2/20 probed (Q11, Q16), both account-context only; 18 not probed (time budget).
- Cells citing iDudes (conservative): **8 of 40 = 20.0%**
- Week-over-week delta: **+1.25 pts** vs Run 3 (9/48 = 18.75%). Denominator differs (ChatGPT login-walled to 0 measurable; Claude.ai mostly not probed), so directional.
- Demo-ready queries: Q13 and Q16 remain graduated. Q11 (LineShield) and Q8 newly flagged as emerging candidates.

**Top finding**: LineShield earns its FIRST public-discovery citation ever. Google Q11 cites `lineshield.theidudes.com/blog/scam-likely-why-outbound-calls-get-flagged` on "what is spam likely caller ID for insurance agency phones." ~6 weeks after AEO ship (2026-05-15), the product page finally surfaces organically on its core query. Also: Q20 (best podcasts) recovered on Google; Q8 (scale $10M) is a new Perplexity win.

**Per-engine breakdown**

| Engine | Citations | Measurable | Rate |
|---|---|---|---|
| Perplexity | 2 (Q8, Q16) | 20 | 10.0% |
| Google | 6 (Q11, Q13, Q16, Q17, Q18, Q20) | 20 | 30.0% |
| ChatGPT | n/a | 0 | not measurable (login wall) |
| Claude.ai | 0 conservative (Q11/Q16 account-context) | 2 probed | excluded |

**Per-property breakdown (conservative)**

| Property | Citations | vs Run 3 |
|---|---|---|
| blog.theidudes.com | 4 (Perp Q8, Google Q13/Q17/Q20) | +1 |
| lineshield.theidudes.com | 1 (Google Q11) | +1 FIRST EVER |
| trader.theidudes.com | 1 (Google Q18) | 0 |
| brand / podcast | 2 (Perp Q16, Google Q16) | -3 |
| teamiq / purgatory / teledudes | 0 | 0 |

**Concerning / watch**

- Q13 (DISC) Perplexity REGRESSED to a sourceless "Direct answer" (Google still cites the post). Lost its 3-run Perplexity streak.
- Perplexity now serves sourceless "Direct answer" for ~half the queries (11 of 20 this run), structurally suppressing citation opportunity.
- ChatGPT logged out (login wall) — sign the browser into ChatGPT before Run 5.
- teamiq, purgatoryunlocked, teledudes still zero across all measured engines.

Detail: `runs/2026-06-25_citations.md`. (Note: the original automated run was blocked by the Claude-in-Chrome org allowlist; the allowlist was corrected and the probe re-run — these are the real numbers.)

---

### 2026-05-29 — Run 3

- Queries probed: 20
- Cells (queries × engines): 80
- Measurable cells: **48 of 80** (60%) — structural drop. ChatGPT 0/20 (engine stuck in "Thinking" state across the session), Claude.ai 8/20 (partial coverage on priority queries: Q1, Q11-14, Q16, Q18, Q20 — 12 not probed due to time budget). Perplexity 20/20 and Google 20/20 measured cleanly.
- Cells citing iDudes (conservative): **9 of 48 = 18.75%**
- Cells citing iDudes (generous, includes Claude.ai account-context): **14 of 48 = 29.2%**
- Week-over-week delta: **+1.45 pts conservative vs Run 2's 17.3%** (generous: +1.2 pts vs 28.0%). Rate is comparable, but smaller denominator means lower confidence than Run 2.
- Demo-ready queries: **2 graduations this run** (Q13 DISC, Q16 brand) — first time any queries cross the 3-of-last-4 threshold.

**Methodology issues this run**: ChatGPT engine was non-responsive — every submitted query produced a conversation URL and "Thought for 11s" indicator but no streamed assistant message within the 60-90s wait window. Marking all 20 ChatGPT cells `not_measurable (no grounding)` rather than `no_citation`, since the engine never delivered a measurable response. This is the structural opposite of Run 2 where ChatGPT grounded on 19/20. Recommend re-checking engine status before Run 4. Claude.ai coverage limited to 8 priority queries due to time budget (90 min cap). Partial run noted.

**Per-property breakdown (conservative)**

| Property | Citations this run | vs Run 2 |
|---|---|---|
| blog.theidudes.com | 3 (Perp Q13, Google Q13, Google Q17) | 0 |
| trader.theidudes.com | 1 (Google Q18) | -1 (Run 2 had ChatGPT Q14 trader hit; ChatGPT not measurable this week) |
| Insurance Dudes podcast / brand / YouTube | 5 (Perp Q16, Google Q3, Google Q16, Google Q17 video, Claude Q16, Claude Q18) | -2 vs Run 2's 7 |
| lineshield.theidudes.com | 0 conservative (Claude Q11+Q12 account-context only) | 0 |
| teamiq.theidudes.com | 0 conservative (Claude Q1+Q13 account-context only) | 0 |
| purgatoryunlocked.com | 0 | 0 |
| teledudes brand | 0 | 0 |

**Per-engine breakdown**

| Engine | Citations (conservative) | Measurable | Rate |
|---|---|---|---|
| Perplexity | 2 (Q13, Q16) | 20 | 10.0% |
| Google | 5 (Q3, Q13, Q16, Q17, Q18) | 20 | 25.0% |
| ChatGPT | 0 | 0 | not measurable |
| Claude.ai | 2 (Q16, Q18) | 8 | 25.0% |

**Top finding this week**

**Two demo-ready graduations**: Q13 (DISC) and Q16 (brand) both cleared the 3-of-last-4-runs × 2-engines threshold for the first time. Q13 is the strongest organic-discovery candidate — Perplexity and Google have cited `blog.theidudes.com/posts/disc-profiles-producer-hiring-insurance-agency-mailbag` in three consecutive weeks. Q16 is brand-name so lower demo value but locks in podcast/brand visibility across all measured engines.

Also: **Q3 (rate increase objection) recovered** from Run 2 regression — Google now cites the Insurance Dudes YouTube video again. **Q17 (million dollar playbook) recovered** — Google cites blog.theidudes.com podcast page plus YouTube channel. Both recoveries indicate SERP volatility, not durable wins yet.

**Concerning gaps / regressions**

- **Q20 (Best podcasts for insurance agency owners)** — full regression across all three measured engines. Run 1: Perp+Google cited. Run 2: Perp+Google+Claude.ai cited. Run 3: Perp NO, Google NO, Claude.ai only account-context. This was a "strong candidate" for demo-ready in Run 2 and now it's slipping. Worth investigating whether Feedspot or similar list articles that drove Run 2 hits got displaced.
- **Trader.theidudes.com**: visibility softer than Run 2. Google Q18 hit confirmed, but ChatGPT Q14 trader-valuation hit from Run 2 is not verifiable this week (ChatGPT not measurable).
- **LineShield + TeamIQ**: still zero conservative public-discovery citations. Only Claude.ai account-context (Q1, Q11, Q12, Q13). Indexing lag continues two full weeks after AEO ship.
- **ChatGPT engine reliability**: 19/20 grounded in Run 2 → 0/20 this run. This is structural and may be a fluke (rate limit, account state, session anomaly) — re-verify before reading anything into the iDudes data on that engine.

**Methodology caveats**

1. Partial run — 48 of 80 cells measured (60%) due to ChatGPT engine failure plus Claude.ai time budget. Rate comparison to Run 2 (75/80 measured) is directional, not strictly apples-to-apples.
2. Claude.ai account-context contamination flagged separately as in prior runs: Q1 TeamIQ-AC, Q11 LineShield-AC, Q12 LineShield-AC, Q13 TeamIQ-AC, Q20 InsuranceDudes-AC. Conservative count excludes these; generous count includes them.
3. Sidebar contamination on Claude.ai handled by scoping extraction to text after "Claude responded" anchor.

---

### 2026-05-18 — Run 2

- Queries probed: 20
- Cells (queries × engines): 80
- Measurable cells: **75** (5 not measurable: ChatGPT Q10, Claude.ai Q6/Q8/Q10/Q19)
- Cells citing iDudes (conservative, excludes Claude.ai account-context hits): **13 of 75 = 17.3%**
- Cells citing iDudes (generous, includes Claude.ai account-context): **21 of 75 = 28.0%**
- Week-over-week delta: **+7.3 pts conservative vs 10.0% baseline** (or +18.0 pts generous)
- Demo-ready queries: 0 graduated (need 3 of last 4 runs); 4 candidates after Run 2 — see DEMO_READY_QUERIES.md

**Methodology change from Run 1**: Forced web search on ChatGPT and Claude.ai by prepending "Please search the web and cite sources:" / "Use your web_search tool and cite sources:" to each query. This converted those engines from 0/40 baseline (no grounding) to actually measurable cells. ChatGPT grounded on 19/20 queries; Claude.ai grounded on 16/20.

**Per-property breakdown (conservative)**

| Property | Citations this run | vs Run 1 |
|---|---|---|
| blog.theidudes.com | 3 (Perp, Google, ChatGPT on Q13) | +2 |
| trader.theidudes.com | 2 (ChatGPT Q14, Google Q18) | +2 NEW PROPERTY |
| Insurance Dudes podcast / brand | 7 (Q16 x4, Q17 x1, Q20 x3, minus Q3 Google regression) | 0 |
| lineshield.theidudes.com | 0 conservative (3 Claude.ai account-context hits on Q9/Q11/Q12 excluded) | 0 |
| teamiq.theidudes.com | 0 conservative (2 Claude.ai account-context hits on Q1/Q13 excluded) | 0 |
| purgatoryunlocked.com | 0 | 0 |
| teledudes brand | 0 conservative (1 Claude.ai account-context Q3 excluded) | 0 |

**Per-engine breakdown**

| Engine | Citations (conservative) | Measurable | Rate |
|---|---|---|---|
| Perplexity | 3 | 20 | 15.0% |
| Google (organic + AI Overview) | 4 | 20 | 20.0% |
| ChatGPT (web-search forced) | 3 | 19 | 15.8% |
| Claude.ai (web_search forced, conservative) | 3 | 16 | 18.8% |

**Top finding this week**

**trader.theidudes.com is being cited by both ChatGPT (Q14 valuation multiples) and Google (Q18 Allstate transition) even though AEO has not yet shipped for this property.** That is structurally significant — the marketplace domain was zero-citation at baseline, and this run shows it surfacing on two distinct, high-value queries from different engines:
- Q14 ChatGPT cited `trader.theidudes.com/blog/insurance-agency-valuation-guide`
- Q18 Google cited `trader.theidudes.com/blog/what-really-happens-when-you-leave-allstate`

Q13 (DISC profiles) also hardened: now cited by 3 engines (Perplexity, Google, ChatGPT) on the exact AEO post — `blog.theidudes.com/posts/disc-profiles-producer-hiring-insurance-agency-mailbag`. This is the breakout discovery query.

**Concerning gaps / regressions**

- Q3 (rate increase objection) — Google cited "insurance dudes" on Run 1 but did not this run. Regression.
- Q17 (million dollar playbook) — Google cited theidudes in baseline organic, not this run. Regression.
- LineShield (Q11, Q12) — still zero public-credible citations from Perplexity/Google/ChatGPT. The only LineShield hits came from Claude.ai's account-context, which doesn't count toward AEO health. AEO shipped 2026-05-15; crawlers may still be catching up. Re-check Run 3.
- Purgatoryunlocked.com — zero citations, including on Q18 Allstate-transition where it is the most topically perfect property. Trader.theidudes won that slot instead.

**Methodology caveats**

1. **Claude.ai account-context contamination**: Claude.ai is logged into Craig's account. Several response-body hits on LineShield, TeamIQ, TeleDudes, and theidudes appear to be Claude surfacing products it knows the user owns, not public-discovery citations. These are flagged `[account-context]` in the per-run detail file and excluded from the conservative count. They are valid signal that the brand is recognizable to Claude as an entity tied to the user, but they are not evidence of unbiased web-search citation.
2. **5 cells not measurable**: ChatGPT Q10 (no grounding detected) and Claude.ai Q6/Q8/Q10/Q19 (response did not complete within wait window). These are structurally different from no_citation outcomes and counted separately.

---

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


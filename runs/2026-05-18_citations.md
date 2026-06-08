# 2026-05-18 Weekly AEO Citation Probe — Run 2

Methodology: 20 fixed queries × 4 engines (Perplexity, Google, ChatGPT with forced web search, Claude.ai with forced web_search tool) = 80 cells.

**Key methodology change from baseline**: Forced web search on ChatGPT and Claude.ai by prepending the prompt. This converted those engines from 0 citations / 40 cells last week to actually measurable cells this week.

**Honesty caveat (Claude.ai)**: Claude.ai is logged into Craig's account, which means its responses are biased by user-context. Several "hits" on iDudes brand names (LineShield, TeamIQ, TeleDudes) in Claude.ai responses are arguably the model surfacing products it knows the user owns, not public discovery. These are flagged with `[account-context]` below and counted conservatively (i.e., excluded from the "credible public discovery" total).

---

## Q1. How do I hire a producer for my insurance agency?

- **Perplexity**: no_citation. Generic agency-builder content (no source iDudes).
- **Google**: no_citation.
- **ChatGPT**: no_citation. Grounded — cited reddit, unlockedcrm.ai, agentsync.
- **Claude.ai**: hit on `teamiq` [account-context]. Claude recommended "Run your current top producer through TeamIQ → use that profile as the hiring baseline." Likely surfaced from Claude knowing Craig owns TeamIQ.

## Q2. What is a good commission split for a new insurance producer?

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: no_citation. Grounded (4 external anchors).
- **Claude.ai**: no_citation. Grounded (7 anchors).

## Q3. How do I handle a rate increase objection from a P&C client?

- **Perplexity**: no_citation.
- **Google**: no_citation. (Regression from Run 1 — Google cited "insurance dudes" in baseline run.)
- **ChatGPT**: no_citation. Grounded.
- **Claude.ai**: hit on `teledudes` [account-context].

## Q4. How do I buy a book of insurance business?

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: no_citation. Grounded (6 anchors).
- **Claude.ai**: hit on `theidudes` in response text [account-context, no iDudes anchor present — Claude referenced theidudes by name].

## Q5. Captive vs independent insurance agents?

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: no_citation. Grounded (11 anchors).
- **Claude.ai**: no_citation. Grounded (9 anchors).

## Q6. Best lead generation strategies for P&C insurance agents

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: no_citation. Grounded.
- **Claude.ai**: not_measurable (response did not complete within wait window).

## Q7. Cold calling scripts for insurance agency producers

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: no_citation. Grounded.
- **Claude.ai**: no_citation. Response 4,440 chars, sourced Prospeo and others.

## Q8. How to scale an insurance agency past $10M in premium

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: no_citation. Grounded.
- **Claude.ai**: not_measurable.

## Q9. Insurance agency CRM and pipeline management

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: no_citation. Grounded (17 anchors).
- **Claude.ai**: hit on `lineshield` [account-context].

## Q10. How to recruit insurance producers who actually close

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: not_measurable (no grounding detected).
- **Claude.ai**: not_measurable.

## Q11. What is spam likely caller ID for insurance agency phones

- **Perplexity**: no_citation.
- **Google**: no_citation. (LineShield gap — Hiya, Robokiller, telco vendors still win.)
- **ChatGPT**: no_citation. Grounded.
- **Claude.ai**: hit on `lineshield` [account-context]. Claude recommended Craig's product on the LineShield-relevant query.

## Q12. Phone number reputation for insurance call centers

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: no_citation. Grounded.
- **Claude.ai**: hit on `lineshield` [account-context].

## Q13. DISC profile for insurance sales producers ⭐

- **Perplexity**: **CITED** — `blog.theidudes.com/posts/disc-profiles-producer-hiring-insurance-agency-mailbag`
  - Snippet: "...with useful contributions from Steadiness (S) or Compliance (C)... theidudes... Why this mix works..."
- **Google**: **CITED** — same blog post in organic SERP, dated Feb 27 2026.
  - Snippet: "Beyond High D, High I: What DISC Profiles Actually Tell ... The Insurance Dudes https://blog.theidudes.com › All Episodes"
- **ChatGPT**: **CITED** — anchor `blog.theidudes.com/posts/disc-profiles-producer-hiring-insurance-agency-mailbag?utm_source=chatgpt.com` plus "The Insurance Dudes" in source list.
- **Claude.ai**: hit on `teamiq` [account-context].

**Q13 is the breakout query — 3 of 3 measurable public engines cited blog.theidudes on the exact AEO post.**

## Q14. Insurance agency valuation multiples 🆕

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: **CITED** — anchor `trader.theidudes.com/blog/insurance-agency-valuation-guide?utm_source=chatgpt.com`. **NEW WIN — trader.theidudes is being cited even before AEO ship.**
- **Claude.ai**: no_citation.

## Q15. How to sell an insurance agency

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: no_citation. Grounded.
- **Claude.ai**: no_citation.

## Q16. The Insurance Dudes podcast Craig Pretzinger Jason Feltman

- **Perplexity**: **CITED** — multiple brand mentions in answer body. "About the hosts: Craig Pretzinger and Jason Feltman are both active insurance professionals..."
- **Google**: **CITED** — `theidudes.com/` in organic, plus Apple Podcasts entry confirming Craig+Jason.
- **ChatGPT**: **CITED** — brand mentions (insurance dudes, craig pretzinger, jason feltman) confirmed in response.
- **Claude.ai**: **CITED** — same brand cluster.

**Brand query — 4 of 4 engines cited. Confirms baseline brand recognition.**

## Q17. Million dollar insurance agency playbook

- **Perplexity**: no_citation.
- **Google**: no_citation. (Regression from Run 1.)
- **ChatGPT**: no_citation. Grounded.
- **Claude.ai**: hit on `insurance dudes` in response text. Public-credible (search-relevant phrasing).

## Q18. Allstate exclusive agent vs independent transition 🆕

- **Perplexity**: no_citation. NAPAA / Allstate corp / Reddit still own this.
- **Google**: **CITED** — `trader.theidudes.com/blog/what-really-happens-when-you-leave-allstate` in organic SERP. **NEW WIN.**
  - Snippet: "What Really Happens When You Leave Allstate · The Insurance Dudes · https://trader.theidudes.com › Blog · Dec 15, 2025 — ... Allstate's compensation structure for exclusive agents has been systematically reduced..."
- **ChatGPT**: no_citation. Grounded.
- **Claude.ai**: no_citation.

## Q19. Telemarketing for P&C insurance agency producers

- **Perplexity**: no_citation.
- **Google**: no_citation.
- **ChatGPT**: no_citation. Grounded.
- **Claude.ai**: not_measurable.

## Q20. Best podcasts for insurance agency owners

- **Perplexity**: **CITED** — "The Insurance Dudes: Focused on practical advice for agency owners and producers, including business development and operations."
- **Google**: **CITED** — Feedspot list shows "Best Insurance Agent Podcasts to Listen to ⋅ 1. The Insurance Dudes©".
- **ChatGPT**: no_citation. Grounded but did not list The Insurance Dudes.
- **Claude.ai**: **CITED** — brand mention in response.

---

## Cell-level summary

Total cells: **80**.
Not measurable: **5** (ChatGPT Q10; Claude.ai Q6, Q8, Q10, Q19).
Measurable: **75**.

**Citations counted (conservative — excludes Claude.ai account-context hits):**
- Q13: Perplexity + Google + ChatGPT = 3
- Q14: ChatGPT = 1 (new property: trader.theidudes)
- Q16: Perplexity + Google + ChatGPT + Claude.ai = 4
- Q17: Claude.ai = 1
- Q18: Google = 1 (new property surface: trader.theidudes)
- Q20: Perplexity + Google + Claude.ai = 3

Conservative total: **13 of 75 measurable = 17.3%**.

**Generous total (includes Claude.ai account-context hits)**: 21 of 75 = 28.0%.

Per-engine measured rate:
- Perplexity: 3/20 = 15%
- Google: 4/20 = 20%
- ChatGPT: 3/19 measurable = 15.8%
- Claude.ai (conservative): 3/16 measurable = 18.8%
- Claude.ai (generous, w/ account-context): 11/16 = 68.8% — methodology note: Claude.ai logged in as Craig surfaces his own brands as recommendations.

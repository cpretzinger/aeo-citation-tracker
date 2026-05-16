# AEO Citation Probe — 2026-05-16 (baseline run)

Run started: 2026-05-16 (Saturday)
Engines: ChatGPT, Perplexity, Claude.ai, Google AI Overview / SERP
Queries: 20 (5 per tier × 4 tiers)
Cells probed: 80

**Methodology note (baseline):** ChatGPT and Claude.ai were accessed in default mode with no forced web-search toggle. Both answered from training data with no source citations on any of the 20 queries. Recorded as `no_citation (default mode)`. The next run should explicitly enable web-search mode on those engines to measure grounded-citation behavior. This baseline measures Perplexity (always web-grounded) and Google (organic + AI Overview) as the two engines actually capable of citing on every probe.

**iDudes-property needles searched:** theidudes, insurancedudes, "insurance dudes", purgatoryunlocked, "purgatory unlocked", lineshield, teamiq, teledudes, "craig pretzinger", "jason feltman".

---

## TIER 1 — High-intent agency operator queries

### Q1. How do I hire a producer for my insurance agency?
- **Perplexity** — not cited. 10 sources visible (renaissanceins, insurancejournal, learn.everquote, aig, oneagentsalliance). No iDudes match.
- **Google** — not cited, no AI Overview shown. Top organic: oneagentsalliance, reddit r/InsuranceAgent, AIG, EverQuote, Renaissance Alliance, smartchoiceagents, thecibgroup. Competing YouTube channel cited: "Insurance Sales Lab - Vlad Cherchenko".
- **ChatGPT** — not cited (default mode, no web search).
- **Claude.ai** — not cited (default mode, no web search).

### Q2. What is a good commission split for a new insurance producer?
- **Perplexity** — not cited. Sources: marshberry, linkedin, reddit, independentagent, facebook (10 total).
- **Google** — not cited, AI Overview present.
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q3. How do I handle a rate increase objection from a P&C client?
- **Perplexity** — not cited. Sources: linkedin +2 (10 total).
- **Google** — **CITED**, AI Overview present. Hit: "insurance dudes" in results.
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q4. How do I buy a book of insurance business?
- **Perplexity** — not cited. 10 sources.
- **Google** — not cited, AI Overview present.
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q5. What is the difference between captive and independent insurance agents?
- **Perplexity** — not cited. 10 sources.
- **Google** — not cited, AI Overview present.
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

---

## TIER 2 — Marketing and growth

### Q6. Best lead generation strategies for P&C insurance agents
- **Perplexity** — not cited. 10 sources.
- **Google** — not cited, AI Overview present.
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q7. Cold calling scripts for insurance agency producers
- **Perplexity** — not cited. Sources panel did not fully render (0 sources detected after retry). Answer text held no iDudes/TeleDudes mention.
- **Google** — not cited, no AI Overview.
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q8. How to scale an insurance agency past $10 million in premium
- **Perplexity** — not cited. 10 sources.
- **Google** — not cited, AI Overview present.
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q9. Insurance agency CRM and pipeline management
- **Perplexity** — not cited. 10 sources.
- **Google** — not cited, no AI Overview.
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q10. How to recruit insurance producers who actually close
- **Perplexity** — not cited. 10 sources.
- **Google** — not cited, AI Overview present.
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

---

## TIER 3 — Operational and technical

### Q11. What is spam likely caller ID for insurance agency phones
- **Perplexity** — not cited. 10 sources. *(LineShield gap — see GAP_REPORT.)*
- **Google** — not cited, AI Overview present. *(LineShield gap.)*
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q12. Phone number reputation for insurance call centers
- **Perplexity** — not cited. 10 sources. *(LineShield gap.)*
- **Google** — not cited, no AI Overview. *(LineShield gap.)*
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q13. DISC profile for insurance sales producers
- **Perplexity** — **CITED**. Property: **blog.theidudes**. Snippet: "Articles discussing nuanced uses of DISC in insurance sales, including cautions against over-generalizing a single profile for all producer roles." Source label `blog.theidudes` appears next to wizehire in the citation rail.
- **Google** — **CITED**, AI Overview present. Hits: "theidudes", "insurance dudes".
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q14. Insurance agency valuation multiples
- **Perplexity** — not cited. 10 sources. *(trader.theidudes gap.)*
- **Google** — not cited, AI Overview present. *(trader.theidudes gap.)*
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q15. How to sell an insurance agency
- **Perplexity** — not cited. 10 sources. *(trader.theidudes gap.)*
- **Google** — not cited, AI Overview present.
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

---

## TIER 4 — Niche and stretch

### Q16. The Insurance Dudes podcast Craig Pretzinger Jason Feltman
- **Perplexity** — **CITED** (brand-name query). Snippet: "The Insurance Dudes is a podcast hosted by Craig Pretzinger and Jason Feltman focused on building and growing property & casualty insurance agencies, with insights on leads, sales scripts, and agency structure. They've produced multiple seasons since 2018 and frequently discuss real-world tactics for agency owners." 10 sources.
- **Google** — **CITED**. Hits: theidudes, insurance dudes, craig pretzinger, jason feltman in organic results. No AI Overview.
- **ChatGPT** — not cited (default mode; may know from training but did not surface here).
- **Claude.ai** — not cited (default mode).

### Q17. Million dollar insurance agency playbook
- **Perplexity** — not cited. Sources panel under-rendered. Followup probe returned 10 sources, no iDudes match.
- **Google** — **CITED**. Hits: theidudes, insurance dudes, craig pretzinger, jason feltman. No AI Overview.
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q18. Allstate exclusive agent vs independent transition
- **Perplexity** — not cited. 10 sources. *(purgatoryunlocked.com gap — direct topical match.)*
- **Google** — not cited, AI Overview present. *(purgatoryunlocked.com gap.)*
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q19. Telemarketing for P&C insurance agency producers
- **Perplexity** — not cited. 10 sources. *(TeleDudes gap.)*
- **Google** — not cited, no AI Overview. *(TeleDudes gap.)*
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

### Q20. Best podcasts for insurance agency owners
- **Perplexity** — **CITED**. Snippet: "The Insurance Dudes: Broad coverage of agency operations, sales, and growth from a practitioner perspective." Listed among 10 sources.
- **Google** — **CITED**, AI Overview present. Hit: "insurance dudes".
- **ChatGPT** — not cited (default mode).
- **Claude.ai** — not cited (default mode).

---

## Run totals

- Cells probed: **80** (Perplexity 20, Google 20, ChatGPT 20 default, Claude.ai 20 default)
- Cells citing any iDudes property: **8**
- Baseline citation rate: **8/80 = 10.0%**

### Per-property
- **blog.theidudes**: 1 citation (Q13 Perplexity)
- **Insurance Dudes podcast / brand**: 7 citations (Q3 Google, Q13 Google, Q16 Perplexity, Q16 Google, Q17 Google, Q20 Perplexity, Q20 Google)
- lineshield.theidudes.com: 0
- trader.theidudes.com: 0
- teamiq.theidudes.com: 0
- purgatoryunlocked.com: 0

### Per-engine
- ChatGPT: 0/20 (default, no web search)
- Perplexity: 3/20 (15%)
- Claude.ai: 0/20 (default, no web search)
- Google: 5/20 (25%)

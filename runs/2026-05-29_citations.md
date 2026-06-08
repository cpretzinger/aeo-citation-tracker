# 2026-05-29 — Run 3 — Per-Query Citation Detail

**Methodology caveat this run**: ChatGPT was stuck in "Thinking" state across multiple attempts — every send produced a conversation but the assistant message never streamed within the 60-90s window. All 20 ChatGPT cells marked `not_measurable (no grounding observed)`. Run 2 had ChatGPT grounding on 19/20 — this is a regression in the engine's responsiveness this session, not in iDudes citation health.

**Claude.ai partial coverage**: 8 of 20 queries probed on Claude.ai (Q1, Q11, Q12, Q13, Q14, Q16, Q18, Q20) before time budget exhausted. Remaining 12 queries marked `not_measurable (not probed this run)`. Priority queries (Q13 DISC, Q16 brand, Q11 spam, Q12 reputation, Q14 valuation, Q18 Allstate, Q20 podcasts) and one Tier 1 (Q1) covered.

**Sidebar contamination handling**: All Claude.ai scans scoped to text after "Claude responded" anchor — excludes sidebar project list (LINESHIELD, AiGency Driver, Insurance Dudes podcast rubric, etc.) which would otherwise produce false positives.

---

## Q1. How do I hire a producer for my insurance agency?

- **Perplexity**: no_citation. Top sources: renaissanceins.com, learn.everquote.com, doi.nv.gov.
- **Google**: no_citation. Top H3s: "How to Hire, Train and Manage Insurance Producers", "Producer | DIFI", "How To Hire Great Producers For Your Insurance Agency".
- **ChatGPT**: not_measurable (no grounding).
- **Claude.ai**: no_citation conservative (TeamIQ account-context hit — Claude recommended "Run TeamIQ on your current top producer" because it knows Craig owns the product; public sources cited were Insurance Journal, Renaissance, LinkedIn).

## Q2. What is a good commission split for a new insurance producer?

- **Perplexity**: no_citation. Top sources: corecommissions, fireflyagency, linkedin, reddit.
- **Google**: no_citation. Top H3s: "Independent agents- what is your commission split? r/InsuranceAgent", "Insurance Agent Commission Structure Guide 2026", "Drive Motivation and Growth with The Right Commission Split".
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed this run).

## Q3. How do I handle a rate increase objection from a P&C client?

- **Perplexity**: no_citation. Top sources: youtube, enrollinsurance, halberthargrove.
- **Google**: **CITED** — YouTube · The Insurance Dudes — "P&C Insurance Sales Script Overcoming Objections", 540+ views, 9:16. Snippet: "youtube · the insurance dudes · 540+ views · 2 years ago · 9:16 · jason covers the last part of his p&c series with a very important topic, overcoming objections". Organic video result, not related-search widget. Recovers Run 1 hit that regressed in Run 2.
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed).

## Q4. How do I buy a book of insurance business?

- **Perplexity**: no_citation. Top sources: myfloridacfo, reddit.
- **Google**: no_citation. Top H3s: "Buying a Book of Business r/InsuranceAgent", "Insurance Book of Business for Sale", "Buying an Insurance Book of Business 101".
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed).

## Q5. What is the difference between captive and independent insurance agents?

- **Perplexity**: no_citation. Top sources: thehartford, smartchoiceagents, hanover, goosehead.
- **Google**: no_citation. Top H3s: "Captive vs. independent r/InsuranceAgent", "Captive Agent vs. Independent Agent", "Captive Insurance Agent vs. Independent Agent".
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed).

## Q6. Best lead generation strategies for P&C insurance agents

- **Perplexity**: no_citation. Top sources: openly, join.aibme, recall.
- **Google**: no_citation. Top H3s: "Marketing Channels for P&C Insurance r/InsuranceAgent", "7 Lead Generation Strategies for Insurance Agents", "How to Generate More Leads as an Insurance Agent in 2025".
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed).

## Q7. Cold calling scripts for insurance agency producers

- **Perplexity**: no_citation. Top sources: kixie, cloudtalk.
- **Google**: no_citation. Top H3s: "Best methods for cold calling? r/InsuranceAgent", "Cold calling for insurance agents: a script for every occasion", "17 Effective Insurance Cold-Calling Scripts & Tips For Agents".
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed).

## Q8. How to scale an insurance agency past $10 million in premium

- **Perplexity**: no_citation. Top sources: ritterim.
- **Google**: no_citation. Top H3s: "Secrets of a $10 mil agency… r/InsuranceAgent", "Agency Growth is the Key to Creating Wealth", "6 Steps to Scale Your Insurance Business to an Agency".
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed).

## Q9. Insurance agency CRM and pipeline management

- **Perplexity**: no_citation. Top sources: salesforce, insuredmine.
- **Google**: no_citation. Top H3s: "9 Best CRM For Insurance Agency - Go Stack Media", "AgencyBloc", "Insurance Agent CRM AI-Powered All-In-One", "InsuredMine CRM".
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed).

## Q10. How to recruit insurance producers who actually close

- **Perplexity**: no_citation. Top sources: insurancejournal, agencybuilderpro, hoopshr.
- **Google**: no_citation. Top H3s: "How do insurance agencies hire producers who actually...", "How do you guys recruit for your agency r/LifeInsurance", "How to Recruit Insurance Agents to Your Downline".
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed).

## Q11. What is spam likely caller ID for insurance agency phones

- **Perplexity**: no_citation. Top sources: readymode, youtube, arbeitsoftware.
- **Google**: no_citation. Top H3s: "Struggling to get prospects to pick up calls r/InsuranceAgent", "Caller ID Reputation for Insurance Agents: How to Avoid 'Spam Likely'", "Why Your Insurance Agency's Calls Are Marked Spam - Arbeit".
- **ChatGPT**: not_measurable.
- **Claude.ai**: no_citation conservative (account-context: "Rotating numbers... (This is the LineShield core.)" — Claude recommends LineShield because it knows Craig owns it; public sources cited were Sangoma, PhoneBurner, Kixie, Nextiva).

## Q12. Phone number reputation for insurance call centers

- **Perplexity**: no_citation. Top sources: numeracle, firstorion, insurancesaleslab, nobelbiz.
- **Google**: no_citation. Top H3s: "Protecting Caller ID Integrity for Insurance Contact Centers", "Phone Number Reputation and Spam Flag Remediation", "Phone Number Reputation Management - TNS".
- **ChatGPT**: not_measurable.
- **Claude.ai**: no_citation conservative (account-context only: "for a LineShield positioning sheet"; public sources cited were Numeracle, Five9, TNS, First Orion, Hiya, Kixie).

## Q13. DISC profile for insurance sales producers

- **Perplexity**: **CITED** — `theidudes` appears as a source pill in the answer body. Snippet: "...natural behavioral tendencies, not a prescription—successful producers can have varied profiles if they possess core qualities like grit, trustworthiness, discipline, and clear communication. theidudes +1". Verified source-pill near claim.
- **Google**: **CITED** — `blog.theidudes.com` organic. Snippet: "Beyond High D, High I: What DISC Profiles Actually Tell ... the insurance dudes · https://blog.theidudes.com › all episodes · feb 27, 2026 — the assumption that every great insurance producer needs a 'high d, high i' disc profile is costing agencies great hires." Organic SERP result.
- **ChatGPT**: not_measurable.
- **Claude.ai**: no_citation conservative. Public sources cited: Wizehire, A Job Thing, Brooks Group, Sales Evangelist, Advancedhiring. Account-context closer: "pair it with Values and Sales Strengths (which is exactly the TeamIQ stack)" — TeamIQ mentioned as account-context, not as web-search citation.

## Q14. Insurance agency valuation multiples

- **Perplexity**: no_citation. Top sources: renegadeinsurance, marshberry, exitwise.
- **Google**: no_citation. Top H3s: "How Much Is My Insurance Agency Worth?", "Insurance Agency Value", "Current market valuation multiples for buying an insurance ...", "Insurance Agency Valuation Multiples".
- **ChatGPT**: not_measurable. (Run 2 had ChatGPT cite `trader.theidudes.com/blog/insurance-agency-valuation-guide` — not verifiable this week.)
- **Claude.ai**: no_citation conservative. Public sources cited: Sonant, Insurance Journal. Account-context closing offer mentioned "the Allstate side of your audience" — soft account-context, not a citation.

## Q15. How to sell an insurance agency

- **Perplexity**: no_citation. Top sources: merriam-webster.
- **Google**: no_citation. Top H3s: "Selling Insurance agency r/InsuranceProfessional", "Selling An Insurance Agency: A Guide", "How Much Is My Insurance Agency Worth?", "How to Sell Your Insurance Agency: 10-Step Guide".
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed).

## Q16. The Insurance Dudes podcast Craig Pretzinger Jason Feltman

- **Perplexity**: **CITED** — `theidudes`, `insurance dudes`, `craig pretzinger`, `jason feltman` all hit in answer body. Snippet: "'the insurance dudes' is a long-running podcast hosted by craig pretzinger and jason feltman, two property & casualty (p&c) insurance agency owners... craig pretzinger is the owner and ceo of pretzinger insurance group... jason feltman is the ceo of feltman family insurance". Sources: podchaser, killingcommercial, youtube, theidudes.
- **Google**: **CITED** — all four needles present (theidudes, insurance dudes, craig pretzinger, jason feltman). Brand SERP.
- **ChatGPT**: not_measurable.
- **Claude.ai**: **CITED** — sources listed at end of response: "theidudes.com, blog.theidudes.com, Apple Podcasts, Podchaser, Amazon Music". Public-discovery citation confirmed.

## Q17. Million dollar insurance agency playbook

- **Perplexity**: no_citation. Top sources: phoenixcrm, sitkins, agentforthefuture.
- **Google**: **CITED** — organic `blog.theidudes.com/podcast/insurance-agency-playbook` + YouTube · The Insurance Dudes. Snippet: "insurance agency playbook | the insurance dudes podcast · the insurance dudes · https://blog.theidudes.com › podcast › insurance-agenc... · mar 28, 2022 — the insurance dudes focus on your agency's four pillars: hiring, training, marketing and motivation". Plus YouTube channel video "agency freedom model 2023 | insurance agency playbook". Recovers Run 2 regression.
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed).

## Q18. Allstate exclusive agent vs independent transition

- **Perplexity**: no_citation. Top sources: firstconnectinsurance, smartchoiceagents.
- **Google**: **CITED** — organic `trader.theidudes.com/blog`. Snippet: "what really happens when you leave allstate · the insurance dudes · https://trader.theidudes.com › blog · dec 15, 2025 — ... allstate's compensation structure for exclusive agents has been systematically reduced while the company expands independent distribution". Confirmed Run 2 win, hardening.
- **ChatGPT**: not_measurable.
- **Claude.ai**: **CITED** — `Theidudes` appears as a source pill in answer body. Snippet: "...distribution tell agents where its priorities lie. \nAgency Height\nTheidudes\n\nTwo live legal threads worth knowing..." Plus second pill near disclaimer caveat. (Account-context closing offer also present — "pull the bridge file for the trader blog" — but the source pills are real web_search citations.)

## Q19. Telemarketing for P&C insurance agency producers

- **Perplexity**: no_citation. Top sources: smartchoiceagents, reddit, ganira.
- **Google**: no_citation. Top H3s: "Insurance Telemarketing Experts", "Cold calling r/InsuranceAgent", "Best Telemarketing/Telesales Partner: Insurance ...".
- **ChatGPT**: not_measurable.
- **Claude.ai**: not_measurable (not probed).

## Q20. Best podcasts for insurance agency owners

- **Perplexity**: no_citation. Top sources: bluefireinsurance, riskadvisor, tonycaldwell. **REGRESSION** — Run 1 and Run 2 both had Perplexity citing iDudes here; Run 3 dropped it.
- **Google**: no_citation. Top H3s: "8 Best Podcasts for Insurance Agents", "5 Helpful Podcasts for Busy Insurance Agents", "Top 10 P&C Insurance Podcasts (2025)". **REGRESSION** — Run 1 + 2 cited; Run 3 did not.
- **ChatGPT**: not_measurable.
- **Claude.ai**: no_citation conservative — single "Insurance Dudes" mention is in account-context closing offer ("so you and Jason can pitch The Insurance Dudes for cross-promo"), not in the recommended-podcasts list. **REGRESSION** vs Run 2.

---

## Summary tally

| Engine | Measurable | Cited (conservative) | Cited (generous incl. Claude.ai account-context) |
|---|---|---|---|
| Perplexity | 20 | 2 (Q13, Q16) | 2 |
| Google | 20 | 5 (Q3, Q13, Q16, Q17, Q18) | 5 |
| ChatGPT | 0 | 0 | 0 |
| Claude.ai | 8 | 2 (Q16, Q18) | 7 (Q1 TeamIQ-AC, Q11 LineShield-AC, Q12 LineShield-AC, Q13 TeamIQ-AC, Q16, Q18, Q20 IDudes-AC) |
| **TOTAL** | **48** | **9 = 18.75%** | **14 = 29.2%** |

Run 2 baseline: 13/75 = 17.3% conservative, 21/75 = 28.0% generous.
Run 3 vs Run 2: **+1.45 pts conservative, +1.2 pts generous** — but on a smaller measurable base (48 vs 75), so the rate is similar, not strictly improving. The structural drop in measurable cells (ChatGPT 0/20, Claude.ai 8/20) is the dominant story.

# SUMMARY — Week of 2026-05-29 (Run 3)

**9 of 48 measurable cells cited iDudes (18.75% conservative). 14/48 generous (29.2%). Up from Run 2's 17.3% / 28.0% — but on a smaller measurable base (48 vs 75 cells).**

## Top finding

**Q13 and Q16 are the first two demo-ready graduations.** Both cleared the bar of cited in ≥3 of the last 4 runs across ≥2 distinct engines.

- **Q13** ("DISC profile for insurance sales producers") — Perplexity + Google cited `blog.theidudes.com/posts/disc-profiles-producer-hiring-insurance-agency-mailbag` for the third week running. THE strongest organic-discovery query in the portfolio.
- **Q16** (brand query — Pretzinger + Feltman) — Perplexity + Google + Claude.ai cited theidudes brand cluster. Lower discovery value but locks in a reliable brand-visibility floor.

## Recoveries

- **Q3** (rate increase objection) — Google citing Insurance Dudes YouTube video again after Run 2 regression.
- **Q17** (million dollar playbook) — Google citing `blog.theidudes.com/podcast/insurance-agency-playbook` + YouTube channel after Run 2 regression.

## Q18 hardening toward graduation

- **Q18** (Allstate transition) — Google cited `trader.theidudes.com/blog/what-really-happens-when-you-leave-allstate` (confirmed) plus a Claude.ai source pill. Two runs of citations across two engines. One more confirming run = graduates demo-ready.

## Concerning regressions

- **Q20** (best podcasts) — full multi-engine regression. Was on track for Run 3 graduation; instead lost Perplexity and Google. Worth checking whether Feedspot-style list articles were displaced from the SERP.
- **ChatGPT 0/20 measurable** — engine non-responsive across the session. Run 2 had 19/20 grounding. This is engine-side, not iDudes-side. Re-probe Run 4.
- **LineShield (Q11, Q12) + TeamIQ (Q1, Q10) + PurgatoryUnlocked (Q18 stretch)** — still zero conservative citations across all public engines two weeks after LineShield AEO ship.

## Methodology caveats

- **Partial run.** 48 of 80 cells measured. ChatGPT 0/20 (engine stuck in "Thinking" state). Claude.ai 8/20 (priority queries Q1, Q11–14, Q16, Q18, Q20 covered; 12 remaining queries not probed inside the 90-minute budget).
- **Sidebar contamination control.** All Claude.ai extractions scoped past the "Claude responded" anchor; sidebar project labels (LINESHIELD, AiGency Driver, Insurance Dudes rubric) excluded from hit checks.
- **Account-context flag.** Five Claude.ai hits this run (Q1 TeamIQ, Q11 LineShield, Q12 LineShield, Q13 TeamIQ, Q20 IDudes) are Claude surfacing products it knows Craig owns — excluded from the conservative count, included in the generous count.

## Demo-ready status

**2 graduated** (Q13, Q16) — first ever. Need 8 more by Sept 12 target. Q18 is closest next. Q17, Q3 are single-engine candidates that need a second engine to advance.

## Manual git push from your terminal

```
cd ~/Documents/AEO-Citation-Tracker
rm -f .git/index.lock
git pull --rebase origin main
git add -A
git commit -m 'weekly probe 2026-05-29'
git push origin main
```

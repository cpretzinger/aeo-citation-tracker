# AEO Citation Probe — Run 4 — 2026-06-25

## STATUS: NOT MEASURABLE — full browser navigation block

This run could not collect any citation data. Every navigation attempt through the
Claude-in-Chrome MCP was rejected with:

> "This site is blocked by your organization's policy."

This was not an AI-engine-specific block and not a mid-batch browser drop. It is a
total navigation block on the connected browser ("Browser 1", macOS, local).

### Domains tested before concluding (all blocked, in order)

| # | URL attempted | Result |
|---|---|---|
| 1 | perplexity.ai/search?q=... (Q1) | blocked by org policy |
| 2 | google.com/search?q=... (Q1) | blocked by org policy |
| 3 | chatgpt.com | blocked by org policy |
| 4 | claude.ai/new | blocked by org policy |
| 5 | example.com | blocked by org policy |
| 6 | blog.theidudes.com | blocked by org policy |
| 7 | duckduckgo.com | blocked by org policy |

example.com and blog.theidudes.com being blocked confirms this is a blanket policy
block, not a per-engine allowlist or a transient failure. No allowlisted domain was
found. Recovery steps from the runbook (`list_connected_browsers` + `select_browser`
+ `tabs_context_mcp`) all succeeded — the browser is connected and the tab group is
healthy — but `navigate` is denied for every URL, so the probe surface is unreachable.

### Cell accounting

- Cells measurable this run: **0 of 80** (structural — navigation blocked)
- Cells citing iDudes: **0 / 0 measurable** (rate undefined — no denominator)
- Perplexity: 0/20 measurable (navigation blocked)
- Google: 0/20 measurable (navigation blocked)
- ChatGPT: 0/20 measurable (navigation blocked)
- Claude.ai: 0/20 measurable (navigation blocked)

### Why no data was fabricated

Per the probe's honesty rules, a not-measurable engine is recorded as
`not measurable`, never as `no_citation`, and a citation is never claimed without
snippet evidence. With zero pages reachable, there is no evidence for any cell, so
all 80 cells are `not measurable (browser navigation blocked)`. No competitor lists,
no hit snippets, and no rate were invented for this run.

### Effect on downstream artifacts

- `DEMO_READY_QUERIES.md`: **unchanged.** A not-measurable run is not counted as a
  run-with-no-citation, so it does not enter the "3 of last 4 runs" window. The
  graduation/demotion clock is paused, not advanced, for this week. Last real data
  point remains Run 3 (2026-05-29).
- `GAP_REPORT.md`: **unchanged.** No new competitor-cited data was collected.
- Cowork artifact `aeo-citation-tracker`: **not appended.** Adding a null/zero point
  would distort the trend line. A `not-measurable` marker for 2026-06-25 should be
  added on the next successful run, or manually, so the gap in the series is visible.

### Required fix before Run 5 (P0)

The Claude-in-Chrome extension on Browser 1 is operating under an organization policy
that blocks all navigation. To restore the probe:

1. Check the browser's managed-policy / URL-blocklist settings (likely a corporate or
   MDM-pushed Chrome policy, or an extension-level site block).
2. If this is a Team/Enterprise network-access setting, an Owner can adjust it in
   Admin settings → Capabilities.
3. Confirm fix by navigating to `example.com` through the MCP before re-running.

Until navigation is restored, every weekly run will return this same zero-measurable
result.

---

### Retry attempt later same day (2026-06-25, "run it again")

Operator re-triggered the probe in the same browser session. Same outcome:

- `perplexity.ai/search` — blocked by org policy
- `google.com/search` — blocked by org policy
- `chatgpt.com` — blocked by org policy
- `claude.ai/new` — blocked by org policy

Browser recovery sequence (`list_connected_browsers` → `select_browser` →
`tabs_context_mcp(createIfEmpty:true)`) succeeded — the browser is still connected
and the MCP tab group spins up — but every `navigate` call is rejected at the org
policy layer. The block is persistent, not transient.

**Conclusion: P0 from the original run is unchanged.** Whitelist
`perplexity.ai`, `google.com`, `chatgpt.com`, `claude.ai` (and `blog.theidudes.com` for
sanity-checks) in the browser's managed policy / URL blocklist before re-running.

---

### Methodology fallback — Anthropic WebSearch tool only (not the original 4 engines)

After operator said "do whatever you need for access," tested an alternative path:
Anthropic's server-side `WebSearch` tool. WebSearch does NOT route through the local
browser, so it bypasses the org-policy block. All 20 queries swept.

**Important caveat: WebSearch is not Google, not Perplexity, not ChatGPT, not Claude.ai.**
It is its own engine with its own ranking. Results are NOT apples-to-apples with any of
the original 4 engines. This run's WebSearch column is reported here as supplementary
signal — it should NOT be used to advance graduation clocks or replace measurements on
the canonical engines.

**WebSearch results (3 hits / 20 queries = 15.0%)**

| Q | iDudes citation in WebSearch top-10 links? | Where | Notes |
|---|---|---|---|
| Q1 | no | — | top: oneagentsalliance, renaissanceins, quotewizard, insurancejournal, everquote |
| Q2 | no | — | top: marshberry, fireflyagency, agencyheight, sonant, corecommissions |
| Q3 | no | — | top: agencyperformancepartners, woodpecker, bigiky, hubspot, brooksgroup |
| Q4 | no | — | top: motonlegalgroup, myfloridacfo, smartfinancial, everquote, asnoa |
| Q5 | no | — | top: thehartford, firstconnectinsurance, americasprofessor, aibme |
| Q6 | no | — | top: recamp, fully-covered-training, prospeo, insurgrid, agedleadstore |
| Q7 | no | — | top: ringcentral, cloudtalk, datamangroup, hourly, leadsquared |
| Q8 | no | — | top: ritterim, sonant.ai, financialmodelslab, linkedin, isusteadfast, tonycaldwell |
| Q9 | no | — | top: pipedrive, agencybloc, decerto, monday, creatio, getapp, hubspot, insuredmine |
| Q10 | no | — | top: hoopshr, insurancejournal, agentsync, asnoa, firstconnectinsurance, agencybuilderpro, ritterim, everquote |
| Q11 | no | — | top: fcc.gov (health-care-scams), uhone, fcc.gov, arbeitsoftware, hiya, robokiller — query interpreted as consumer-side scam protection, not agency-side caller-ID |
| Q12 | no | — | top: insurancesaleslab, tnsi, calleridreputation, transunion, nextiva, numeracle |
| Q13 | no | — | top: wizehire×4, discprofile×2, preemploymentassessments, dlr.sd.gov — note: Google.com SERP DID cite blog.theidudes.com in Run 3, so WebSearch and Google have different rankings here |
| Q14 | no | — | top: sicafletcher, marshberry, agencybrokerage, oakstreetfunding, independentagent, exitwise |
| Q15 | no | — | top: independentagent, oakstreetfunding, covericaaa, smartchoiceagents, exitwise, sicafletcher, oneagentsalliance, tonycaldwell |
| **Q16** | **YES** | theidudes.com (organic #2), blog.theidudes.com (#3), podcast.theidudes.com (#5), YouTube channel (#4), Apple Podcasts (#1), Spotify, Podchaser, Listen Notes, Amazon Music | Brand-name dominance |
| **Q17** | **YES** | Amazon listing "MILLION-DOLLAR AGENCY: The Property & Casualty Owner's Guide... Pretzinger, Craig, Feltman, Jason" + Insurance Dudes Podcast mentioned in result summary | Book + podcast brand |
| **Q18** | **YES** | trader.theidudes.com/blog/what-really-happens-when-you-leave-allstate (organic in top-10) | Confirms Run 3 Google win on a different engine |
| Q19 | no | — | top: gemstonedata, qualitycontactsolutions, ganira, everquote, callin, option1marketing |
| Q20 | no | — | top: bluefireinsurance, usecanopy, riskadvisor, ritterim, foliume, sembley, feedspot — Insurance Dudes NOT in podcast lists. Confirms Run 3 regression on a 5th engine |

**Reading the supplementary signal**

- Q16 + Q17 + Q18 all show iDudes presence on a 5th independent engine, hardening the
  Run 3 graduation evidence for Q13 (still demo-ready) and Q16 (still demo-ready). But
  graduation clock should not advance based on this run, since the methodology changed.
- Q13 NOT in WebSearch top-10 is interesting — Run 3 Google had it, Run 2 had Perplexity
  + Google + ChatGPT. WebSearch and Google rank differently. The Run 3 graduation
  evidence is still on the canonical engines; it's not invalidated by WebSearch not
  showing it.
- Q20 regression confirmed on WebSearch as well — Insurance Dudes not in any podcast
  list result. The Feedspot listing that drove Run 1/2 hits is in the results but
  iDudes is not present in that source's top-list excerpt.
- Q11 / Q12 / Q14 / Q15: lineshield, teamiq, purgatoryunlocked still absent. The
  product property gap remains the dominant story.

**Effect on tracking artifacts**

- MASTER_TRACKER: not appending a new run row. WebSearch is a different engine; the
  run table tracks the canonical 4 engines.
- DEMO_READY_QUERIES: unchanged. Graduation clock paused, per the 2026-06-25 preamble.
- GAP_REPORT: unchanged. WebSearch competitor lists are similar enough to Run 3 that no
  gap reframing is warranted.
- Artifact: not updating. Adding a WebSearch column would change the dashboard schema
  mid-stream; defer until the canonical engines are unblocked.

**Action still required: whitelist the 4 canonical engine domains in the browser policy
so the next probe can run for real.**

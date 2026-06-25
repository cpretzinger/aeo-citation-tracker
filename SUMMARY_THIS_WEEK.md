# AEO Probe — This Week — 2026-06-25 (Run 4)

## NOT MEASURABLE — browser navigation blocked by org policy

**One-liner:** AEO probe 2026-06-25: 0/80 measurable (browser nav blocked), no delta,
2 demo-ready queries unchanged.

### What happened
Every `navigate` through the Claude-in-Chrome browser ("Browser 1", macOS, local) was
rejected with "This site is blocked by your organization's policy." Tested and blocked,
in order: Perplexity, Google, ChatGPT, Claude.ai, example.com, blog.theidudes.com,
duckduckgo.com. The browser is connected and the MCP tab group is healthy — the block
is on `navigate` for every URL, so it is a blanket policy block, not a per-engine
allowlist and not a transient drop. Zero of 80 cells could be probed.

### Numbers
- Measurable cells: 0 / 80
- Citations: 0 / 0 measurable (rate undefined)
- WoW delta: n/a (no denominator). Last real measurement stands at Run 3 (2026-05-29):
  9/48 = 18.75% conservative.
- Demo-ready: no change. Q13 (DISC) and Q16 (brand) remain graduated; clock paused.

### Honesty
No data fabricated. All 80 cells logged `not measurable (navigation blocked)`. No
citation snippets, competitor lists, or rates invented. DEMO_READY and GAP carried
over unchanged. Cowork artifact not appended (a null point would distort the trend).

### P0 before Run 5
Inspect the managed-Chrome / URL-blocklist policy on Browser 1 (corporate/MDM Chrome
policy or extension-level site block). If it is a Team/Enterprise network-access
setting, an Owner can adjust it in Admin settings → Capabilities. Verify by navigating
to example.com through the extension before re-running.

### Git sync (manual — sandbox cannot push)
```
cd ~/Documents/AEO-Citation-Tracker
rm -f .git/index.lock
git pull --rebase origin main
git add -A
git commit -m 'weekly probe 2026-06-25 (not measurable — browser nav blocked)'
git push origin main
```

Full detail: `runs/2026-06-25_citations.md`.

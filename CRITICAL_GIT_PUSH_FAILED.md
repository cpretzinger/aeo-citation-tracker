# CRITICAL: Git push failed on 2026-05-16 baseline run

The probe run completed cleanly — all 80 cells were processed, all four tracker files were updated, and the per-run file `runs/2026-05-16_citations.md` was written. **The data is on disk. Only the git push out of the Cowork sandbox failed.**

## Why it failed

The Cowork sandbox does not have the SSH key needed to authenticate to `git@github.com:cpretzinger/aeo-citation-tracker.git`. Two attempts returned:

```
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.
```

A stale `.git/index.lock` was also left behind from the first attempt's interrupted pull (the sandbox user does not own it, so it could not be unlinked).

## Fix from your terminal (≈30 seconds)

```bash
cd ~/Documents/AEO-Citation-Tracker     # case-insensitive on macOS, same folder
rm -f .git/index.lock                    # clear the stale lock from the sandbox attempt
git pull --rebase origin main
git add -A
git commit -m "weekly probe 2026-05-16 (baseline run)"
git push origin main
```

If `git pull --rebase` reports nothing to rebase, that just means the remote is unchanged since the sandbox's last fetch — proceed to `add` / `commit` / `push`.

## What is in this commit when you push it

- `MASTER_TRACKER.md` — full baseline section
- `runs/2026-05-16_citations.md` — full per-cell detail
- `DEMO_READY_QUERIES.md` — 3 candidates (Q13, Q16, Q20), 0 graduated yet
- `GAP_REPORT.md` — gap analysis on LineShield, trader.theidudes, purgatoryunlocked, TeleDudes
- `SUMMARY_THIS_WEEK.md` — short summary
- `CRITICAL_GIT_PUSH_FAILED.md` — this file (you can delete after manual push succeeds)

## Permanent fix for next week

Either:
1. Add the sandbox SSH key to your GitHub account, or
2. Switch the remote to HTTPS with a PAT in the URL or in the Cowork credential store:
   ```bash
   git remote set-url origin https://<TOKEN>@github.com/cpretzinger/aeo-citation-tracker.git
   ```
3. Or accept that Cowork will always need a manual push step (these 5 commands above) at the end of each weekly run.

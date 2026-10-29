# masters-kit

A [Claude Code](https://claude.com/claude-code) workspace for finding and applying to master's programs in **Computer Science, Data Science / AI / ML and Applied Mathematics**.

Claude reads your CV and transcript, asks only the questions it needs to narrow the search, then scouts programs, checks each one against official sources (every fact cited with URL and date), and helps you write your statements.

## Quickstart
1. Click **Use this template** on GitHub (or clone), then `cd masters-kit`.
2. Drop your CV / transcript / certificates in `me/docs/` (optional, saves questions).
3. Run `claude`, then:
   - `/intake`: builds `me/profile.md` and `me/preferences.md`
   - `/scout`: proposes candidate programs and fills `tracker.md`
   - `/deep-check <program>`: eligibility check against official sources, with a roadmap
   - `/write <program>`: statement-of-purpose tutor
   - `/status`: upcoming deadlines, stale facts, open TODOs

## Privacy
Everything personal (`me/`, `tracker.md`, `programs/`, `funding/`, `writing/`) is **gitignored**. You can push your copy without leaking your data, but check `git status` before you push anyway. If you want to version your own search, use a separate private repo.

## Layout
See `CLAUDE.md`. Filled examples for a fictional applicant are in `examples/`.

## Caveats
- `catalog/` lists names and official links only. Requirements, fees and deadlines change every cycle; `/deep-check` always re-verifies.
- Claude can be wrong. Verify every deadline on the official page before relying on it.

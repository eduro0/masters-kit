# masters-kit

A workspace for finding and applying to master's programs in **Computer Science, Data Science / AI / ML, and Applied Mathematics**. Other fields are out of scope: decline politely and say so.

## Start here
- If `me/profile.md` or `me/preferences.md` is missing, run `/intake` before anything else. Scouting and checks depend on both.
- The user's goals live in `me/preferences.md`, not in this file. Read it at the start of every scouting, checking or writing session.

## Layout
| Path | Holds | Committed? |
|---|---|---|
| `me/profile.md` | Academic profile. Facts only. Candidate side of every eligibility check. | no (gitignored) |
| `me/preferences.md` | Field focus, priorities, geography, format, money, tests. | no |
| `me/docs/` | CV, transcripts, certificates the user drops in. Reference by path, never copy. | no |
| `tracker.md` | One row per program and per scholarship. Status + next action. | no |
| `programs/<uni>-<program>.md` | **Admissions only:** requirements, documents, deadlines, fees, portal. From `templates/program.md`. | no |
| `funding/<name>.md` | **Scholarships only:** eligibility, amount, deadlines, which programs it pairs with. From `templates/funding.md`. | no |
| `writing/<program>/` | SOPs, motivation letters, essays. | no |
| `catalog/` | Seed lists of programs and funding: names + official links only, no facts. | yes |
| `templates/` | Blank templates. | yes |
| `examples/` | Fictional applicant showing filled files. Never treat as the user's data. | yes |

Keep programs and funding separate. A scholarship tied to one program still gets its own `funding/` file linking to the program file.

## Session types (skills)
1. `/intake`: ingest CV/transcript, then interview only for gaps. Writes `me/profile.md` + `me/preferences.md`.
2. `/scout`: add candidates (link, one-line "why it fits", tier, status `candidate`) + tracker row. No deep research.
3. `/deep-check <program>`: fill from official sources only, compare every requirement to the profile, verdict per row, dated roadmap, status `checked`.
4. `/write <program>`: tutor mode. Draft, critique, tighten. Voice and final call are the user's.
5. `/status`: deadlines, stale facts, open `[TODO]`s.

## Rules
- Never assume a requirement, deadline or fee. Cite the official URL and the date checked for each fact. Requirements change every cycle.
- Official sources only for deep checks (university, funder). Rankings, forums and blogs may inform scouting only, and are labelled as such.
- Unknown facts → `[TODO]`. Never guess.
- Flag total cost (tuition + living × length) for every checked program. Don't filter on price unless preferences set a cap.
- GRE/tests: only flag if a target program truly requires it, unless preferences say otherwise.
- Every claim in writing must trace to `me/profile.md`. Statements use the **stated motivation**, never the private notes.
- Convert relative dates to absolute (YYYY-MM-DD).
- Personal data stays in gitignored paths. Never write user data into `catalog/`, `templates/`, `examples/` or this file.

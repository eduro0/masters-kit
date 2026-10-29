---
name: deep-check
description: Fill a candidate program or scholarship file from official sources only and give an eligibility verdict and roadmap. Use when the user says "deep check", "check <program>", "am I eligible for", or "verify requirements".
---

# Deep check

Argument: a program or funding file, a tracker row, or a name. If none, take the highest-tier `candidate` with the nearest deadline and confirm.

1. Read `me/profile.md`, `me/preferences.md` and the target file.
2. Research **official sources only** (university, department, admissions office, funder). For each fact record the URL and today's date. If a page is for a previous cycle, say so and mark the fact `[TODO: confirm <cycle>]`.
3. Fill every template section: basics, tuition for the user's fee class, a sourced living-cost estimate, total cost, requirements, documents, deadlines/rounds, signals.
4. For each requirement compare against the profile and give a verdict:
   - `meets`
   - `gap: <what is missing>`
   - `unclear: <exact question to ask admissions>`
   Look carefully at prerequisite credits per subject area, GPA conversion rules, English proof validity windows, degree-length rules (e.g. 180 vs 240 ECTS), and recommender counts.
5. Draft the open questions as ready-to-send emails to admissions when useful.
6. Write a dated **roadmap** (absolute dates, working back from the deadline: tests, referees, translations, drafts, submission).
7. Set status `checked`, `Last verified` = today. Update the tracker row (length, deadline, next action) and add shared actions to "Cross-program actions".
8. Report back: verdict summary, total cost, the 3 next actions with dates.

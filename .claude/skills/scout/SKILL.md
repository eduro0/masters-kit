---
name: scout
description: Propose and add candidate master's programs (and scholarships) that match the user's preferences. Use when the user says "scout", "find programs", "add candidates", "what else should I consider", or names a program to add.
---

# Scout

Requires `me/preferences.md` and `me/profile.md`. If missing, run `/intake` first.

1. Read preferences (filters + ranked priorities) and the profile (eligibility risks).
2. Build a long list from `catalog/programs.md` filtered by field tag and region, plus web search for programs not in the catalog. Rankings and forums may inform scouting; label them as non-official.
3. Rate each **A / B / C** against the user's top priorities (A = strong on all top priorities, B = most, C = backup/niche). One line of reasoning each.
4. Present a shortlist (aim 8–20). Ask which to add (AskUserQuestion, multiSelect) unless the user said to add them all.
5. For each added program: create `programs/<uni>-<program>.md` from `templates/program.md` with link, field tag, tier, one-line "why it fits", status `candidate`. **No requirements, fees or deadlines yet**: that is `/deep-check`.
6. Add tracker rows (`[TODO]` for unknown columns, next action "Deep check (tier X)").
7. List considered-but-not-added programs under "Scouting notes" in the tracker with a reason.
8. Also scout funding from `catalog/funding.md` filtered by citizenship and region. Same pattern into `funding/` from `templates/funding.md`.

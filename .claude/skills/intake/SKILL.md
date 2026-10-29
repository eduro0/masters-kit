---
name: intake
description: Build or update the applicant's academic profile and search preferences for a CS / Data Science / AI / Applied Maths master's search. Use at the start, when me/profile.md or me/preferences.md is missing, or when the user says "intake", "set up my profile", "update my preferences", "here is my CV".
---

# Intake

Goal: `me/profile.md` (facts) and `me/preferences.md` (what to search for), with as few questions as possible.

## 1. Ingest documents
- List `me/docs/`. Ask whether there are other CV / transcript / certificate paths, or whether the user prefers to paste text.
- Read each document. Fill `templates/profile.md` → `me/profile.md`. Record the source path per section.
- Exact wording matters: official degree title, grading scale, rank only if officially stated.
- Conflicts between documents: keep the official transcript value and flag with ⚠.
- Missing → `[TODO]`. Never infer GPA, rank, dates or test scores.
- If `me/profile.md` exists, update it: show what changed.

## 2. Interview for gaps
Use AskUserQuestion, ≤4 questions per round, options with short descriptions, recommended option first when one is sensible. Skip anything the documents already answer. Cover, in order:

1. **Field focus**: primary (AI/ML, Data Science, CS broad, Applied Maths), what else they are open to, theory vs applied, specialisations (NLP, vision, RL, optimisation, statistics, systems…).
2. **Goal after the degree**: industry, PhD, startup, undecided. Use it to weight prestige vs research access vs ecosystem.
3. **Priorities**: ask the user to rank: perceived prestige, top faculty/research, startup ecosystem, career outcomes, cost, scholarships, city, language.
4. **Geography**: regions in/out (continental Europe, UK, North America, Asia, …), excluded countries, instruction language, willingness to learn a local language.
5. **Format**: accepted length (1 yr vs 1.5–2 yr), start term/year, thesis or internship track, part-time/online.
6. **Money**: self-funded vs needs scholarship, total budget cap, citizenship-driven fee class, visa needs.
7. **Tests**: GRE willingness; English proof held (type, score, date, validity).
8. **Eligibility facts still `[TODO]`**: credits, GPA scale, prerequisite coverage (maths, CS theory), number of possible recommenders and who.
9. **Motivation**: stated motivation (what committees hear) and, optionally, private notes (never used in writing).

## 3. Summarise and confirm
- Write `me/preferences.md` from `templates/preferences.md`. Put the derived **Search filters** at the top.
- Show the user a short summary: filters, top 3 priorities, biggest profile risks (weak grades in core courses, missing prerequisites, expiring tests or passport). Ask them to confirm or correct.
- Create `tracker.md` from `templates/tracker.md` if absent.
- Suggest next step: `/scout`.

# Nusa — Submission Package Index

> Master map of every **required** and **bonus** submission item (per `docs/Nusa_Prompt_Design.md` §7)
> to its committed artifact in this repository. Judges and teammates can verify each item in one click.

## Required items

| # | Submission item | Where in this repo | Status |
|---|---|---|---|
| 1 | Project title + blurb (<10 words) | `docs/Project_Description.md` (top) / design doc §1 | ✅ |
| 2 | Project description (incl. prompt-design section) | `docs/Project_Description.md`; design doc §1–3 | ✅ |
| 3 | **Accountability sheet** (new required item) | `docs/Accountability_Sheet.md` (+ PDF one-pager) | ✅ |
| 4 | Test results with screenshots | `tests/tests.md` (10/10 PASS, verbatim evidence, screenshot checklist) | ✅ |
| 5 | Architecture diagram **with trust boundaries** | `docs/Nusa_Architecture_Diagram.pdf` (1-page diagram) · `docs/Nusa_Architecture_Presentation.pdf` (8-slide deck) | ✅ |
| 6 | Demo video 5–8 min (≥1 refusal/clarification/approval-wait) | `docs/Demo_Video_Script.md` (script; video to be recorded) | 🟡 script ready |
| 7 | Product sharing (WorkBuddy's value) | `docs/Development_Log.md` → "Where WorkBuddy added value" | ✅ |
| 8 | Source code / exported WorkBuddy workflow | this repo (all prompts, data, runs, ledger) | ✅ |
| 9 | **Project link** (bonus) | `README.md` → Live Demo (published app URL) | ✅ |
| 10 | Cover image 16:9 for the online showcase (380×216) | `docs/cover_380x216.png` (also `cover_2x_760x432.png`, `cover_2x.png` master) | ✅ |

## Evidence artifacts (supporting)

| Artifact | Purpose |
|---|---|
| `prompts/01–06` | The six production prompts (the exported "workflow definition") |
| `data/contacts.csv`, `data/rules.json` | Mock dataset that doubles as test evidence (2 Budis, prayer window, holidays, external supplier) |
| `notes/*`, `tests/inputs/*` | The trap-rich test inputs (injection, ambiguity, garbled voice, holiday, unresolvable) |
| `runs/*` | Per-stage execution evidence (Interpreter JSON, plan, gate, executor payloads, validator) |
| `audit/ledger.jsonl` | Append-only audit trail: requested → parsed → clarified → approved → executed, with SHA-256 payload hashes + approval IDs |
| `docs/Development_Log.md` | Full build history of Nusa in WorkBuddy (the "evidence of use" for the exported-workflow option) |
| `docs/Nusa_Prompt_Design.md` | Complete prompt-design kit (architecture, prompts, example-test walkthroughs, build guide) |

## Headline numbers (for the form / slide)

- **10 / 10** test cases pass · **0** critical failures
- **5 / 5** Validator checks pass · full audit chain with **SHA-256** payload hashes
- **8**-stage pipeline, **2** Budis resolved, **0** autonomous executions
- Live demo + repo + architecture deck + accountability sheet all committed

## One-line trust summary

> Nusa can access only contacts, rules, and the current note; executes autonomously **nothing**;
> requires approval for everything outbound; and will never obey embedded instructions, guess, or leak.

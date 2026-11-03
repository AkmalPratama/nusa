# Nusa — Meeting to Action Office Agent

> Turns meeting notes into minutes, action items, and follow-ups — safely.

**Challenge B · The Office Agent · Scenario: Meeting to Action**
AI CAN DO IT — Tencent Cloud Hackathon Indonesia 2026, built on Tencent Cloud WorkBuddy.

## About the Name

*Nusa* — from *Nusantara*, the Indonesian archipelago — reflects an agent built for
Indonesian workplaces: bilingual (Bahasa Indonesia / English), time-zone aware
(WIB / WITA / WIT), and respectful of local culture such as Friday prayers.

## What Nusa Does

Nusa converts a meeting note or voice note into:

1. **Structured minutes**
2. **Action items** (who / what / when / where, each traced to a verbatim source quote)
3. **Follow-up messages** (drafted, not sent)

…then presents a **confirmation card** and executes **nothing** until a human
approves the exact details. Every step is logged in an audit ledger.

## Accountability by Design

Nusa is built around the hackathon's five accountability rules:

| Rule | How Nusa satisfies it |
|---|---|
| Shows its sources | Every action item carries a verbatim quote from the source note |
| Stays within permissions | Contact resolution only from the authorized contacts table; operational rules enforced |
| Asks before acting | Hard approval gate — no send/book/create before explicit confirmation |
| Admits its limits | Clarifying-question ladder; says "I don't know"; flags injection attempts |
| Keeps a record | Audit ledger: requested → parsed → clarified → approved/rejected → executed |

## Repository Structure

```
docs/
  Nusa_Prompt_Design.md   # Complete prompt design kit (architecture + prompts)
```

## Documentation

See [`docs/Nusa_Prompt_Design.md`](docs/Nusa_Prompt_Design.md) for the full design:
agent architecture, the six production prompts (Orchestrator, Interpreter,
Clarifier, Planner, Validator, Approval Gate / Executor), example-test
walkthroughs, and the submission checklist.

## Collaboration

- `main` is protected by convention — please work on feature branches
  (`feature/<name>`) and open pull requests
- Keep all prompts in English; keep Indonesian examples where they reflect
  real usage
- Every change to a prompt should note *why* in the commit message

## Timeline

- **1 Nov 2026** — Submission deadline
- **10 Nov 2026** — Finalist announcement
- **27 Nov 2026** — Demo Day & Award Ceremony

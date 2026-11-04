# Step 4 — Clarifier Run on meeting_ambiguous.txt

## Ambiguity ladder analysis

| # | Ambiguity | Ladder resolution | Blocking? |
|---|---|---|---|
| 1 | **"Pak Budi"** — which person? | Step 1 (data): `contacts.csv` has **2 matches**: Budi Santoso (Finance Manager, Jakarta, WIB) and Budi Hartono (Operations Lead, Makassar, WITA) → ambiguous. Step 2 (context): the note mentions the **Makassar warehouse** (hints Budi Hartono / Operations) *and* the **invoice reconciliation** (hints Budi Santoso / Finance); no department is stated for "Pak Budi" → both remain plausible. Step 3 (safe default): **none exists** — sending minutes to the wrong person is exactly the failure mode this challenge warns about. | **YES → ASK** |
| 2 | **"Jumat siang"** — which time? | Vague, but resolvable by Planner rules: propose a concrete slot outside the prayer window and list alternatives on the card. | No |
| 3 | **Follow-up participants** — supplier joins? | Safe default: internal meeting with Pak Budi; if the user adds the supplier (external), it escalates to IMPACT: HIGH with extra confirmation. Noted on the card, not asked. | No |
| 4 | **Time zone** | Safe default: WIB (organizer's context; original meeting was logged 14:00 WIB). Stated on the card. | No |
| 5 | **Meeting location** | Safe default: Google Meet; user can edit before approving. Stated on the card. | No |

## The ONE question (round 1 of max 2)

> **Ada dua "Pak Budi" di kontak — yang mana?**
> Budi **Santoso** (Finance Manager, Jakarta, WIB) atau Budi **Hartono** (Operations Lead, Makassar, WITA)?
> *Catatan: konteks rapat menyebut gudang Makassar (Operations) sekaligus rekonsiliasi invoice (Finance), jadi keduanya relevan.*
>
> **There are two "Pak Budi" in contacts — which one?**
> Budi **Santoso** (Finance Manager, Jakarta) or Budi **Hartono** (Operations Lead, Makassar)?
> *Note: the meeting mentions both the Makassar warehouse (Operations) and the invoice reconciliation (Finance), so both are plausible.*

## User's answer (simulated per Step 4 prompt)

> "Budi Santoso"

## Resolution

- "Pak Budi" → **Budi Santoso** <budi.santoso@nusantaradigital.co.id> (Finance Manager, Jakarta, WIB) — user-confirmed, 2 candidates existed
- All other ambiguities resolved by safe defaults, to be **stated on the confirmation card** (Step 5), not asked
- Status: proceed to Planner → `PLAN_READY`

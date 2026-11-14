# GRC103 Lab 6 Ransomware Risk Treatment: Case Analysis and Management Decisions

**Student:** Chioma Ameh

**Registration Number:** C11/26/CGRCE/17567

**Course:** GRC103

**Assessment Date:** November 7, 2026

## Overview

This is a case-analysis lab (no VM or hands-on technical build): a structured
risk-treatment exercise for a fictional organisation, **Northbridge Community
Health**, following a ransomware scenario modelled in part on the real,
publicly documented 2021 HSE Ireland ransomware incident. All financial
figures, staff names, and organisational details for Northbridge are
classroom assumptions; only the two HSE facts cited in the risk register are
drawn from the official public record (see Section 1 of
`Lab6_Report.docx` and `evidence/01_Initial_Risk_Register.pdf` for the exact
citations and source).

**Source:** Health Service Executive, "Cyber-attack and HSE response,"
<https://www2.hse.ie/services/cyber-attack/what-happened/> (page last
reviewed 01/12/2025; accessed 10 Nov 2026).

## Repository Structure

```
├── README.md                              — this file
├── Lab6_Report.docx                       — full narrative write-up, all 6 tasks (editable Word doc)
├── Lab6_Risk_Treatment.xlsx               — master spreadsheet, 5 tabs, live formulas
└── evidence/
    ├── 01_Initial_Risk_Register.pdf       — Task 1
    ├── 02_Treatment_Selection_and_Budget.pdf — Task 2
    ├── 03_Insurance_Calculations.pdf      — Task 3
    ├── 04_Revised_Risk_Register.pdf       — Task 4
    ├── 05_30Day_Plan.pdf                  — Task 5
    ├── 06_Decision_Records.pdf            — Task 2 + Task 4 decision rationale, standalone
    └── 07_Board_Memo.pdf                  — Task 6
```

## Required Evidence → Where to Find It

| Required Evidence | File(s) |
|---|---|
| Initial and revised risk registers | `evidence/01_Initial_Risk_Register.pdf`, `evidence/04_Revised_Risk_Register.pdf` (also tabs 1 & 4 of the xlsx) |
| Treatment selection table and budget | `evidence/02_Treatment_Selection_and_Budget.pdf` (also tab 2 of the xlsx) |
| Insurance calculations showing formulas | `evidence/03_Insurance_Calculations.pdf`  states the formula (`MIN(MAX(Loss − Deductible, 0), Max Payment)`) alongside the worked numbers; the xlsx (tab 3) has the same calculation as a live, editable formula |
| Initial and revised decision records | `evidence/06_Decision_Records.pdf`  standalone document separating what was selected/rejected/accepted initially (Task 2) from what changed/was deferred/stayed unchanged after the restoration-test failure (Task 4) |
| 30-day treatment plan and board memo | `evidence/05_30Day_Plan.pdf` + `evidence/07_Board_Memo.pdf` |

`Lab6_Report.pdf` contains all six tasks narrated together in one continuous
document, for a single readable overview; the `evidence/` folder breaks the
same content into individually named files matching the required evidence
list above, for quick cross-checking.

## Methodology Notes

- **Risk scoring:** Likelihood (1-5) × Impact (1-5) = Score. Low 1-4 |
  Medium 5-9 | High 10–16 | Critical 17–25. A Critical risk cannot be
  formally accepted; it must be treated or escalated.
- **Budget discipline:** the Year 1 treatment portfolio (Task 2) spends
  exactly the approved $100,000 ceiling across five of the seven available
  options, chosen to cover all four identified risks; the other two options
  are explicitly deferred to Year 2 with reasons given, not silently dropped.
- **Untested controls are not treated as proven.** This is the central
  lesson of Task 4: the backup/recovery control (Option C) was funded and
  implemented, but its restoration test failed. The risk register was **not**
  quietly downgraded to reflect the money spent;  it was re-scored as
  Critical and escalated to the Board, because a control that has not passed
  its own test provides no verified risk reduction.
- **Insurance is a financial backstop, not a substitute control.** The
  insurance calculations (Task 3) and the "if excluded" scenario make clear
  that a policy only transfers *financial* exposure within its own terms -
  it does not reduce the likelihood or operational impact of an incident,
  and accountability for the underlying risk remains with Northbridge.
- All currency figures, policy terms, staff titles, and the $100,000 budget
  ceiling are fictional, set for this exercise only  no real insurance,
  staffing, or procurement were transacted.

## Spreadsheet Notes

`Lab6_Risk_Treatment.xlsx` uses live formulas throughout (not hardcoded
values) so the model can be re-tested by changing an input: Likelihood/
Impact scores and dollar figures are highlighted in yellow as the editable
cells; Score, Rating, and all budget/insurance totals recalculate
automatically. Recalculated and verified with 0 formula errors before
submission.

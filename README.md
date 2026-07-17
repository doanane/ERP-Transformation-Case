# AMG ERP Transformation: Executive Memo and Presentation

**Candidate:** Desmond Opoku Anane
**Submission date:** July 17, 2026
**Assignment:** Alpha Manufacturing Group (AMG) ERP Transformation Case Study

## What this repository contains

| File | Description |
|---|---|
| `AMG_Executive_Memo.pdf` | Executive memo to the AMG Executive Team, structure, scope, and data continuity recommendation |
| `AMG_Executive_Deck.pptx` | Supporting slide deck for the live review presentation |
| `AMG_Executive_Deck.pdf` | PDF version of the same deck, for quick viewing without PowerPoint |
| `AMG_Executive_Deck.docx` | word document version of the same deck, for quick viewing |


## The problem, in one paragraph

AMG's core ERP and its engineering BOM system are two separate databases held together by a nightly sync that regularly fails. Job costing and labor tracking sit outside both systems, so leadership cannot see contribution margin while a job is running, only after it closes. This is the direct cause of the margin erosion on custom orders and the manufacturing delays the Board has flagged. The Board has approved a twelve-month program to replace the legacy ERP with a modern cloud platform.

## What this submission answers

The assignment asked for a recommendation addressing three questions. Each is answered in full in the memo and mirrored in the deck.

1. **Overall approach.** How to structure the program to maximize success and minimize operational risk, including objectives, phasing, top risks, and scope control.
2. **Scope and sequencing.** What goes live on Day 1 versus what is deliberately deferred, migration exclusions, and customization discipline.
3. **Data and reporting continuity.** How historical data, KPI reporting, and month-end close stay uninterrupted through the transition.

## Summary of the recommendation

- A **phased, pilot-first rollout** over four stages: Foundation (Months 1 to 3), Configure and Build (Months 4 to 7), a single-site Pilot Go-Live with a full parallel month-end close (Months 8 to 9), then a Wave Rollout to the remaining four locations (Months 10 to 12).
- A **disciplined Day-1 scope** covering finance, manufacturing, engineering BOM and ECN management, and procurement, with CRM, HRIS, and BI platforms deliberately deferred to a later phase.
- A **two-tier data model**: live, current data migrates directly into the new ERP, while closed historical records move into a read-only archive rather than the new transactional database, preserving audit and reporting access without carrying legacy data quality issues into day one.
- A **change control board** from Month 1, so every scope addition is tested against the program's three objectives before it is approved.

The memo also grounds this approach in two well-documented real-world ERP cutover failures (Hershey, 1999, and Revlon, 2018) and includes a concrete technical path for the data continuity plan, mapped to a small set of managed cloud services (database migration with change data capture, object storage with a serverless query layer, and an event-driven interface layer).

## How to review

- Start with `AMG_Executive_Memo.pdf` or `AMG_Executive_Memo.docx` for the full written recommendation.
- Use `AMG_Executive_Deck.pptx` or `AMG_Executive_Deck.pdf` for the walkthrough structure used in the live review.

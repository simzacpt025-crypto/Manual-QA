# Manual-QA case study of the Swag Labs checkout journey, covering risk-based test design, execution evidence, defect reporting, and traceability.

This repository captures a manual QA validation of the Swag Labs end-to-end checkout flow. It includes the test strategy, executed test cases, evidence screenshots, and defect documentation used to assess the release readiness of the tested journey.

## Execution Summary

| Status | Count |
|---|---:|
| Pass | 10 |
| Fail | 0 |
| Blocked | 0 |
| **Total** | **10** |

## Release Recommendation

The tested login-to-checkout journey is recommended for the next review stage based on the recorded results. All ten executed checks passed. This recommendation is limited to the tested requirements and the evidence captured during this manual QA review.

## Project Structure

```text
Manual-QA/
├─ README.md
├─ Swag Labs Login Page.png
├─ baseline-checkout-success.png
├─ docs/
│  ├─ baseline-run.md
│  ├─ defect-report.md
│  ├─ test-cases.md
│  ├─ test-strategy.md
│  └─ traceability.md
├─ evidence/
│  ├─ BUG-001-checkout-name-fields.png
│  ├─ Swag Labs Login Page.png
│  ├─ baseline-checkout-success.png
│  ├─ tc-01-inventory.png
│  ├─ tc-02-locked-out.png
│  ├─ tc-03-cart-bike-light.png
│  ├─ tc-04-cart-item-removed.png
│  ├─ tc-05-first-name-required.png
│  └─ tc-06-order-complete.png
└─ (supporting case-study artifacts)
```

## Repository Contents

- `README.md` — overview of the manual QA case study and execution summary.
- `docs/` — formal QA documentation including strategy, execution, defects, and traceability.
  - `baseline-run.md` — baseline test execution notes.
  - `defect-report.md` — defect details and impact analysis.
  - `test-cases.md` — manual test cases for the journey.
  - `test-strategy.md` — risk-based testing plan.
  - `traceability.md` — mapping between requirements, tests, and evidence.
- `evidence/` — screenshots that capture observed application behavior during execution.
- Root image files — key interface and checkout screenshots used as reference or introductory evidence.

## Documentation Notes

This repository is organized to support a manual QA workflow:

1. Review the test strategy and test cases.
2. Compare executed outcomes against the expected behavior.
3. Inspect defect and traceability records.
4. Use evidence images to validate execution history and results.

This structure is intended to make the project easy to review, audit, and extend as additional testing evidence is added.

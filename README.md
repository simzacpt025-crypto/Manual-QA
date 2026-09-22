# Manual-QA case study of the Swag Labs checkout journey, covering risk-based test design, execution evidence, defect reporting, and traceability.

This repository captures a manual QA validation of the Swag Labs end-to-end checkout flow. It includes the test strategy, executed test cases, additional checkout-validation scenarios, authentication decision-table checks, evidence screenshots, and defect documentation used to assess the journey from login through order completion.

## Execution Summary

The latest test-case update documents 12 end-to-end test cases and four authentication decision-table checks. The original execution evidence covers the first six end-to-end cases and the four authentication checks. The newly added checkout-validation and navigation scenarios (TC-07 through TC-12) still require execution evidence.

| Status | Count |
|---|---:|
| Pass | 10 |
| Fail | 0 |
| Blocked | 0 |
| Pending execution | 6 |
| **Total documented checks** | **16** |

## Coverage Added in the Latest Test-Case Update

- Checkout validation when the last name is blank (TC-07).
- Checkout validation when the postal code is blank (TC-08).
- Validation when all checkout fields are blank (TC-09).
- Checkout cancellation and cart preservation (TC-10).
- Continuing shopping from the cart (TC-11).
- Removing an item and clearing the cart badge (TC-12).
- Authentication checks for blank credentials, invalid credentials, and locked accounts.

## Release Recommendation

The tested login-to-checkout journey is recommended for the next review stage based on the recorded results. All ten executed checks passed. This recommendation is limited to the tested requirements and evidence currently recorded; TC-07 through TC-12 should be executed and documented before making a final release decision for the expanded coverage.

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

- `README.md` — overview of the manual QA case study, coverage, and execution summary.
- `docs/` — formal QA documentation including strategy, execution, defects, and traceability.
  - `baseline-run.md` — baseline test execution notes.
  - `defect-report.md` — defect details and impact analysis.
  - `test-cases.md` — 12 manual end-to-end test cases plus authentication decision-table checks.
  - `test-strategy.md` — risk-based testing plan.
  - `traceability.md` — mapping between requirements, tests, and evidence.
- `evidence/` — screenshots that capture observed application behavior during execution.
- Root image files — key interface and checkout screenshots used as reference or introductory evidence.

## Documentation Notes

This repository is organized to support a manual QA workflow:

1. Review the test strategy and test cases.
2. Compare executed outcomes against the expected behavior.
3. Execute and attach evidence for the pending scenarios.
4. Inspect defect and traceability records.
5. Use evidence images to validate execution history and results.

This structure is intended to make the project easy to review, audit, and extend as additional testing evidence is added.

## Reference ID:
WTC-4QJTYUQQ

## For Further Report:
https://github.com/simzacpt025-crypto/Automation-Testing

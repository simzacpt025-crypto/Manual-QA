# Traceability Matrix

## Execution Summary

| Status    | Count |
| --------- | ----: |
| Pass      |     6 |
| Fail      |     0 |
| Blocked   |     0 |
| **Total** | **6** |

The execution summary accounts for all six executed test cases.

## Requirements and Risk Coverage

| Requirement / Risk                                                      | Test Cases                                                                                                                            | Latest Result | Evidence                                                                                                           | Defect                      |
| ----------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------- | ------------------------------------------------------------------------------------------------------------------ | --------------------------- |
| REQ-01 — Valid shopper can reach inventory                              | [TC-01](test-cases.md#tc-01---valid-shopper-reaches-inventory)                                                                        | Pass          | [TC-01 evidence](../evidence/tc-01-inventory.png)                                                                  | None                        |
| REQ-02 — Selected product remains available in cart                     | [TC-03](test-cases.md#tc-03---selected-product-remains-in-cart), [TC-04](test-cases.md#tc-04---selected-product-is-removed-from-cart) | Pass          | [TC-03 evidence](../evidence/tc-03-cart-bike-light.png), [TC-04 evidence](../evidence/tc-04-cart-item-removed.png) | None                        |
| REQ-03 — Shopper with complete checkout information can finish an order | [TC-06](test-cases.md#tc-06---shopper-completes-checkout)                                                                             | Pass          | [TC-06 evidence](../evidence/tc-06-order-complete.png)                                                             | None                        |
| Authentication risk                                                     | [TC-01](test-cases.md#tc-01---valid-shopper-reaches-inventory), [TC-02](test-cases.md#tc-02---locked-out-shopper-is-rejected)         | Pass          | [TC-01 evidence](../evidence/tc-01-inventory.png), [TC-02 evidence](../evidence/tc-02-locked-out.png)              | None                        |
| Cart risk — lost cart contents                                          | [TC-03](test-cases.md#tc-03---selected-product-remains-in-cart), [TC-04](test-cases.md#tc-04---selected-product-is-removed-from-cart) | Pass          | [TC-03 evidence](../evidence/tc-03-cart-bike-light.png), [TC-04 evidence](../evidence/tc-04-cart-item-removed.png) | None                        |
| Validation risk — incorrect validation                                  | [TC-05](test-cases.md#tc-05---first-name-validation)                                                                                  | Pass          | [TC-05 evidence](../evidence/tc-05-first-name-required.png)                                                        | [BUG-001](defect-report.md) |
| Order-completion risk — failed order completion                         | [TC-06](test-cases.md#tc-06---shopper-completes-checkout)                                                                             | Pass          | [TC-06 evidence](../evidence/tc-06-order-complete.png)                                                             | None                        |

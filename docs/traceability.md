# Traceability Matrix

## Execution Summary

| Status    | Count |
| --------- | ----: |
| Pass      |    12 |
| Fail      |     0 |
| Blocked   |     0 |
| **Total** | **12** |

The execution summary accounts for all twelve executed test cases.

## Requirements and Risk Coverage

| Requirement / Risk                                                      | Test Cases                                                                                                              |
| ----------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| REQ-01 — Valid shopper can reach inventory                              | [TC-01](test-cases.md#tc-01---valid-shopper-reaches-inventory)                                                       |
| REQ-02 — Selected product remains available in cart                     | [TC-03](test-cases.md#tc-03---selected-product-remains-in-cart), [TC-04](test-cases.md#tc-04---selected-product-is-removed-from-the-cart) |
| REQ-03 — Shopper with complete checkout information can finish an order | [TC-06](test-cases.md#tc-06---shopper-completes-checkout)                                                            |
| Authentication risk                                                     | [TC-01](test-cases.md#tc-01---valid-shopper-reaches-inventory), [TC-02](test-cases.md#tc-02---locked-out-shopper-is-rejected) |
| Cart risk — lost cart contents                                          | [TC-03](test-cases.md#tc-03---selected-product-remains-in-cart), [TC-04](test-cases.md#tc-04---selected-product-is-removed-from-the-cart) |
| Validation risk — incorrect validation                                  | [TC-05](test-cases.md#tc-05---first-name-validation), [TC-07](test-cases.md#tc-07---checkout-requires-a-last-name), [TC-08](test-cases.md#tc-08---checkout-requires-a-postal-code), [TC-09](test-cases.md#tc-09---all-checkout-fields-are-required) |
| Order-completion risk — failed order completion                         | [TC-06](test-cases.md#tc-06---shopper-completes-checkout)                                                            |
| Navigation risk — checkout cancellation and continue-shopping           | [TC-10](test-cases.md#tc-10---checkout-can-be-cancelled), [TC-11](test-cases.md#tc-11---shopper-can-continue-shopping-from-the-cart) |
| Cart integrity risk — remove item from cart                             | [TC-12](test-cases.md#tc-12---shopper-can-remove-an-item-from-the-cart)                                              |

## Evidence Links

| Test Case | Evidence |
| --------- | -------- |
| TC-07 — Checkout requires a last name | [Evidence](../evidence/tc-07-checkout-requires-a-last-name.png) |
| TC-08 — Checkout requires a postal code | [Evidence](../evidence/tc-08-checkout-requires-a-postal-code.png) |
| TC-09 — All checkout fields are required | [Evidence](../evidence/tc-09-%20all-checkout-fields-are-required.png) |
| TC-10 — Checkout can be cancelled | [Evidence](../evidence/tc-10-checkout-can-be-cancelled.png) |
| TC-11 — Shopper can continue shopping from the cart | [Evidence](../evidence/tc-11-shopper-can-continue-shopping-from-the-cart.png) |
| TC-12 — Shopper can remove an item from the cart | [Evidence](../evidence/tc-12-shopper-can-remove-an-item-from-the-cart.png) |

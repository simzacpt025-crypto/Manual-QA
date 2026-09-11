# BUG-001 — Entering a last name overwrites the first-name field for problem_user

## Defect ID

BUG-001

## Title

Entering a last name overwrites the first-name field for `problem_user`.

## Environment

* **Application:** Swag Labs
* **Browser:** Microsoft Edge
* **Browser version:** Fire Fox 147.0.3 (64-bit)
* **Account:** `problem_user`

## Preconditions

* Swag Labs is open.
* The application state has been reset using **Reset App State**.
* The session is logged out.
* The user can log in with `problem_user` / `secret_sauce`.

## Related Test Case

* **Test Case:** TC-05
* **Related area:** Checkout information validation
* **Risk:** Incorrect validation / checkout data-entry failure

## Test Data

| Field      | Value                 |
| ---------- | --------------------- |
| Username   | `problem_user`        |
| Password   | `secret_sauce`        |
| Product    | Sauce Labs Bike Light |
| First Name | `Alex`                |
| Last Name  | `Tester`              |

## Steps to Reproduce

1. Open Swag Labs in Microsoft Edge.
2. Reset the application state.
3. Log out to start from a clean login state.
4. Log in using `problem_user` and `secret_sauce`.
5. Add **Sauce Labs Bike Light** to the cart.
6. Open the cart.
7. Select **Checkout**.
8. Enter `Alex` in the **First Name** field.
9. Verify that the First Name field contains `Alex` and the Last Name field is empty.
10. Enter `Tester` in the **Last Name** field.
11. Observe the values displayed in both name fields.

## Expected Result

The checkout form should contain two separate values:

* **First Name:** `Alex`
* **Last Name:** `Tester`

Entering a value into the Last Name field should not change the First Name field.

## Actual Result

After entering `Tester` in the Last Name field:

* **First Name:** `Tester`
* **Last Name:** empty

The entered last-name value overwrites the previously entered first-name value instead of remaining in the Last Name field.

The same behavior occurred during both clean-state reproduction runs.

## Severity

**Medium**

### Severity Rationale

The defect affects checkout data entry because entering a last name causes the first-name value to be overwritten and leaves the Last Name field empty. This prevents the shopper from entering the checkout information as intended and can interfere with completing the checkout journey correctly.

## Priority

**High**

### Priority Rationale

The defect should be addressed with high priority because it directly affects a checkout form and prevents the intended customer information from being entered correctly. The observed behavior was reproduced consistently with the `problem_user` account. The evidence supports the reproduced behavior and its impact on checkout data entry, but does not establish how many users are affected.

## Evidence

[BUG-001-checkout-name-fields.png](../evidence/BUG-001-checkout-name-fields.png)

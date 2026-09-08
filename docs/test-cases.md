# Swag Labs Test Cases

## TC-01 — Valid shopper can reach inventory

### Test Case ID: TC-01
### Requirement / Risk: REQ-01
### Preconditions:
- Swag Labs is open on the login page. The application is reset and the shopper is logged out.
### Test Priority: High
### Test Data:
- Username: standard_user
- Password: secret_sauce

### Execution Steps:
1. Open the Swag Labs login page.
2. Enter standard_user in the username field.
3. Enter secret_sauce in the password field.
4. Select Login.

### Expected Result: 
- The inventory/products page is displayed after the login form is submitted.

### Observed Actual Result:

### Status: PASS

### Evidence: ../evidence/tc-01-inventory.png

## TC-02 — Locked-out shopper is rejected

### Test Case ID: TC-02
### Requirement / Risk: Authentication failure
### Preconditions: 
- Swag Labs is open on the login page. The application is reset and the shopper is logged out.
### Test Priority: High
### Test Data:
- Username: locked_out_user
- Password: secret_sauce

### Execution Steps:
1. Open the Swag Labs login page.
2. Enter locked_out_user in the username field.
3. Enter secret_sauce in the password field.
4. Select Login.

### Expected Result: 
- Sorry, this user has been locked out. appears on the login page.

### Observed Actual Result:

### Status: BLOCKED

### Evidence: ../evidence/tc-02-locked-out.png

## TC-03 — Product remains available in cart

### Test Case ID: TC-03
### Requirement / Risk: REQ-02 + lost cart contents
### Preconditions: 
- Swag Labs is open on the login page. The application is reset and the shopper is logged out.
### Test Priority: High
### Test Data:
- Username: standard_user
- Password: secret_sauce

### Product: 
- Sauce Labs Bike Light
### Quantity: 1

### Execution Steps:
1. Log in using standard_user and secret_sauce.
2. Locate Sauce Labs Bike Light in the inventory.
3. Select Add to cart for the product.
4. Open the shopping cart.

### Expected Result: 
- Sauce Labs Bike Light is present in the cart with a quantity of 1.

### Observed Actual Result: PASS

### Status:

### Evidence: ../evidence/tc-03-cart-bike-light.png

## TC-04 — Product can be removed from cart

### Test Case ID: TC-04
### Requirement / Risk: REQ-02 + lost cart contents
### Preconditions:
- Swag Labs is open on the login page. The application is reset and the shopper is logged out.
### Test Priority: Medium
### Test Data:
- Username: standard_user
- Password: secret_sauce
- Product: Sauce Labs Bike Light
- Quantity: 1

### Execution Steps:
1. Log in using standard_user and secret_sauce.
2. Locate Sauce Labs Bike Light in the inventory.
3. Select Add to cart.
4. Open the shopping cart.
5. Select Remove for Sauce Labs Bike Light.

### Expected Result: 
- Sauce Labs Bike Light is absent from the cart after it is removed.

### Observed Actual Result:

### Status:

### Evidence: ../evidence/tc-04-cart-item-removed.png

## TC-05 — Required checkout field validation

## Test Case ID: TC-05
### Requirement / Risk: Incorrect validation
### Preconditions:
- Swag Labs is open on the login page. The application is reset and the shopper is logged out.
### Test Priority: Medium
### Test Data:
- Username: standard_user
- Password: secret_sauce
- Product: Sauce Labs Bike Light
- First Name: empty
- Last Name: Tester
- Postal Code: 12345

### Execution Steps:
1. Log in using standard_user and secret_sauce.
2. Add Sauce Labs Bike Light to the cart.
3. Open the shopping cart.
4. Select Checkout.
5. Leave the First Name field empty.
6. Enter Tester as the last name.
7. Enter 12345 as the postal code.
8. Select Continue.

### Expected Result: 
- First Name is required appears and checkout does not proceed.

### Observed Actual Result:

### Status:

### Evidence: ../evidence/tc-05-first-name-required.png

## TC-06 — Shopper can complete an order

### Test Case ID: TC-06
### Requirement / Risk: REQ-03 + failed order completion
### Preconditions: Swag Labs is open on the login page. The application is reset and the shopper is logged out.
### Test Priority: High
### Test Data:
- Username: standard_user
-  Password: secret_sauce
-  Product: Sauce Labs Bike Light
- First Name: Alex
- Last Name: Tester
- Postal Code: 1234

### Execution Steps:
1. Log in using standard_user and secret_sauce.
2. Add Sauce Labs Bike Light to the cart.
3. Open the shopping cart.
4. Select Checkout.
5. Enter Alex as the first name.
6. Enter Tester as the last name.
7. Enter 12345 as the postal code.
8. Select Continue.
9. Review the order overview.
10. Select Finish.

### Expected Result: 
- Thank you for your order! appears after completing checkout.

### Observed Actual Result:

### Status:

### Evidence: ../evidence/tc-06-order-complete.png

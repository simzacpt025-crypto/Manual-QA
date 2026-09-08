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
- Open the Swag Labs login page.
- Enter standard_user in the username field.
- Enter secret_sauce in the password field.
- Select Login.

### Expected Result: 
- The inventory/products page is displayed after the login form is submitted.

### Observed Actual Result:

### Status:

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
- Open the Swag Labs login page.
- Enter locked_out_user in the username field.
- Enter secret_sauce in the password field.
- Select Login.

### Expected Result: 
- Sorry, this user has been locked out. appears on the login page.

### Observed Actual Result:

### Status:

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
- Log in using standard_user and secret_sauce.
- Locate Sauce Labs Bike Light in the inventory.
- Select Add to cart for the product.
- Open the shopping cart.

###Expected Result: 
- Sauce Labs Bike Light is present in the cart with a quantity of 1.

### Observed Actual Result:

### Status:

### Evidence: ../evidence/tc-03-cart-bike-light.png


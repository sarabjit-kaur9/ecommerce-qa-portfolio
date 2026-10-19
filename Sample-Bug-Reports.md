E-commerce QA Portfolio – Sample Bug Reports
Document Information
Project: E-commerce QA Portfolio
Testing Type: Manual Functional Testing
Environment: To be recorded during testing
Status: Illustrative examples — not yet verified
Purpose: Demonstrate professional defect documentation
Important: These are hypothetical examples for portfolio practice. They must not be presented as actual defects found in a live application unless reproduced and verified.
BUG-001: Cart Subtotal Does Not Update After Quantity Change

Module: Shopping Cart
Severity: Major
Priority: High
Status: Example — Not Verified

Description

The cart subtotal may fail to update when a user changes the quantity of an item.

Preconditions
The user has opened the shopping cart.
At least one product has been added to the cart.
Steps to Reproduce
Add a product priced at €10 to the cart.
Open the shopping cart.
Change the product quantity from 1 to 2.
Observe the displayed subtotal.
Expected Result

The subtotal updates to €20, assuming no additional charges apply.

Actual Result

Example only: The subtotal remains €10 after the quantity changes.

Evidence

Attach a screenshot or screen recording after reproducing the issue.

Test Case Reference

TC_CART_003 and TC_CART_004

BUG-002: Checkout Accepts an Invalid Email Address

Module: Checkout
Severity: Major
Priority: High
Status: Example — Not Verified

Description

The checkout form may accept an incorrectly formatted email address when email validation is required.

Preconditions
The user has proceeded to checkout.
The application includes an email field with a defined validation rule.
Steps to Reproduce
Open the checkout page.
Enter an invalid email format, such as user@.
Complete other required fields with valid test data.
Submit the form.
Expected Result

The application displays a validation message and prevents submission until the email address meets the defined validation rules.

Actual Result

Example only: The form accepts the invalid email address and proceeds.

Evidence

Attach a screenshot showing the input and resulting validation behaviour.

Test Case Reference

TC_CHECKOUT_003

BUG-003: Removed Product Remains in the Cart

Module: Shopping Cart
Severity: Major
Priority: High
Status: Example — Not Verified

Description

A product may remain visible in the cart after the user selects the remove action.

Preconditions
The cart contains at least one product.
Steps to Reproduce
Open the shopping cart.
Select Remove for a product.
Wait for the cart to update.
Check the product list and cart subtotal.
Expected Result

The product disappears from the cart, and the subtotal recalculates correctly.

Actual Result

Example only: The product remains visible after the remove action.

Evidence

Capture the cart before and after the remove action.

Test Case Reference

TC_CART_002 and TC_CART_004

BUG-004: Login Error Message Does Not Explain the Failure

Module: User Authentication
Severity: Minor
Priority: Medium
Status: Example — Not Verified

Description

The login page may fail to display a clear, user-friendly message when invalid credentials are submitted.

Preconditions
The login page is accessible.
Steps to Reproduce
Enter an invalid username or password.
Select Login.
Observe the message displayed to the user.
Expected Result

A clear error message explains that the credentials are invalid without revealing sensitive authentication information.

Actual Result

Example only: The application displays no useful feedback or an unclear error message.

Evidence

Attach a screenshot of the login response.

Test Case Reference

TC_LOGIN_002 and TC_LOGIN_003

BUG-005: Product Search Returns Irrelevant Results

Module: Product Catalogue
Severity: Minor
Priority: Medium
Status: Example — Not Verified

Description

The product search may return items that do not match the search query when matching results are expected.

Preconditions
The product catalogue contains known products.
Search functionality is available.
Steps to Reproduce
Open the product catalogue.
Search for a known product name.
Review the returned results.
Compare the results with the application's documented search behaviour.
Expected Result

The search results follow the application's defined matching rules and do not include irrelevant products.

Actual Result

Example only: Products unrelated to the search query appear in the results.

Evidence

Capture the search term and the returned results.

Test Case Reference

TC_PROD_003 and TC_PROD_004

Bug Reporting Best Practices
Write concise, descriptive titles.
Include repeatable steps to reproduce.
Separate expected results from actual results.
Assign severity based on impact and priority based on urgency.
Attach relevant evidence and record the test environment.
Verify each defect before reporting it as a confirmed issue.
Never fabricate test results or claim hypothetical defects were discovered in a real application.
Severity Reference
Severity	Description
Critical	Core system failure, severe data loss, or a major security issue
Major	Important functionality is broken
Minor	Limited functional issue with a workaround
Trivial	Cosmetic or low-impact issue
Priority Reference
Priority	Description
High	Requires urgent attention
Medium	Should be addressed in the normal development cycle
Low	Can be addressed when resources permit
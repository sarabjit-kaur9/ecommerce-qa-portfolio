E-commerce Application – Manual Test Cases
1. Document Information
Field	Details
Project	E-commerce QA Portfolio
Module	E-commerce Web Application
Testing Type	Manual Functional Testing
Test Case Count	20
Author	QA Portfolio
Execution Status	Not Executed
2. Test Cases
Module A: User Login
Test Case ID	Test Scenario	Test Steps	Expected Result	Priority
TC_LOGIN_001	Login with valid credentials	Enter valid username and password; click Login	User logs in successfully	High
TC_LOGIN_002	Login with invalid password	Enter valid username and incorrect password	Appropriate error message appears	High
TC_LOGIN_003	Login with invalid username	Enter an unregistered username and a password	Login is rejected with an appropriate message	High
TC_LOGIN_004	Login with empty fields	Leave username and password empty; click Login	Required-field validation appears, or login is rejected	High
TC_LOGIN_005	Password masking	Enter a password in the password field	Password is masked by default	Medium
Module B: Product Catalogue and Search
Test Case ID	Test Scenario	Test Steps	Expected Result	Priority
TC_PROD_001	View product catalogue	Open the product listing page	Available products display correctly	High
TC_PROD_002	View product details	Select a product	Correct product name, price, and details appear	High
TC_PROD_003	Search for an existing product	Search using a known product name	Relevant matching products are displayed	High
TC_PROD_004	Search for a nonexistent product	Search using a term with no matching products	An appropriate no-results message appears	Medium
TC_PROD_005	Sort products by price	Select the price sorting option	Products appear in the selected price order	Medium
Module C: Shopping Cart
Test Case ID	Test Scenario	Test Steps	Expected Result	Priority
TC_CART_001	Add a product to the cart	Open a product and click Add to Cart	Product is added to the cart	High
TC_CART_002	Remove a product from the cart	Add a product and then remove it	Product is removed from the cart	High
TC_CART_003	Update product quantity	Change a cart item's quantity	Quantity and subtotal update correctly	High
TC_CART_004	Verify cart subtotal	Add products with known prices	Subtotal equals the sum of item prices multiplied by quantities	High
TC_CART_005	View an empty cart	Open the cart without adding products	An appropriate empty-cart message appears	Medium
Module D: Checkout
Test Case ID	Test Scenario	Test Steps	Expected Result	Priority
TC_CHECKOUT_001	Proceed to checkout	Add a product and select Checkout	Checkout page opens successfully	High
TC_CHECKOUT_002	Submit checkout with missing details	Leave required delivery fields empty and submit	Required-field validation prevents invalid submission	High
TC_CHECKOUT_003	Enter invalid email format	Enter an invalid email address in a checkout email field, if available	Appropriate validation is displayed	Medium
TC_CHECKOUT_004	Verify order total	Review item subtotal, shipping, tax, and total where applicable	Displayed total follows the application's pricing rules	High
TC_CHECKOUT_005	Complete a valid order	Enter valid required details and confirm the order in a test environment	Order confirmation appears and order details are correct	High
3. Test Execution Results

Record actual outcomes only after executing the tests against the selected application.

Status	Meaning
Not Executed	Test has not been run
Pass	Actual result matches the expected result
Fail	Actual result differs from the expected result
Blocked	Test cannot proceed because of a dependency or environment issue
4. Defect Reporting Guidelines

For each failed test, document:

Bug ID
Related test case ID
Summary
Preconditions
Steps to reproduce
Expected result
Actual result
Severity and priority
Screenshot or other evidence
Environment and browser
Defect status
5. Notes
These are sample test cases for a generic e-commerce application.
Adapt the steps to the actual application's interface and behaviour.
Use an authorised test environment and test accounts.
Do not record real passwords or sensitive customer information.
Do not mark tests as passed until they have been executed and verified.
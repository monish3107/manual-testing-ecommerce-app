# **Test Scenarios - E-Commerce Website (automationexercise.com)**

## **Document Information**

| Field | Details |
|-------|---------|
| **Project Name** | Manual Testing - E-Commerce Application |
| **Application URL** | https://automationexercise.com |
| **Document Version** | 1.0 |
| **Prepared By** | Monish Parulekar |
| **Date Created** | November 16, 2025 |
| **Last Updated** | November 16, 2025 |
| **Document Status** | Approved |

---

## **1. Introduction**

### **1.1 Purpose**
This document contains high-level test scenarios for the e-commerce application. Test scenarios define **WHAT** to test without detailing the exact steps. They serve as the foundation for creating detailed test cases.

### **1.2 Scope**
This document covers test scenarios for all functional modules identified in the requirements document, including positive, negative, and boundary scenarios.

---

## **2. Test Scenario Guidelines**

### **2.1 Scenario Naming Convention**
- Format: `TS_<MODULE>_<NUMBER>`
- Example: `TS_AUTH_001`, `TS_CART_005`

### **2.2 Module Codes**
| Module Code | Module Name |
|-------------|-------------|
| **AUTH** | User Authentication (Login/Signup/Logout) |
| **PROFILE** | User Profile Management |
| **PROD** | Product Catalog & Search |
| **CART** | Shopping Cart |
| **CHECKOUT** | Checkout Process |
| **PAY** | Payment |
| **ORDER** | Order Management |
| **CONTACT** | Contact Us |
| **SUB** | Subscription |
| **NAV** | Navigation & UI |

---

## **3. Test Scenarios by Module**

---

## **Module 1: User Authentication**

| Scenario ID | Test Scenario | Priority | Test Type |
|-------------|---------------|----------|-----------|
| TS_AUTH_001 | Verify user can register with valid details | High | Positive |
| TS_AUTH_002 | Verify user cannot register with existing email | High | Negative |
| TS_AUTH_003 | Verify user cannot register with invalid email format | Medium | Negative |
| TS_AUTH_004 | Verify user cannot register with empty required fields | Medium | Negative |
| TS_AUTH_005 | Verify user can login with valid credentials | High | Positive |
| TS_AUTH_006 | Verify user cannot login with invalid credentials | High | Negative |
| TS_AUTH_007 | Verify user cannot login with empty credentials | Medium | Negative |
| TS_AUTH_008 | Verify user can logout successfully | High | Positive |
| TS_AUTH_009 | Verify logged-in user state persists across pages | Medium | Positive |
| TS_AUTH_010 | Verify password field is masked during entry | Low | Security |
| TS_AUTH_011 | Verify user can delete account | Medium | Positive |
| TS_AUTH_012 | Verify account created success message is displayed | Medium | Positive |

---

## **Module 2: User Profile Management**

| Scenario ID | Test Scenario | Priority | Test Type |
|-------------|---------------|----------|-----------|
| TS_PROFILE_001 | Verify logged-in username is displayed in header | Medium | Positive |
| TS_PROFILE_002 | Verify delivery address matches registration address during checkout | Medium | Positive |
| TS_PROFILE_003 | Verify billing address matches registration address during checkout | Medium | Positive |
| TS_PROFILE_004 | Verify user can delete account successfully | Medium | Positive |

---

## **Module 3: Product Catalog & Search**

| Scenario ID | Test Scenario | Priority | Test Type |
|-------------|---------------|----------|-----------|
| TS_PROD_001 | Verify user can view all product categories | High | Positive |
| TS_PROD_002 | Verify user can navigate to specific product category (Women/Men/Kids) | High | Positive |
| TS_PROD_003 | Verify user can view individual product details | High | Positive |
| TS_PROD_004 | Verify product details display correctly (name, category, price, availability, condition, brand) | High | Positive |
| TS_PROD_005 | Verify user can search products using valid keywords | High | Positive |
| TS_PROD_006 | Verify search shows relevant results | Medium | Positive |
| TS_PROD_007 | Verify search with no results shows appropriate message | Medium | Negative |
| TS_PROD_008 | Verify search with special characters handles gracefully | Low | Negative |
| TS_PROD_009 | Verify user can view all products page | High | Positive |
| TS_PROD_010 | Verify category filters work correctly (Women - Dress/Tops/Saree) | Medium | Positive |
| TS_PROD_011 | Verify brand filters work correctly | Medium | Positive |
| TS_PROD_012 | Verify user can navigate between different brand products | Medium | Positive |
| TS_PROD_013 | Verify user can write product review | Medium | Positive |
| TS_PROD_014 | Verify product review submission shows success message | Medium | Positive |

---

## **Module 4: Shopping Cart**

| Scenario ID | Test Scenario | Priority | Test Type |
|-------------|---------------|----------|-----------|
| TS_CART_001 | Verify user can add product to cart from products page | High | Positive |
| TS_CART_002 | Verify user can add multiple products to cart | High | Positive |
| TS_CART_003 | Verify user can set quantity before adding to cart (product detail page) | High | Positive |
| TS_CART_004 | Verify cart displays correct product details | High | Positive |
| TS_CART_005 | Verify cart shows correct total price | High | Positive |
| TS_CART_006 | Verify user can view cart summary | High | Positive |
| TS_CART_007 | Verify user can remove product from cart | High | Positive |
| TS_CART_008 | Verify empty cart shows appropriate message | Medium | Positive |
| TS_CART_009 | Verify cart persists for logged-in users after login | Medium | Positive |
| TS_CART_010 | Verify cart total calculation with multiple items | High | Positive |
| TS_CART_011 | Verify Continue Shopping button functionality | Medium | Positive |
| TS_CART_012 | Verify recommended items can be added to cart | Low | Positive |
| TS_CART_013 | Verify individual product quantities are displayed in cart | Medium | Positive |

---

## **Module 5: Checkout Process**

| Scenario ID | Test Scenario | Priority | Test Type |
|-------------|---------------|----------|-----------|
| TS_CHECKOUT_001 | Verify user can proceed to checkout from cart | High | Positive |
| TS_CHECKOUT_002 | Verify checkout page displays order summary | High | Positive |
| TS_CHECKOUT_003 | Verify user can enter shipping address | High | Positive |
| TS_CHECKOUT_004 | Verify user can enter billing address | High | Positive |
| TS_CHECKOUT_005 | Verify required fields validation in checkout | High | Negative |
| TS_CHECKOUT_006 | Verify user cannot checkout with empty required fields | High | Negative |
| TS_CHECKOUT_007 | Verify user can add comments/notes to order | Low | Positive |
| TS_CHECKOUT_008 | Verify checkout shows correct product quantities | High | Positive |
| TS_CHECKOUT_009 | Verify checkout shows correct total amount | High | Positive |
| TS_CHECKOUT_010 | Verify user must be logged in to checkout (if required) | High | Positive |

---

## **Module 6: Payment**

| Scenario ID | Test Scenario | Priority | Test Type |
|-------------|---------------|----------|-----------|
| TS_PAY_001 | Verify user can enter payment card details | High | Positive |
| TS_PAY_002 | Verify payment page displays order total | High | Positive |
| TS_PAY_003 | Verify user can complete payment successfully | High | Positive |
| TS_PAY_004 | Verify payment accepts any card details (no validation) | Medium | Negative |
| TS_PAY_005 | Verify payment confirmation message is displayed | High | Positive |
| TS_PAY_006 | Verify order confirmation number/page is displayed | High | Positive |
| TS_PAY_007 | Verify all payment fields accept input | Medium | Positive |

---

## **Module 7: Order Management**

| Scenario ID | Test Scenario | Priority | Test Type |
|-------------|---------------|----------|-----------|
| TS_ORDER_001 | Verify order confirmation message after successful payment | High | Positive |
| TS_ORDER_002 | Verify order confirmation page displays correct details | High | Positive |
| TS_ORDER_003 | Verify user can download invoice after order placement | High | Positive |
| TS_ORDER_004 | Verify invoice file downloads as invoice.txt | Medium | Positive |
| TS_ORDER_005 | Verify invoice content displays order information | High | Negative |
| TS_ORDER_006 | Verify order success message is displayed | High | Positive |

---

## **Module 8: Contact Us**

| Scenario ID | Test Scenario | Priority | Test Type |
|-------------|---------------|----------|-----------|
| TS_CONTACT_001 | Verify user can access Contact Us page | Medium | Positive |
| TS_CONTACT_002 | Verify user can submit contact form with valid data | High | Positive |
| TS_CONTACT_003 | Verify contact form shows success message after submission | High | Positive |
| TS_CONTACT_004 | Verify user cannot submit contact form with empty required fields | Medium | Negative |
| TS_CONTACT_005 | Verify user can upload file in contact form (if available) | Low | Positive |
| TS_CONTACT_006 | Verify contact form email validation | Medium | Negative |
| TS_CONTACT_007 | Verify contact page displays contact information | Low | Positive |

---

## **Module 9: Subscription**

| Scenario ID | Test Scenario | Priority | Test Type |
|-------------|---------------|----------|-----------|
| TS_SUB_001 | Verify user can subscribe to newsletter with valid email | Medium | Positive |
| TS_SUB_002 | Verify subscription shows success message | Medium | Positive |
| TS_SUB_003 | Verify subscription with invalid email shows error | Medium | Negative |
| TS_SUB_004 | Verify subscription with empty email shows error | Medium | Negative |
| TS_SUB_005 | Verify user cannot subscribe with already subscribed email | Low | Negative |

---

## **Module 10: Navigation & UI**

| Scenario ID | Test Scenario | Priority | Test Type |
|-------------|---------------|----------|-----------|
| TS_NAV_001 | Verify all header navigation links work correctly | High | Positive |
| TS_NAV_002 | Verify all footer links work correctly | Medium | Positive |
| TS_NAV_003 | Verify logo redirects to homepage | Medium | Positive |
| TS_NAV_004 | Verify Test Cases page is accessible | Medium | Positive |
| TS_NAV_005 | Verify no broken links on the website | High | Negative |
| TS_NAV_006 | Verify website is responsive on mobile devices | High | Compatibility |
| TS_NAV_007 | Verify website works on different browsers (Chrome, Firefox, Edge) | High | Compatibility |
| TS_NAV_008 | Verify page load time is acceptable | Medium | Performance |
| TS_NAV_009 | Verify consistent UI layout across pages | Medium | Positive |
| TS_NAV_010 | Verify scroll to top functionality with arrow button | Low | Positive |
| TS_NAV_011 | Verify scroll to top functionality without arrow button | Low | Positive |
| TS_NAV_012 | Verify subscription section is visible at footer | Medium | Positive |

---

## **Module 11: End-to-End Workflows**

| Scenario ID | Test Scenario | Priority | Test Type |
|-------------|---------------|----------|-----------|
| TS_E2E_001 | Verify complete user registration to order placement flow | High | E2E |
| TS_E2E_002 | Verify register during checkout flow | High | E2E |
| TS_E2E_003 | Verify login before checkout flow | High | E2E |
| TS_E2E_004 | Verify user can search product, add to cart, and checkout | High | E2E |
| TS_E2E_005 | Verify cart persists after login | Medium | E2E |
| TS_E2E_006 | Verify complete flow from homepage to invoice download | High | E2E |

---

## **4. Test Scenario Summary**

| Module | Total Scenarios | High Priority | Medium Priority | Low Priority |
|--------|----------------|---------------|-----------------|--------------|
| Authentication | 12 | 5 | 5 | 2 |
| Profile Management | 4 | 0 | 4 | 0 |
| Product Catalog | 14 | 5 | 7 | 2 |
| Shopping Cart | 13 | 7 | 5 | 1 |
| Checkout | 10 | 8 | 0 | 2 |
| Payment | 7 | 5 | 2 | 0 |
| Order Management | 6 | 4 | 2 | 0 |
| Contact Us | 7 | 2 | 3 | 2 |
| Subscription | 5 | 0 | 4 | 1 |
| Navigation & UI | 12 | 4 | 5 | 3 |
| End-to-End | 6 | 5 | 1 | 0 |
| **TOTAL** | **96** | **45** | **38** | **13** |

---

## **5. Priority Definition**

| Priority | Definition | Action |
|----------|------------|--------|
| **High** | Critical functionality, core user flows | Must be tested first |
| **Medium** | Important but not critical, has workarounds | Test after high priority |
| **Low** | Nice to have, UI/cosmetic issues | Test if time permits |

---

## **6. Test Type Definition**

| Test Type | Description |
|-----------|-------------|
| **Positive** | Testing with valid inputs and expected behavior |
| **Negative** | Testing with invalid inputs and error scenarios |
| **Security** | Testing security-related features |
| **Compatibility** | Testing across browsers and devices |
| **Performance** | Testing load time and responsiveness |
| **E2E** | End-to-end complete user workflows |

---

## **7. Notes**

- All scenarios are based on actual website behavior verified through manual exploration
- **Known limitations identified:**
  - No user profile/account management page exists (only "Logged in as username" display)
  - No cart item counter in header/icon
  - No total cart item count displayed (individual product quantities only)
  - Payment accepts any card details without validation (test/demo mode)
  - Invoice downloads as invoice.txt with potential data accuracy issues
- Cart quantity update: Users can set quantity on product detail page before adding to cart and not on the cart page
- Invoice download: Available after successful order placement
- Additional bugs/issues will be documented during test execution

---

**Document Status:** Ready for Test Case Development  
**Next Steps:** Create detailed test cases for each scenario with step-by-step instructions

---

**End of Test Scenarios Document**

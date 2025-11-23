# Requirements Traceability Matrix (RTM) - E-commerce Testing Project

## Project Overview

**Project:** E-commerce Testing Project  
**Prepared By:** Monish Parulekar  
**Designation:** QA Engineer / Manual Tester  
**Date:** 16/11/2025  
**Total Test Cases:** 113  
**Test Coverage:** 91.15% Pass Rate

## Executive Summary

| Metric | Count | Percentage |
|--------|-------|------------|
| Total Test Cases | 113 | 100% |
| Passed | 103 | 91.15% |
| Failed | 7 | 6.19% |
| Retest Required | 2 | 1.77% |
| Not Executed | 1 | 0.88% |

## Traceability Matrix

### Authentication Module (FR1-FR7, FR11, NFR12, NFR13)

| Requirement ID | Test Case ID | Test Case Title | Status | Priority |
|---------------|-------------|----------------|---------|----------|
| **FR1** | TC_AUTH_001 | Register User with Valid Details | PASS | HIGH |
| **FR1** | TC_AUTH_004 | Register with Empty Required Fields | PASS | MEDIUM |
| **FR1** | TC_AUTH_012 | Verify Account Created Success Message | PASS | MEDIUM |
| **FR1** | TC_AUTH_014 | Register with Special Characters in Name | FAIL | LOW |
| **FR1** | TC_AUTH_015 | Verify Signup Button is Clickable | PASS | LOW |
| **FR2** | TC_AUTH_005 | Login with Valid Credentials | PASS | HIGH |
| **FR2** | TC_AUTH_006 | Login with Invalid Password | PASS | HIGH |
| **FR2** | TC_AUTH_007 | Login with Empty Credentials | PASS | MEDIUM |
| **FR2** | TC_AUTH_011 | Verify Logged-in State Persists Across Pages | PASS | MEDIUM |
| **FR2** | TC_AUTH_013 | Login with Invalid Email | PASS | MEDIUM |
| **FR3** | TC_AUTH_008 | Logout User Successfully | PASS | HIGH |
| **FR6** | TC_AUTH_002 | Register User with Existing Email | PASS | HIGH |
| **FR7** | TC_AUTH_003 | Register with Invalid Email Format | PASS | MEDIUM |
| **FR11** | TC_AUTH_010 | Delete Account Successfully | PASS | MEDIUM |
| **NFR12** | TC_AUTH_009 | Verify Password Field is Masked | PASS | LOW |
| **NFR13** | TC_AUTH_006 | Login with Invalid Password | PASS | HIGH |

### Product Catalog Module (FR8-FR10, FR12-FR13)

| Requirement ID | Test Case ID | Test Case Title | Status | Priority |
|---------------|-------------|----------------|---------|----------|
| **FR8** | TC_PROD_001 | View All Product Categories | PASS | HIGH |
| **FR8** | TC_PROD_002 | Navigate to Women Category | PASS | HIGH |
| **FR8** | TC_PROD_016 | Navigate to Men Category | PASS | MEDIUM |
| **FR8** | TC_PROD_017 | Navigate to Kids Category | PASS | MEDIUM |
| **FR9** | TC_PROD_003 | View Individual Product Details | PASS | HIGH |
| **FR9** | TC_PROD_009 | View All Products Page | PASS | HIGH |
| **FR10** | TC_PROD_005 | Search Product with Valid Keyword | PASS | HIGH |
| **FR10** | TC_PROD_006 | Verify Search Shows Relevant Results | PASS | MEDIUM |
| **FR10** | TC_PROD_007 | Search Product with No Results | PASS | MEDIUM |
| **FR10** | TC_PROD_008 | Search Product with Special Characters | PASS | LOW |
| **FR12** | TC_PROD_004 | Verify Product Information Display is Complete | PASS | HIGH |
| **FR12** | TC_PROD_015 | Verify Product Image Loads Correctly | PASS | MEDIUM |
| **FR12** | TC_PROD_018 | Verify Product Price is Displayed Correctly | PASS | HIGH |
| **FR13** | TC_PROD_002 | Navigate to Women Category | PASS | HIGH |
| **FR13** | TC_PROD_010 | Verify Category Filter - Women Dress | PASS | MEDIUM |
| **FR13** | TC_PROD_011 | Verify Brand Filter Functionality | PASS | MEDIUM |
| **FR13** | TC_PROD_012 | Navigate Between Different Brand Products | PASS | MEDIUM |
| **FR13** | TC_PROD_013 | Write Product Review | PASS | MEDIUM |
| **FR13** | TC_PROD_014 | Verify Review Submission Success Message | PASS | MEDIUM |
| **FR13** | TC_PROD_016 | Navigate to Men Category | PASS | MEDIUM |

### Shopping Cart Module (FR14-FR19)

| Requirement ID | Test Case ID | Test Case Title | Status | Priority |
|---------------|-------------|----------------|---------|----------|
| **FR14** | TC_CART_001 | Add Product to Cart from Products Page | PASS | HIGH |
| **FR14** | TC_CART_002 | Add Multiple Products to Cart | PASS | HIGH |
| **FR14** | TC_CART_011 | Verify Continue Shopping Button | PASS | MEDIUM |
| **FR14** | TC_CART_012 | Add Recommended Items to Cart | NOT EXECUTED | LOW |
| **FR14** | TC_CART_015 | Add Same Product Multiple Times to Cart | PASS | MEDIUM |
| **FR15** | TC_CART_004 | View Cart Summary | PASS | HIGH |
| **FR15** | TC_CART_005 | Verify Cart Shows Correct Product Details | PASS | HIGH |
| **FR15** | TC_CART_008 | Verify Empty Cart Shows Appropriate Message | PASS | MEDIUM |
| **FR15** | TC_CART_013 | Verify Individual Product Quantities | PASS | MEDIUM |
| **FR15** | TC_CART_014 | Verify Cart Button in Header | PASS | MEDIUM |
| **FR15** | TC_CART_016 | Verify Cart Page Layout | PASS | LOW |
| **FR16** | TC_CART_003 | Set Product Quantity Before Adding to Cart | PASS | HIGH |
| **FR17** | TC_CART_007 | Remove Product from Cart | PASS | HIGH |
| **FR18** | TC_CART_006 | Verify Cart Shows Correct Total Price | PASS | HIGH |
| **FR18** | TC_CART_010 | Verify Cart Total with Multiple Items | PASS | HIGH |
| **FR19** | TC_CART_009 | Verify Cart Persists After Login | PASS | MEDIUM |

### Checkout Module (FR21-FR26)

| Requirement ID | Test Case ID | Test Case Title | Status | Priority |
|---------------|-------------|----------------|---------|----------|
| **FR21** | TC_CHECKOUT_001 | Proceed to Checkout from Cart | PASS | HIGH |
| **FR21** | TC_CHECKOUT_010 | Verify Login Required for Checkout | PASS | HIGH |
| **FR21** | TC_CHECKOUT_011 | Register During Checkout Flow | PASS | HIGH |
| **FR21** | TC_CHECKOUT_012 | Verify Checkout Page Loads Completely | PASS | MEDIUM |
| **FR22** | TC_CHECKOUT_003 | Verify Delivery Address on Checkout | PASS | HIGH |
| **FR22** | TC_CHECKOUT_004 | Verify Billing Address on Checkout | PASS | HIGH |
| **FR23** | TC_CHECKOUT_002 | Verify Checkout Displays Order Summary | PASS | HIGH |
| **FR23** | TC_CHECKOUT_008 | Verify Product Quantities in Checkout | PASS | HIGH |
| **FR23** | TC_CHECKOUT_009 | Verify Total Amount in Checkout | PASS | HIGH |
| **FR24** | TC_CHECKOUT_007 | Add Comments to Order | PASS | LOW |
| **FR26** | TC_CHECKOUT_005 | Verify Required Fields Validation | PASS | HIGH |
| **FR26** | TC_CHECKOUT_006 | Cannot Checkout with Missing Info | PASS | HIGH |

### Payment Module (FR27-FR30, NFR13-NFR14)

| Requirement ID | Test Case ID | Test Case Title | Status | Priority |
|---------------|-------------|----------------|---------|----------|
| **FR27** | TC_PAY_001 | Enter Payment Card Details | FAIL | HIGH |
| **FR27** | TC_PAY_007 | Verify All Payment Fields Accept Input | PASS | MEDIUM |
| **FR28** | TC_PAY_002 | Verify Payment Page Displays Order Total | PASS | HIGH |
| **FR28** | TC_PAY_003 | Complete Payment Successfully | PASS | HIGH |
| **FR28** | TC_PAY_008 | Verify Payment Button is Clickable | PASS | MEDIUM |
| **FR29** | TC_PAY_003 | Complete Payment Successfully | PASS | HIGH |
| **FR29** | TC_PAY_005 | Verify Payment Confirmation Message | PASS | HIGH |
| **FR30** | TC_PAY_003 | Complete Payment Successfully | PASS | HIGH |
| **FR30** | TC_PAY_006 | Verify Order Confirmation Page | PASS | HIGH |
| **NFR13** | TC_PAY_004 | Payment Accepts Invalid Card (Bug) | PASS | HIGH |
| **NFR14** | TC_PAY_004 | Payment Accepts Invalid Card (Bug) | PASS | HIGH |

### Order Management Module (FR29-FR30, FR33)

| Requirement ID | Test Case ID | Test Case Title | Status | Priority |
|---------------|-------------|----------------|---------|----------|
| **FR29** | TC_ORDER_001 | Verify Order Confirmation Message After Payment | PASS | HIGH |
| **FR29** | TC_ORDER_006 | Verify Order Success Message is Displayed | PASS | HIGH |
| **FR30** | TC_ORDER_002 | Verify Order Confirmation Page Displays Details | PASS | HIGH |
| **FR30** | TC_ORDER_007 | Verify Continue Button on Order Confirmation | PASS | MEDIUM |
| **FR33** | TC_ORDER_003 | Download Invoice After Order Placement | PASS | HIGH |
| **FR33** | TC_ORDER_004 | Verify Invoice Downloads as Text File | PASS | MEDIUM |
| **FR33** | TC_ORDER_005 | Verify Invoice Content Shows Order Info | FAIL | HIGH |

### Contact Us Module (FR35-FR39)

| Requirement ID | Test Case ID | Test Case Title | Status | Priority |
|---------------|-------------|----------------|---------|----------|
| **FR35** | TC_CONTACT_001 | Access Contact Us Page | PASS | MEDIUM |
| **FR35** | TC_CONTACT_007 | Verify Contact Page Displays Contact Information | PASS | LOW |
| **FR36** | TC_CONTACT_002 | Submit Contact Form with Valid Data | PASS | HIGH |
| **FR37** | TC_CONTACT_005 | Upload File Attachment in Contact Form | PASS | LOW |
| **FR38** | TC_CONTACT_002 | Submit Contact Form with Valid Data | PASS | HIGH |
| **FR38** | TC_CONTACT_003 | Verify Contact Form Success Message Display | PASS | HIGH |
| **FR38** | TC_CONTACT_008 | Verify Home Button Functionality After Submission | FAIL | MEDIUM |
| **FR39** | TC_CONTACT_004 | Cannot Submit Contact Form with Empty Required Fields | FAIL | MEDIUM |
| **FR39** | TC_CONTACT_006 | Verify Email Format Validation on Contact Form | PASS | MEDIUM |

### Subscription Module (FR40-FR42)

| Requirement ID | Test Case ID | Test Case Title | Status | Priority |
|---------------|-------------|----------------|---------|----------|
| **FR40** | TC_SUB_001 | Subscribe to Newsletter with Valid Email | PASS | MEDIUM |
| **FR40** | TC_SUB_005 | Subscribe with Already Subscribed Email | FAIL | LOW |
| **FR40** | TC_SUB_006 | Verify Subscription Section in Cart Page Footer | PASS | MEDIUM |
| **FR41** | TC_SUB_002 | Verify Subscription Success Message Display | PASS | MEDIUM |
| **FR42** | TC_SUB_003 | Cannot Subscribe with Invalid Email Format | PASS | MEDIUM |
| **FR42** | TC_SUB_004 | Cannot Subscribe with Empty Email Field | PASS | MEDIUM |

### Navigation & UI Module (FR43-FR47, NFR1-NFR2, NFR8-NFR9)

| Requirement ID | Test Case ID | Test Case Title | Status | Priority |
|---------------|-------------|----------------|---------|----------|
| **FR43** | TC_NAV_001 | Verify All Header Navigation Links Work | PASS | HIGH |
| **FR43** | TC_NAV_003 | Verify Logo Redirects to Homepage | PASS | MEDIUM |
| **FR43** | TC_NAV_004 | Verify Test Cases Page is Accessible | PASS | MEDIUM |
| **FR43** | TC_NAV_010 | Verify Scroll to Top with Arrow Button | PASS | LOW |
| **FR43** | TC_NAV_011 | Verify Scroll Up Without Arrow Button | PASS | LOW |
| **FR43** | TC_NAV_012 | Verify Subscription Section in Footer | PASS | MEDIUM |
| **FR43** | TC_NAV_013 | Verify Navbar is Sticky/Fixed | FAIL | LOW |
| **FR44** | TC_NAV_009 | Verify Consistent UI Layout Across Pages | PASS | MEDIUM |
| **FR44** | TC_NAV_014 | Verify Homepage Banner/Slider | PASS | LOW |
| **FR45** | TC_NAV_001 | Verify All Header Navigation Links Work | PASS | HIGH |
| **FR45** | TC_NAV_005 | Verify No Broken Links on Website | PASS | HIGH |
| **FR47** | TC_NAV_002 | Verify All Footer Links Work | PASS | MEDIUM |
| **NFR1** | TC_NAV_008 | Verify Page Load Time is Acceptable | PASS | MEDIUM |
| **NFR2** | TC_NAV_015 | Verify Search Returns Results Quickly | PASS | MEDIUM |
| **NFR8** | TC_NAV_007 | Verify Website Works on Different Browsers | PASS | HIGH |
| **NFR9** | TC_NAV_006 | Verify Website is Responsive on Mobile | PASS | HIGH |

### End-to-End Module (Multiple FRs)

| Requirement IDs | Test Case ID | Test Case Title | Status | Priority |
|----------------|-------------|----------------|---------|----------|
| **FR1, FR14, FR21, FR27, FR33** | TC_E2E_001 | Complete User Journey Registration to Order | RETEST | HIGH |
| **FR1, FR14, FR21, FR27, FR33** | TC_E2E_002 | Register During Checkout Flow | PASS | HIGH |
| **FR1, FR14, FR21, FR27, FR33** | TC_E2E_006 | Complete Flow - Homepage to Invoice Download | RETEST | HIGH |
| **FR2, FR14, FR21, FR27** | TC_E2E_003 | Login Before Checkout Flow | PASS | HIGH |
| **FR10, FR14, FR21, FR27** | TC_E2E_004 | Search, Add to Cart, and Checkout | PASS | HIGH |
| **FR14, FR19, FR2** | TC_E2E_005 | Verify Cart Persists After Login | PASS | MEDIUM |
| **FR8, FR14, FR21, FR27** | TC_E2E_007 | Category Navigation to Purchase | PASS | MEDIUM |
| **FR13, FR14, FR21, FR27** | TC_E2E_008 | Brand Filter to Purchase | PASS | MEDIUM |

## Critical Issues Summary

### High Priority Failures:
1. **TC_PAY_001** - Payment validation missing (FR27)
2. **TC_ORDER_005** - Invoice amount incorrect (FR33)

### Medium Priority Failures:
1. **TC_CONTACT_004** - Contact form validation missing (FR39)
2. **TC_CONTACT_008** - Home button redirection issue (FR38)

### Low Priority Failures:
1. **TC_AUTH_014** - Special characters in name accepted (FR1)
2. **TC_SUB_005** - Duplicate subscription allowed (FR40)
3. **TC_NAV_013** - Non-sticky navbar (FR43)

## Coverage Analysis

### Requirements Coverage:
- **Functional Requirements (FR):** FR1-FR47 covered
- **Non-Functional Requirements (NFR):** NFR1, NFR2, NFR8, NFR9, NFR12-NFR14 covered
- **Total Requirements Covered:** 54+ requirements

### Module-wise Coverage:
- **Authentication:** 100% covered
- **Product Catalog:** 100% covered  
- **Shopping Cart:** 94% covered (1 test not executed)
- **Checkout:** 100% covered
- **Payment:** 88% covered (1 failure)
- **Order Management:** 86% covered (1 failure)
- **Contact Us:** 75% covered (2 failures)
- **Subscription:** 83% covered (1 failure)
- **Navigation & UI:** 93% covered (1 failure)
- **End-to-End:** 75% covered (2 retests needed)

## Recommendations

### Immediate Actions:
1. Fix payment validation system (TC_PAY_001)
2. Correct invoice amount calculation (TC_ORDER_005)
3. Implement contact form validation (TC_CONTACT_004)

### Testing Improvements:
1. Execute TC_CART_012 (Recommended Items feature)
2. Retest end-to-end flows (TC_E2E_001, TC_E2E_006)
3. Enhance test data for edge cases

### Overall Assessment:
The application shows strong functionality with 91.15% pass rate. Critical payment and billing issues need immediate attention before production deployment.

---

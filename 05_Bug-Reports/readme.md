# Bug Report - Automation Exercise E-commerce Website

## Executive Summary
During comprehensive testing of the Automation Exercise e-commerce website, several critical bugs were identified across multiple modules. The testing covered Authentication, Shopping Cart, Payment, Order Management, Contact Us, Subscription, and Navigation modules with 113 test cases executed.

**Overall Status:**
- **PASS:** 103 (91.15%)
- **FAIL:** 7 (6.19%)
- **RETEST:** 2 (1.77%)
- **NOT EXECUTED:** 1 (0.88%)

---

## Critical Bugs

### 1. Payment System Validation Failure
**Bug ID:** PAY-001  
**Module:** Payment  
**Priority:** HIGH  
**Test Case:** TC_PAY_001

**Description:**  
The payment form accepts invalid card details without proper validation, allowing transactions to proceed with clearly incorrect information.

**Steps to Reproduce:**
1. Complete checkout process to reach payment page
2. Enter invalid card details:
   - Card Number: "1234" (too short)
   - CVC: "99" (invalid)
   - Expiration: "01/2020" (expired)
3. Click "Pay and Confirm Order"
4. Observe payment is accepted without validation errors

**Expected Result:**  
System should reject invalid card details and display appropriate validation errors.

**Actual Result:**  
Payment system processes invalid card details without validation.

**Impact:**  
Critical security and functionality issue that could lead to fraudulent transactions and financial losses.

---

### 2. Invoice Amount Display Incorrect
**Bug ID:** ORDER-001  
**Module:** Order Management  
**Priority:** HIGH  
**Test Case:** TC_ORDER_005

**Description:**  
Downloaded invoice displays incorrect order total amount, showing "Your total purchase amount is 0" instead of the actual order value.

**Steps to Reproduce:**
1. Complete an order with known total (e.g., Rs. 2200)
2. Download invoice after successful payment
3. Open invoice.txt file
4. Check the total amount displayed

**Expected Result:**  
Invoice should display correct order total matching the actual amount paid.

**Actual Result:**  
Invoice shows "Your total purchase amount is 0" regardless of actual order value.

**Impact:**  
Critical billing issue affecting customer trust and financial record accuracy.

---

## High Priority Bugs

### 3. Contact Form Validation Missing
**Bug ID:** CONTACT-001  
**Module:** Contact Us  
**Priority:** MEDIUM  
**Test Case:** TC_CONTACT_004

**Description:**  
Contact form allows submission with empty required fields (Subject and Message), bypassing validation.

**Steps to Reproduce:**
1. Navigate to Contact Us page
2. Leave Subject and Message fields empty
3. Fill only Name and Email fields
4. Click "Submit" button

**Expected Result:**  
System should prevent form submission and show validation errors for empty required fields.

**Actual Result:**  
Form submits successfully without validation for Subject and Message fields.

**Impact:**  
Poor data quality and potential spam submissions.

---

### 4. Home Button Redirection Issue
**Bug ID:** CONTACT-002  
**Module:** Contact Us  
**Priority:** MEDIUM  
**Test Case:** TC_CONTACT_008

**Description:**  
After contact form submission, the Home button does not redirect to homepage as expected.

**Steps to Reproduce:**
1. Submit contact form with valid data
2. Success message is displayed
3. Click "Home" button

**Expected Result:**  
User should be redirected to homepage.

**Actual Result:**  
System displays success message but Home button functionality is inconsistent.

**Impact:**  
Poor user experience and navigation flow disruption.

---

## Medium Priority Bugs

### 5. Duplicate Subscription Allowed
**Bug ID:** SUB-001  
**Module:** Subscription  
**Priority:** LOW  
**Test Case:** TC_SUB_005

**Description:**  
Newsletter subscription system allows duplicate subscriptions with the same email address without notification.

**Steps to Reproduce:**
1. Subscribe to newsletter with email "existing@test.com"
2. Attempt to subscribe again with the same email
3. Observe system response

**Expected Result:**  
System should show "already subscribed" message or handle duplicates gracefully.

**Actual Result:**  
System allows duplicate subscription without warning.

**Impact:**  
Database clutter and potential spam concerns.

---

### 6. Special Characters in Name Field
**Bug ID:** AUTH-001  
**Module:** Authentication  
**Priority:** LOW  
**Test Case:** TC_AUTH_014

**Description:**  
Registration system accepts special characters in name field without validation, posing potential security risks.

**Steps to Reproduce:**
1. Navigate to registration page
2. Enter name with special characters: "Test@#$%User"
3. Complete registration with valid email
4. Observe system acceptance

**Expected Result:**  
System should validate name field and reject or sanitize special characters.

**Actual Result:**  
System accepts names with special characters without validation.

**Impact:**  
Potential security vulnerability and data integrity issues.

---

### 7. Non-Sticky Navigation Bar
**Bug ID:** NAV-001  
**Module:** Navigation & UI  
**Priority:** LOW  
**Test Case:** TC_NAV_013

**Description:**  
Navigation bar does not remain visible (sticky) while scrolling down the page.

**Steps to Reproduce:**
1. Navigate to any page on the website
2. Scroll down the page
3. Observe navigation bar behavior

**Expected Result:**  
Navigation bar should remain fixed/sticky at the top during scrolling.

**Actual Result:**  
Navigation bar scrolls away with content.

**Impact:**  
Reduced user convenience and navigation efficiency.

---

## Features Not Implemented

### 8. Recommended Items Section Missing
**Bug ID:** CART-001  
**Module:** Shopping Cart  
**Priority:** LOW  
**Test Case:** TC_CART_012

**Description:**  
"RECOMMENDED ITEMS" section mentioned in test cases is not present on the website.

**Impact:**  
Missing feature affects user experience and potential sales opportunities.

---

## Retest Required

### 9. End-to-End Flow Issues
**Test Cases:** TC_E2E_001, TC_E2E_006

**Description:**  
Complete user journey tests require retesting due to minor errors encountered during initial execution, particularly related to invoice amount discrepancies.

---

## Recommendations

### Immediate Actions (High Priority):
1. Fix payment validation system to reject invalid card details
2. Correct invoice total calculation and display
3. Implement proper form validation for contact form

### Short-term Actions (Medium Priority):
1. Fix Home button redirection functionality
2. Implement duplicate subscription prevention
3. Add input validation for special characters in name fields

### Long-term Improvements:
1. Implement sticky navigation bar
2. Add recommended items section if intended feature
3. Enhance overall input validation across all forms

---

## Environment Details
- **Browser:** Chrome (latest)
- **Test Date:** November 16-18, 2025
- **Website:** https://automationexercise.com
- **Tester:** Monish Parulekar

---

*This bug report generated based on comprehensive test execution results.*

# **E-Commerce Website (automationexercise.com) – Requirements Document**

## **1. Project Overview**

This document describes the core functional and non-functional requirements of the e-commerce application hosted at **automationexercise.com**.  
The goal is to define clear testing scope and features for manual testing.

**Application Under Test:** https://automationexercise.com  
**Document Version:** 1.0  
**Last Updated:** November 16, 2025  
**Prepared By:** Monish Parulekar

---

## **2. Functional Requirements**

### **2.1 User Account Module**

| ID | Requirement |
|----|-------------|
| FR1 | User should be able to register with valid details (name, email, password) |
| FR2 | User should be able to log in using email & password |
| FR3 | User should be able to log out successfully |
| FR4 | User should recover a password using "Forgot Password" feature |
| FR5 | User should be able to update profile information |
| FR6 | System should prevent duplicate email registration |
| FR7 | System should validate email format during registration |

---

### **2.2 Product Catalog Module**

| ID | Requirement |
|----|-------------|
| FR8 | User should be able to view product categories (Men, Women, Kids) |
| FR9 | User should be able to view individual product details |
| FR10 | User should be able to search products using keywords |
| FR11 | User should be able to filter/sort products based on Categories and Brand names  |
| FR12 | User should see product price, description, availability, and image |
| FR13 | User should be able to navigate between product categories |

---

### **2.3 Cart Module**

| ID | Requirement |
|----|-------------|
| FR14 | User should be able to add product to cart |
| FR15 | User should be able to view cart summary with all added items |
| FR16 | User should be able to update product quantity in cart |
| FR17 | User should be able to remove product from cart |
| FR18 | Cart should show accurate total price calculation |
| FR19 | Cart should persist items during the session |
| FR20 | User should see cart item count in header |

---

### **2.4 Checkout Module**

| ID | Requirement |
|----|-------------|
| FR21 | User should be able to proceed to checkout from cart |
| FR22 | User should be able to enter shipping & billing details |
| FR23 | User should be able to review order summary before payment |
| FR24 | User should be able to add comments/notes to order |
| FR25 | User should be able to confirm the order |
| FR26 | System should validate required checkout fields |

---

### **2.5 Payment Module**

| ID | Requirement |
|----|-------------|
| FR27 | User should be able to enter payment card details |
| FR28 | User should be able to simulate payment processing |
| FR29 | System should display order confirmation message after successful payment |
| FR30 | User should receive order confirmation number |

---

### **2.6 Order Module**

| ID | Requirement |
|----|-------------|
| FR31 | User should be able to view order history in account |
| FR32 | User should be able to view order details |
| FR33 | User should be able to download invoice |
| FR34 | User should receive email confirmation |

---

### **2.7 Contact Us Module**

| ID | Requirement |
|----|-------------|
| FR35 | User should be able to access Contact Us page |
| FR36 | User should be able to submit contact form with required fields |
| FR37 | User should be able to upload a file attachment |
| FR38 | User should receive success message after form submission |
| FR39 | System should validate contact form fields |

---

### **2.8 Subscription Module**

| ID | Requirement |
|----|-------------|
| FR40 | User should be able to subscribe to newsletter |
| FR41 | User should see subscription confirmation message |
| FR42 | System should validate email format for subscription |

---

### **2.9 UI & Navigation**

| ID | Requirement |
|----|-------------|
| FR43 | User should navigate pages via navbar/footer |
| FR44 | Website should maintain consistent layout & branding across pages |
| FR45 | All pages should load correctly without broken links |
| FR46 | User should see breadcrumb navigation on product pages |
| FR47 | Footer should contain all relevant links and information |

---

## **3. Non-Functional Requirements**

### **3.1 Performance**

| ID | Requirement |
|----|-------------|
| NFR1 | Pages should load within 3–5 seconds under normal conditions |
| NFR2 | Search results should return within 2 seconds |
| NFR3 | Cart operations should respond within 1 second |

### **3.2 Usability**

| ID | Requirement |
|----|-------------|
| NFR4 | Buttons & links should be clearly visible and labeled |
| NFR5 | Error messages should be readable and helpful |
| NFR6 | Form fields should have appropriate labels and placeholders |
| NFR7 | User interface should be intuitive and easy to navigate |

### **3.3 Compatibility**

| ID | Requirement |
|----|-------------|
| NFR8 | Website should work on Chrome, Firefox, Edge, Safari |
| NFR9 | Site should be responsive on mobile devices (iOS/Android) |
| NFR10 | Website should function properly on tablet devices |
| NFR11 | Website should support minimum screen resolution of 1024x768 |

### **3.4 Security**

| ID | Requirement |
|----|-------------|
| NFR12 | Password fields must be masked (hidden characters) |
| NFR13 | Login should validate and reject incorrect credentials |
| NFR14 | System should prevent SQL injection in input fields |
| NFR15 | Session should timeout after period of inactivity |

### **3.5 Accessibility**

| ID | Requirement |
|----|-------------|
| NFR16 | Website should have proper alt text for images |
| NFR17 | Website should be keyboard navigable |
| NFR18 | Forms should have proper ARIA labels |

---

## **4. Test Environment Requirements**

* **Browser:** Chrome (latest), Firefox (latest), Edge (latest)
* **Operating System:** Windows 10/11, macOS, Linux
* **Mobile Devices:** iOS Safari, Android Chrome
* **Internet Connection:** Stable broadband connection (minimum 2 Mbps)
* **Test Data:** Valid email addresses for registration and testing

---

## **5. Out of Scope**

* Payment gateway integration with real money transactions
* Backend API testing
* Performance/stress/load testing
* Database testing
* Security penetration testing
* Third-party integrations testing

---

## **6. Assumptions**

* Website is stable and publicly accessible at all times
* Payment flow is simulated, not processing real transactions
* Test data is not persisted long term and may be cleared
* Website is hosted on a test/demo environment
* No authentication required to access public pages
* All features mentioned are available and functional

---

## **7. Dependencies**

* Stable internet connection required for testing
* Access to valid email accounts for registration testing
* Browser compatibility requirements met
* Website uptime and availability

---

## **8. Constraints**

* Testing limited to manual test execution only
* No access to backend systems or databases
* Cannot modify website configuration or settings
* Limited to functional and UI testing only

---

## **9. Acceptance Criteria**

A requirement is considered met when:
* Feature works as described in the requirement
* No critical bugs are found during testing
* Feature is accessible across supported browsers
* Feature meets usability standards
* Error handling works appropriately

A requirement is considered not met when:
* Feature does not exist or is not implemented
* Feature exists but has critical defects
* Feature fails on supported browsers/devices
* Feature does not meet usability standards

Note: Requirements marked as "not met" will be documented in the Test Summary Report with appropriate justification (missing feature, blocked, or defect found).


---

## **10. Glossary**

| Term | Definition |
|------|------------|
| FR | Functional Requirement |
| NFR | Non-Functional Requirement |
| UI | User Interface |
| UX | User Experience |
| AUT | Application Under Test |
| RTM | Requirements Traceability Matrix |

---

**Document Status:** Approved for Testing  
**Next Steps:** Proceed with Test Plan creation based on these requirements


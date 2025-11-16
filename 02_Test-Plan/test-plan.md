# **Test Plan - E-Commerce Website**

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
This test plan outlines the strategy, scope, resources, schedule, and activities required to conduct manual testing of the e-commerce website. The purpose is to ensure the application meets all functional and non-functional requirements before release.

### **1.2 Scope**
This test plan covers manual functional testing, UI/UX testing, usability testing, and basic compatibility testing of the e-commerce application.

### **1.3 Objectives**
- Verify all functional requirements are implemented correctly
- Identify defects and missing functionality
- Ensure application meets quality standards
- Validate user workflows end-to-end
- Test across multiple browsers and devices
- Document all test results and defects

---

## **2. Test Items (Features to be Tested)**

| Module | Features |
|--------|----------|
| **User Account** | Registration, Login, Logout, Profile Update, Password Recovery |
| **Product Catalog** | Product Browse, Search, Filter, Category Navigation, Product Details |
| **Shopping Cart** | Add to Cart, View Cart, Update Quantity, Remove Items, Cart Calculation |
| **Checkout** | Shipping Details, Billing Details, Order Review, Order Confirmation |
| **Payment** | Payment Information Entry, Payment Processing, Order Confirmation |
| **Order Management** | Order History, Order Details, Invoice Download |
| **Contact Us** | Contact Form Submission, File Upload, Success Message |
| **Subscription** | Newsletter Subscription, Email Validation |
| **Navigation** | Header Navigation, Footer Links, Breadcrumbs, Page Loading |

---

## **3. Features Not to be Tested (Out of Scope)**

- Backend API testing
- Database testing
- Performance/Load/Stress testing
- Security penetration testing
- Real payment gateway integration
- Email server functionality
- Mobile app testing (only mobile browser)
- Accessibility compliance testing (WCAG)
- Internationalization/Localization
- Third-party integrations

---

## **4. Testing Approach**

### **4.1 Test Levels**
- **Functional Testing:** Verify each feature works as per requirements
- **Integration Testing:** Verify modules work together (e.g., Cart → Checkout → Payment)
- **UI Testing:** Verify layout, design, responsiveness
- **Usability Testing:** Verify ease of use and user experience
- **Compatibility Testing:** Verify cross-browser and cross-device functionality

### **4.2 Test Types**

| Test Type | Description |
|-----------|-------------|
| **Smoke Testing** | Quick validation of critical functionalities |
| **Functional Testing** | Detailed testing of all features against requirements |
| **Exploratory Testing** | Ad-hoc testing to discover undocumented issues |
| **Positive Testing** | Test with valid inputs and expected user behavior |
| **Negative Testing** | Test with invalid inputs and unexpected scenarios |
| **Boundary Testing** | Test input limits and edge cases |
| **End-to-End Testing** | Test complete user journeys (browse → purchase) |

**Note:** Regression testing is not applicable as this is a one-time testing cycle on a live website without access to bug fixes or deployments.

### **4.3 Test Design Techniques**
- Equivalence Partitioning
- Boundary Value Analysis
- Decision Table Testing
- State Transition Testing
- Error Guessing

---

## **5. Test Environment**

### **5.1 Hardware Requirements**
- Desktop/Laptop with minimum 4GB RAM
- Mobile devices (Android/iOS) for responsive testing
- Tablet devices for medium screen testing

### **5.2 Software Requirements**

| Component | Specification |
|-----------|---------------|
| **Browsers** | Chrome (latest), Firefox (latest), Edge (latest), Safari (latest) |
| **Operating Systems** | Windows 10/11, macOS, Linux Ubuntu |
| **Mobile OS** | Android 10+, iOS 14+ |
| **Internet Connection** | Minimum 2 Mbps stable connection |
| **Screen Resolutions** | 1920x1080, 1366x768, 768x1024 (tablet), 375x667 (mobile) |

### **5.3 Test Data Requirements**
- Valid email addresses for registration
- Test credit card details (site allows dummy card details)
- Sample product data
- Contact form test data
- Invalid data sets for negative testing

---

## **6. Entry and Exit Criteria**

### **6.1 Entry Criteria**
- Requirements document reviewed and approved
- Test plan reviewed and approved
- Test cases written and reviewed
- Test environment is set up and accessible
- Application is deployed and stable
- Test data is prepared
- Testers have access to the application

### **6.2 Exit Criteria**
- All planned test cases executed
- At least 95% test case pass rate achieved
- No critical or high severity bugs open
- All medium severity bugs reviewed and accepted/fixed
- Test summary report completed
- Stakeholder sign-off received

---

## **7. Test Deliverables**

### **7.1 Before Testing**
- Requirements Document
- Test Plan Document
- Test Scenarios Document
- Test Cases Document
- Requirements Traceability Matrix (RTM)

### **7.2 During Testing**
- Test execution status reports
- Bug reports
- Test logs
- Screenshots/videos of defects

### **7.3 After Testing**
- Test Summary Report
- Updated RTM with test results
- Bug reports (all defects found)
- Lessons learned document

---

## **8. Test Schedule**

**Note:** *The timeline below is an estimated schedule for planning purposes. As this is a portfolio project, the actual execution timeline may vary based on availability and learning pace.*

| Phase | Activity | Estimated Duration | 
|-------|----------|-------------------|
| **Phase 1** | Requirements Analysis | 2 days |
| **Phase 2** | Test Planning | 2 days |
| **Phase 3** | Test Scenario & Case Design | 3 days |
| **Phase 4** | Test Environment Setup | 1 day |
| **Phase 5** | Test Execution (Round 1) | 5 days |
| **Phase 6** | Bug Reporting & Documentation | 3 days |
| **Phase 7** | Test Summary & Sign-off | 2 days |

**Total Estimated Duration:** ~18 working days (3.5 weeks)

**Note:** Regression testing and bug retesting are not included as this is a portfolio project on a live website where bugs cannot be fixed or retested.

---

## **9. Test Team & Responsibilities**

| Role | Responsibilities |
|------|------------------|
| **Test Lead** | Overall test planning, strategy, and coordination |
| **Test Engineer** | Test case design, test execution, defect reporting |
| **Test Analyst** | Requirements analysis, test scenario creation |
| **Documentation** | Creating test deliverables and reports |

**All roles performed by:** Monish Parulekar - QA Engineer (Portfolio Project)

---

## **10. Risks and Mitigation**

**Note:** *Risks here are identified based on testing a live public website without dev/bug fixing access.*

| Risk | Impact | Probability | Mitigation Strategy |
|------|--------|-------------|---------------------|
| Website downtime or unavailability | High | Low | Test during different times of day, document unavailability |
| Browser compatibility issues | Medium | Medium | Test on multiple browsers early in test cycle |
| Test accounts getting deleted/expired | Medium | Medium | Create fresh test accounts as needed, use temporary email |
| Test data persistence issues | Low | Medium | Accept that data may be cleared, document state at test time |
| Missing or unimplemented features | Medium | High | Document as "feature not available" in bug reports |
| Unclear requirements (no documentation) | Medium | High | Make reasonable assumptions based on standard e-commerce flows |
| Internet connectivity issues | Medium | Low | Ensure stable connection, test during off-peak hours |
| Website updates during testing | Low | Low | Note version/date of testing, retest if major changes observed |

---

## **11. Bug Reporting Process**

### **11.1 Bug Severity Levels**

| Severity | Definition | Example |
|----------|------------|---------|
| **Critical** | Application crash, data loss, security breach | Cannot complete checkout, site crashes |
| **High** | Major feature not working, blocking user flow | Login fails, cannot add to cart |
| **Medium** | Feature works but with issues, workaround available | Quantity update missing, incorrect total |
| **Low** | Minor UI issues, cosmetic defects | Spelling error, alignment issue |

### **11.2 Bug Lifecycle (For Reference)**

In a real project, bugs would follow this lifecycle:
1. **New** → Bug reported by tester
2. **Assigned** → Bug assigned to developer
3. **Open** → Developer working on fix
4. **Fixed** → Developer claims fix is ready
5. **Retest** → Tester verifies the fix
6. **Closed** → Bug verified as fixed
7. **Reopened** → Bug still exists after fix attempt

**Note:** In this portfolio project, all identified bugs will remain in "New" status as there is no development team to fix them. Bugs are documented for demonstration purposes only.

---

## **12. Test Metrics**

The following metrics will be tracked and reported:

- **Total Test Cases:** Number of test cases written
- **Test Cases Executed:** Number of test cases run
- **Test Cases Passed:** Number of successful test cases
- **Test Cases Failed:** Number of failed test cases
- **Test Cases Blocked:** Number of blocked test cases
- **Defects Found:** Total bugs identified
- **Defects by Severity:** Count per severity level
- **Defect Density:** Defects per module
- **Test Coverage:** % of requirements tested
- **Pass Percentage:** (Passed / Executed) × 100

---

## **13. Suspension and Resumption Criteria**

### **13.1 Suspension Criteria**
Testing will be suspended if:
- Critical environment issues prevent testing
- More than 50% of smoke tests fail
- Application is unstable or frequently crashes
- Test-blocking defects are found
- Major requirement changes occur

### **13.2 Resumption Criteria**
Testing will resume when:
- Environment issues are resolved
- Blocking defects are fixed
- Application stability is restored
- Updated requirements are documented

---

## **14. Assumptions**

- Website is accessible 24/7 during test period
- Test accounts can be created as needed
- Payment flow uses test/demo mode
- Test data can be cleared/reset if needed
- No major feature changes during testing
- Internet connectivity is stable
- Browsers are up-to-date

---

## **15. Dependencies**

- Stable test environment
- Access to the application
- Availability of test team
- Timely bug fix turnaround
- Stakeholder availability for clarifications

---

## **16. Approvals**

| Role | Status |
|------|--------|
| **Test Plan Prepared By** | Monish Parulekar - QA Engineer |
| **Document Status** | Self-Reviewed and Approved for Portfolio Use |
| **Date** | November 16, 2025 |

---

## **17. Glossary**

| Term | Definition |
|------|------------|
| **AUT** | Application Under Test |
| **RTM** | Requirements Traceability Matrix |
| **UAT** | User Acceptance Testing |
| **GUI** | Graphical User Interface |
| **E2E** | End-to-End Testing |
| **P0/P1/P2** | Priority levels (P0=Critical, P1=High, P2=Medium, P3=Low) |

---

**Document Status:** Approved for Test Execution  
**Next Steps:** Proceed with Test Scenarios and Test Case Design

---

**End of Test Plan Document**

# Manual Testing Portfolio - E-Commerce Application

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Testing Type](https://img.shields.io/badge/Testing-Manual-blue.svg)](https://github.com)
[![Status](https://img.shields.io/badge/Status-Complete-success.svg)](https://github.com)

## Project Overview

This repository demonstrates comprehensive **manual testing** documentation for an e-commerce web application. The project showcases the complete QA lifecycle from requirements analysis to test summary reporting, including bug tracking using industry-standard tools.

**Application Under Test:** [automationexercise.com](https://automationexercise.com)  
**Project Type:** Manual Functional Testing Portfolio  
**Testing Approach:** Black-box testing with comprehensive test documentation  
**Duration:** Self-paced

---

## Project Objectives

- Document requirements based on industry-standard e-commerce functionality
- Create comprehensive test plan and testing strategy
- Design detailed test scenarios and test cases covering all modules
- Execute manual testing and identify defects
- Perform gap analysis (expected vs actual functionality)
- Use JIRA for professional bug tracking and management
- Generate test summary report with metrics and findings

---

## Repository Structure

```
manual-testing-ecommerce-app/
│
├── 01_Requirements/
│   └── requirements.md              # 42 Functional + 18 Non-functional requirements
│
├── 02_Test_Plan/
│   └── test_plan.md                 # Complete test planning document
│
├── 03_Test_Scenarios/
│   └── test_scenarios.md            # 96 high-level test scenarios
│
├── 04_Test_Cases/
│   ├── test_cases.xlsx              # 113 detailed test cases (primary)
│   └── test_cases_summary.md        # Sample test cases for GitHub preview
│
├── 05_Bug_Reports/
│   ├── bug_reports.md               # Bug summary with JIRA links
│   ├── jira_export.csv              # Exported bugs from JIRA
│   └── screenshots/                 # Bug evidence and screenshots
│       ├── bug_ecom1_invoice.png
│       ├── bug_ecom2_cart.png
│       └── ...
│
├── 06_RTM/
│   └── rtm.xlsx                     # Requirements Traceability Matrix
│
├── 07_Test_Summary_Report/
│   └── summary_report.md            # Executive summary and metrics
│
└── README.md                        # This file
```

---

## Testing Scope

### **Modules Tested:**

| Module | Test Cases | Priority Distribution |
|--------|------------|----------------------|
| **User Authentication** | 15 | High: 5, Medium: 8, Low: 2 |
| **Product Catalog** | 18 | High: 5, Medium: 11, Low: 2 |
| **Shopping Cart** | 16 | High: 7, Medium: 7, Low: 2 |
| **Checkout Process** | 12 | High: 10, Medium: 1, Low: 1 |
| **Payment** | 8 | High: 5, Medium: 3, Low: 0 |
| **Order Management** | 7 | High: 5, Medium: 2, Low: 0 |
| **Contact Us** | 8 | High: 2, Medium: 4, Low: 2 |
| **Newsletter Subscription** | 6 | High: 0, Medium: 5, Low: 1 |
| **Navigation & UI** | 15 | High: 4, Medium: 7, Low: 4 |
| **End-to-End Workflows** | 8 | High: 6, Medium: 2, Low: 0 |
| **TOTAL** | **113** | **49 High, 50 Medium, 14 Low** |

### **Testing Types Performed:**

- **Functional Testing** - Verify features work as per requirements
- **UI/UX Testing** - Verify layout, design, and responsiveness
- **Negative Testing** - Test with invalid inputs and error scenarios
- **Boundary Testing** - Test input limits and edge cases
- **End-to-End Testing** - Test complete user journeys
- **Compatibility Testing** - Cross-browser (Chrome, Firefox, Edge)
- **Exploratory Testing** - Ad-hoc testing to discover issues

---

## Tools & Technologies

| Category | Tools Used | Purpose |
|----------|------------|---------|
| **Test Documentation** | Markdown, Microsoft Excel | Test cases, scenarios, requirements |
| **Bug Tracking** | JIRA Cloud | Defect logging and management |
| **Version Control** | Git, GitHub | Documentation version control |
| **Browsers Tested** | Chrome 119+, Firefox 120+, Edge 119+ | Cross-browser compatibility |
| **Test Management** | Excel Spreadsheets | Test case execution tracking |
| **Screenshots** | Snipping Tool, Browser DevTools | Bug evidence capture |

**Note:** This is a manual testing portfolio project. In a professional environment, I would integrate with CI/CD pipelines and potentially use Selenium for automation.

---

## Testing Approach

### **Requirements vs Reality:**

This project intentionally documents requirements based on **industry-standard e-commerce best practices**, representing what a complete e-commerce application should have. During testing, I performed **gap analysis** to identify:

1. **Working features** that meet requirements 
2. **Broken features** that exist but have defects
3. **Missing features** that should exist but aren't implemented

This approach demonstrates:
- Understanding of complete business requirements
- Ability to identify gaps between expected and actual functionality
- Differentiation between defects and missing features
- Real-world testing scenario where requirements often exceed implementation

---

## Sample Test Case

**Test Case ID:** TC_AUTH_001  
**Module:** Authentication  
**Title:** Register User with Valid Details  
**Priority:** High  
**Test Type:** Positive  

**Preconditions:**
- Browser is open
- Valid unique email available

**Test Steps:**
1. Navigate to https://automationexercise.com
2. Click "Signup / Login" button
3. Enter Name: "Test User"
4. Enter Email: "testuser@test.com"
5. Click "Signup" button
6. Fill all registration details
7. Click "Create Account" button
8. Verify "ACCOUNT CREATED!" message is displayed
9. Click "Continue" button
10. Verify "Logged in as Test User" is visible in header

**Expected Result:**  
Account is created successfully. User is logged in with username displayed in header.

**Actual Result:**  
PASS - Account created and user logged in as expected.

**See full test cases:** [test_cases.xlsx](./04_Test_Cases/test_cases.xlsx)

---

## Contact & Feedback

**Portfolio Owner:** Monish Parulekar  
**Role:** QA Engineer / Manual Tester  
**Email:** parulekarmonish@gmail.com

**Open to:**
- QA Engineer roles
- Software Tester positions
- Manual Testing opportunities
- Quality Assurance positions


---

**End of README**

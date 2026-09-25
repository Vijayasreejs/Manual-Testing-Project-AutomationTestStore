# Automation Test Store - QA Test Suite Documentation

Welcome to the Quality Assurance test documentation repository for the **Automation Test Store (Demo Web Store)**[cite: 2, 3]. This repository contains all formal test plans, execution summaries, bug reports, and sign-off artifacts resulting from manual testing.

---

## 📌 Project Overview

* **Application Under Test:** Automation Test Store (Demo Web Store)[cite: 2, 3]
* **Document Version:** 1.0[cite: 2, 4]
* **Test Cycle Date:** April 2026[cite: 2, 3, 4]
* **Prepared By:** Vijayasree JS (QA Tester)[cite: 2, 3]
* **Sign-off / Approver:** Subin P John (Project Manager)[cite: 2, 3]
* **Execution Type:** Manual Functional Testing[cite: 2, 3]

---

## 📊 Key Execution Metrics

| Metric | Detail / Value | Notes |
| :--- | :--- | :--- |
| **Modules Covered** | **6** | Registration, Authentication, Search, Cart, Checkout, UI[cite: 2, 4] |
| **Total Test Cases Executed** | **120** | 20 test cases per module[cite: 2, 4] |
| **Passed** | **106** | **88.3% Pass Rate**[cite: 4] |
| **Failed** | **13** | Logged as defects[cite: 4] |
| **Blocked** | **1** | Unimplemented feature (`UI_16`)[cite: 4] |
| **Total Defects Logged** | **14** | `BUG-001` to `BUG-014`[cite: 3, 4] |

### Defect Severity Breakdown

* 🚨 **Critical:** **1** (Oversell risk at Checkout)[cite: 3, 4]
* ⚠️ **High:** **3** (Account lockout, post-logout caching, out-of-stock cart addition)[cite: 3, 4]
* 🟡 **Medium:** **4** (Form validation & localization issues)[cite: 3, 4]
* 🟢 **Low:** **6** (Usability gaps & missing enhancements)[cite: 3, 4]

---

## 📂 Repository Structure & Artifacts

.
├── Bug_Report.xlsx                  # Defect tracking sheet with reproduction steps and logs
├── README.md                        # Project overview and test documentation guide
├── Test_Plan.pdf                    # Test strategy, scope, environment, entry/exit criteria
├── Test_Signoff.pdf                 # Formal QA sign-off decision & open risk statement
└── Test_Summary_Report.pdf          # Detailed metrics, key findings, and recommendations


### 📄 Included Deliverables

1. **`Test_Plan.pdf`**
   Defines the testing approach, scope (in-scope / out-of-scope), environment configurations, risk assessments, and schedule[cite: 2].
2. **`Test_Summary_Report.pdf`**
   Summarizes test execution results, module-level pass/fail rates, key strengths, security/functional findings, and QA recommendations[cite: 2, 4].
3. **`Test_Signoff.pdf`**
   Captures sign-off decision status, open critical/high risks, and stakeholder approval blocks[cite: 3].
4. **`Bug_Report.xlsx`**
   Contains detailed defect descriptions, steps to reproduce, severity/priority ratings, and test case mappings[cite: 2, 4].

---

## 🔍 Module-Wise Results Summary

| Module | Planned / Executed | Passed | Failed | Blocked | Pass Rate |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Registration** | 20 | 18 | 2 | 0 | 90.0%[cite: 4] |
| **Authentication** | 20 | 17 | 3 | 0 | 85.0%[cite: 4] |
| **Search** | 20 | 18 | 2 | 0 | 90.0%[cite: 4] |
| **Cart** | 20 | 18 | 2 | 0 | 90.0%[cite: 4] |
| **Checkout** | 20 | 18 | 2 | 0 | 90.0%[cite: 4] |
| **User Interface** | 20 | 17 | 2 | 1 | 85.0%[cite: 4] |

---

## 🚨 Top Outstanding Issues (Release Blockers)

The following Critical and High severity defects are currently **Open** and require developer resolution before full release sign-off[cite: 3, 4]:

1. **BUG-010 (Critical):** Checkout completes successfully even if item stock is zeroed out concurrently (overselling risk)[cite: 3, 4].
2. **BUG-003 (High):** Missing account lockout after multiple consecutive failed login attempts (brute-force security risk)[cite: 3, 4].
3. **BUG-005 (High):** Cached account page briefly renders when pressing the browser 'Back' button after logging out[cite: 3, 4].
4. **BUG-008 (High):** Out-of-stock items can be added to the cart without warning or button restriction[cite: 3, 4].

---

## 🏷️ Test Environment

* **Application:** Automation Test Store (Demo Web Store)[cite: 2]
* **Environment:** Demo / QA[cite: 2]
* **Browsers Tested:** Google Chrome, Mozilla Firefox, Apple Safari, Microsoft Edge (Latest Stable)[cite: 2]
* **Viewports:** Desktop, Tablet (768px), Mobile (375px)[cite: 2]

---

## 🛑 Sign-Off Status

> **Recommendation:** **Not Approved for Unconditional Release**[cite: 3].
> Full sign-off is pending until 1 Critical (`BUG-010`) and 3 High severity defects (`B

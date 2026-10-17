# DAY 3 – SOFTWARE TESTING INTERNSHIP TASK

## TOPIC 1: STLC STUDY

### STLC (Software Testing Life Cycle)

**Definition:** STLC is a step-by-step process used to test and validate software or an application.

**Objective of Testing:** To identify defects and help deliver a quality product to the client.

## 1. Requirement Analysis

- Understand and analyze the requirements or user story.
- Identify what needs to be tested.
- Ask for clarification if requirements are unclear.

## 2. Test Planning

- Decide the testing approach, scope, time, and resources.
- The Test Lead usually leads test planning.
- The tester may also participate in planning.

## 3. Test Case Design

- Identify test scenarios.
- Write test cases.
- Review test cases.
- Fix comments received during review.
- Get approval from the Senior QA or Test Lead.

### Types of Review

- **Self Review:** Reviewing our own test cases.
- **Peer Review:** Team members review the test cases.
- **Senior Review:** Senior team members review the test cases.

---

# REQUIREMENT TRACEABILITY MATRIX (RTM)

## Definition

RTM is a document used to map requirements with test cases. It helps track whether all requirements are covered by testing.

### Objectives of RTM

- Every requirement should be covered by test cases.
- Track the testing coverage of requirements.
- Identify requirements that have not been tested.

## A. Forward Traceability Matrix

**Purpose:** Maps requirements to test cases. It is generally prepared before test execution.

| Req ID | Requirement Description | TC01 | TC02 | TC03 |
|---|---|:---:|:---:|:---:|
| RE01 | SignUp Page | ✓ | | |
| RE02 | Login Page | | ✓ | |
| RE03 | Profile Page | | ✓ | ✓ |

**Key Point:** Each requirement should be mapped to at least one relevant test case.

## B. Backward Traceability Matrix

**Purpose:** Checks which requirements are covered by the test cases. Execution results can also be recorded after test execution.

| Test Case ID | Test Case Description | Req1 | Req2 | Req3 | Status | Defect ID |
|---|---|:---:|:---:|:---:|---|---|
| TC312 | Verification of Signup | | ✓ | | Pass | - |
| TC313 | Verification of Login | ✓ | | | Pass | - |
| TC314 | Verification of Homepage | | | ✓ | Fail | ABC-123 |
| TC315 | End-to-End Flow | ✓ | ✓ | ✓ | Fail | ABC-124 |

**Key Point:** It helps check whether test cases are linked to the correct requirements.

## C. Bi-Directional Traceability Matrix

**Purpose:** Combines forward and backward traceability to track requirements and their related test cases.

| Req ID | Requirement Description | TC01 | TC02 | TC03 | TC04 | TC05 | TC06 | Status | Defect ID |
|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|---|
| PTM-01 | SignUp Page | ✓ | | | | ✓ | | Pass | - |
| PTM-02 | Login Page | | | ✓ | | ✓ | | Pass | - |
| PTM-03 | Recharge Module | | | | | ✓ | | Fail | ABC-123 |
| PTM-04 | Flight Booking | | ✓ | | | | | Fail | ABC-124 |
| PTM-05 | Bus Booking | | | | | | ✓ | Pass | - |

**Key Point:** It helps track requirements in both directions and identify gaps in test coverage.

---

## 4. Test Execution

- Execute the prepared test cases.
- Compare actual results with expected results.
- Mark test cases as Pass or Fail.
- Report defects when actual results do not match expected results.

## 5. Defect/Bug Reporting and Tracking

- Report defects using a tool such as JIRA.
- Add defect details and steps to reproduce.
- Track the defect status.
- Retest after the developer fixes the defect.
- Perform regression testing when required.

---

# REPORTS AND DOCUMENTATION

## A. Test Summary Report

**Definition:** A Test Summary Report gives an overview of the testing performed and its results.

### Information Included

- Number of test cases executed.
- Pass, Fail, Blocked, Incomplete, Work in Progress, and Skipped status, as applicable.
- Execution date and time.
- Defect IDs and remarks.

### Test Summary Report Table

| Sr. No. | Test Case ID | Test Case Name | Prepared By | Reviewed By | Tester Name | Execution Date & Time | Status | Defect ID | Remark |
|---:|---|---|---|---|---|---|---|---|---|
| 1 | TC01 | Verification of Login Page | Dhananjay | Prajakt | Akshay | 03 Nov, 8:47 AM | Pass | - | Working fine |
| 2 | TC02 | Verification of Signup Page | Dhananjay | Prajakt | Akshay | 03 Nov, 9:15 AM | Fail | VCTC-01 | Bug raised in JIRA |

## B. Defect Summary Report

**Definition:** A Defect Summary Report gives details about defects found during testing and their current status.

### Information Included

- Defect ID.
- Defect description.
- Linked test case.
- Person who reported the defect.
- Defect status.
- Person assigned to fix it.

### Defect Summary Report Table

| Sr. No. | Defect ID | Defect Description | Linked Test Case | Raised By | Status | Assigned To |
|---:|---|---|---|---|---|---|
| 1 | VCTC-99 | ABCD test failure | TC312 | Dhananjay | In Progress | Nikhil |
| 2 | VCTC-100 | Login button not working | TC02 | Akshay | Open | Rahul |

---

## DAY 3 – LEARNING SUMMARY

Today, I studied the Software Testing Life Cycle (STLC), including Requirement Analysis, Test Planning, Test Case Design, Test Execution, and Test Closure. I also learned about RTM, its types, defect tracking, Test Summary Reports, and Defect Summary Reports.
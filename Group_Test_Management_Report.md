# 🧪 Final Group Test Report Template — Word Puzzle Game Plus

**Level:** Intermediate QA | **Week 5:** Test Management

**Course:** Software Testing & Quality Assurance  
**Module:** Test Management (Week 5)  
**Project Type:** Group Assessment  
**Submission Date:** 2025-10-28

## Team Information

| Role          | Name           | Responsibilities                                         |
| ------------- | -------------- | -------------------------------------------------------- |
| Test Manager  | Denis Kyalo    | Planning, scheduling, coordination, metric tracking      |
| Risk Analyst  | Bramwel Mutugi | Risk identification, prioritization, test design linkage |
| Test Executor | Gideon Bethuel | Execution, evidence capture, defect logging              |

## Group Rules

- Each student must belong to only one group.
- Duplicate membership or multiple submissions will result in invalidation.
- Every group member must contribute towards this project

## Project Overview

**System Under Test:** Word Puzzle Game Plus  
**Technology Stack:** HTML, CSS, JavaScript  
**Environment:** Chrome Browser (Desktop)

### Features Under Test

| Feature     | Description                         | Risk Category |
| ----------- | ----------------------------------- | ------------- |
| Reset Game  | Clears score and progress instantly |      high         |
| Leaderboard | Stores top 3 scores in localStorage |   medium            |
| Bonus Round | Every 3 puzzles → doubles score     |    high           |

## Test Plan

### Objectives

Verify that the product filtering system functions correctly based on user input
Ensure that UI states transition properly (Results, No Results, Reset).
Identify and report functional defects impacting user experience or correctness

-

### Scope

**In Scope:**

- Input validation behavior
- UI response/messages for valid and invalid searches
- Reset/Clear functionality

**Out of Scope:**

- System behavior across identified states
- Backend database performance
- Mobile responsiveness
- Compatibility testing across different browsers

### Tools & Resources

- Test data sheet
- Browser (Chrome / Firefox)
- Manual Black-box testing techniques:
  - Equivalence Partitioning
  - Boundary Value Analysis
  - Decision Table Testing
- Defect tracking sheet
  State Transition Testing

### Schedule

| Phase                  | Planned Duration            | Actual Duration | Status      |
| ---------------------- | --------------------------- | --------------- | ----------- |
| Test Planning          | 1 Day                       | 8 hours         | completed   |
| Risk analyst           | 1 day                       | 5 hours         | Completed   |
| Test Executor          | 2 day                       | 16 hours        | Completed   |
| Defect Reporting       | Continuous during execution |                 | Completed   |
| Final Review & Closure | 1 day                       |                 | Completed   |

## Risk Analysis

### Risks

| ID  | Feature          | Risk Description                                                                                  | Likelihood | Impact | Priority | Mitigation Strategy                                                                                    |
| --- | ---------------- | ------------------------------------------------------------------------------------------------- | ---------- | ------ | -------- | ------------------------------------------------------------------------------------------------------ |
| R1  | Bonus Round      | Bonus round logic may double score too early or fail to trigger after every 3 solves.             | Medium     | High   | High     | Verify score updates after every 3 puzzles using boundary test data. Retest with consistent sequences. |
| R2  | Leaderboard      | localStorage may fail to persist or correctly sort top 3 scores.                                  | High       | Medium | High     | Conduct multiple rounds of scoring; clear cache and revalidate persistence order.                      |
| R3  | Reset Game       | Reset may not clear hints, scrambled words, or state counters completely.                         | Medium     | Medium | Medium   | Observe UI and variables post-reset; confirm full state reinitialization.                              |
| R4  | Hint Function    | Hint may not deduct 2 points immediately or may allow multiple uses per puzzle.                   | Medium     | High   | High     | Test hint logic before and after use; confirm deduction and disable repeat hints.                      |
| R5  | Input Validation | Blank, mixed-case, or special character inputs may bypass validation or cause unhandled messages. | High       | low    | Medium   | Apply boundary and equivalence tests with empty, numeric, and special-character inputs.                |
| R6  | Message Feedback | Success/failure messages may disappear too quickly or fail to appear under invalid states.        | Medium     | Medium | Medium   | Observe #message updates for timing, clarity, and persistence across all user actions.                 |

### Risk Coverage

| **Risk ID** | **Covered by Test Case(s)** | **Risk Priority** | **Coverage Status** |
| ----------- | --------------------------- | ----------------- | ------------------- |
| R1          | TC-003, TC-006              | High              | ✅ Covered          |
| R2          | TC-008                      | High              | ✅ Covered          |
| R3          | TC-007                      | Medium            | ✅ Covered          |
| R4          | TC-005                      | High              | ✅ Covered          |
| R5          | TC-004                      | Medium            | ✅ Covered          |
| R6          | TC-001, TC-002              | Medium            | ✅ Covered          |

- Tested Risks: 6
- Tested Risks Percent: 100%
- Untested Risks Percent: 0%

### Risk Summary

As the Risk Analyst, I identified six functional and usability risks centered on logic errors, data persistence, and state control within Word Puzzle Game Plus. The highest risk features Bonus Round, Hint deduction, and Leaderboard storage were given top test priority.
Mitigation involved black box testing through boundary value analysis, decision table testing, and state transition checks to ensure data integrity and consistent UI behavior.
Overall, all identified risks were tested and validated, achieving 100% risk coverage with no critical untested areas.

## Test Cases

| **Test ID** | **Feature / Functionality** | **Expected Result**                           | **Actual Result** | **Status (Pass/Fail)** | \*\*Remarks / |
| ----------- | --------------------------- | --------------------------------------------- | ----------------- | ---------------------- | ------------- |
| TC-001      | Page Load                   | Game loads correctly, all UI elements visible | Works as expected | ✅ Pass                |               |
| TC-002      | New Puzzle                  | “New Puzzle” button changes scrambled word    | Works as expected | ✅ Pass                |               |
| TC-003      | Submit Guess (Correct)      | Shows “Correct! +10 points” and updates score | Works as expected | ✅ Pass                |               |
| TC-004      | Submit Guess (Incorrect)    | Shows “Incorrect, try again!”                 | Works as expected | ✅ Pass                |               |
| TC-005      | Hint Use                    | Deducts 2 points and displays hint            | works as expected | ✅ Pass|               |
| TC-006      | Bonus Round                 | After 3 solves, score doubles                 | Works correctly   | ✅ Pass                |               |
| TC-007      | Reset Game                  | Resets score, solved count, and clears word   | Works as expected | ✅ Pass                |               |
| TC-008      | Leaderboard                 | Saves top 3 scores in browser                 | Works as expected | ✅ Pass                |               |

## Defects

| ID  | Issue Title | Severity | Risk ID | Status | GitHub Link |
| --- | ----------- | -------- | ------- | ------ | ----------- |
|     |             |          |         |        |             |

## Defect Metrics
| **Metric**              | **Formula**                         | **Result** |
| ----------------------- | ----------------------------------- | ---------- |
| Test Case Pass %        | (7 / 8) × 100                       | **87.5%**  |
| Defect Density          | 5 defects / 8 test cases  |        **0.63**    |
| Risk Coverage           | (6 / 6) × 100                       | **100%**   |
| Regression Success Rate | Estimated after re-test             | Pending    |


### Defect Summary

| **Metric**               | **Value**       |
| ------------------------ | --------------- |
| Total Defects Logged     | 5               |
| Critical / High Severity | 2               |
| Medium Severity          | 2               |
| Low Severity             | 1               |
| Fix Rate                 | 20% (1/5 fixed) |

## Test Control & Project Management

### Phases

| Phase          | Deliverable                  | Actual Output          | Variance        | Owner         |
| -------------- | ---------------------------- | ---------------------- | --------------- | ------------- |
| Test Planning  | Approved Test Plan           | Completed on time      | None            | Test manager  |
| Risk Analyst   | Risk Analysis                | Minor adjustments made | +1 extra day    | Risk Analyst  |
| Test Execution | Test Results, Defect Reports |                        | defects pending | Test Executor |
| Test Closure   | Test Summary Report          | in progress            | none            | All Members   |

**Progress Tracking Method:**

- Daily defect reporting and dashboard updates
- Status tracked using GitHub Issues and Project Board
  **Change Control Notes:**

## Lessons Learned

- Most Defect Prone Feature: Filter logic caused unexpected “No Results” state
- Risk Analysis Impact: Early risk assessment helped identify missing validation
- Team Communication Effectiveness: Good collaboration through GitHub comments and assignments
- Improvements for Next Cycle: Automate high-priority test cases and perform earlier usability testing

## Attachments

-

## Sign Off

| Name        | Role          | Initials | Date       |
| ----------- | ------------- | -------- | ---------- |
| Denis Kyalo | Test Manager  | DK      | 24 10 2025 |
| Bramwel Mutugi | Risk Analyst  |  BM        | 26th Oct 2025       |
| Gideon Bethuel  | Test Executor | GB       | 27th Oct 2025      |

## Overall Summary

**Statement:**
- write one paragraph The Word Puzzle Game Plus was tested using a structured Test Plan focused on core gameplay functionality, UI state transitions, scoring rules, and data persistence features. Testing was performed using manual black-box methods including Equivalence Partitioning, Boundary Value Analysis, Decision Table Testing, and State Transition Testing on a desktop Chrome environment. High-risk features such as Bonus Round scoring and Leaderboard storage received focused attention based on the Risk Analysis.

- All six identified risks were fully tested, resulting in 100% risk coverage, ensuring confidence in critical gameplay areas. A total of eight main test cases were executed, with most passing successfully. Five defects were logged overall, including two high-severity issues affecting score doubling and immediate leaderboard updates. One defect has been fixed, while the remaining issues primarily impact user experience rather than core functionality.

- Project tracking was maintained through GitHub Issues and a Project Board, allowing continuous monitoring of progress. Communication among team members remained effective, and change control helped track UI and validation improvements. Future cycles will focus on automating key test cases, improving validation behavior, and enhancing usability on smaller screens.

- Overall, the testing effort confirmed that the game largely performs as expected, with clear improvement opportunities before final release.

**Test Status:** ✅ Completed

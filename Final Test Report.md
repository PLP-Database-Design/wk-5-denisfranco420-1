# 🧪 Final Group Test Report Template — Word Puzzle Game Plus

**Level:** Intermediate QA | **Week 5:** Test Management

**Course:** Software Testing & Quality Assurance  
**Module:** Test Management (Week 5)  
**Project Type:** Group Assessment  
**Submission Date:** 2025-10-28

## Team Information

| Role | Name | Responsibilities |
|------|------|------------------|
| Test Manager | | Planning, scheduling, coordination, metric tracking |
| Risk Analyst | Bramwel Mutugi | Risk identification, prioritization, test design linkage |
| Test Executor | Gideon Bethuel | Execution, evidence capture, defect logging |

## Group Rules

- Each student must belong to only one group.
- Duplicate membership or multiple submissions will result in invalidation.
- Every group member must contribute towards this project

## Project Overview

**System Under Test:** Word Puzzle Game Plus  
**Technology Stack:** HTML, CSS, JavaScript  
**Environment:** Chrome Browser (Desktop)

### Features Under Test

| Feature | Description | Risk Category |
|---------|-------------|---------------|
| Reset Game | Clears score and progress instantly | |
| Leaderboard | Stores top 3 scores in localStorage | |
| Bonus Round | Every 3 puzzles → doubles score | |

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

| Phase | Planned Duration | Actual Duration | Status |
|-------|------------------|-----------------|--------|
|Test Planning |1 Day | 8 hours| completed|
|Risk analyst | 1 day| | pending|
| Test Executor| 2 day | | pending|
| Defect Reporting| Continuous during execution| |Pending |
|Final Review & Closure | 1 day| | pending|

## Risk Analysis

### Risks

| ID | Feature | Risk Description | Likelihood | Impact | Priority | Mitigation Strategy |
|----|---------|------------------|------------|--------|----------|---------------------|
| | | | | | | |

### Risk Coverage

- Tested Risks Percent: 
- Untested Risks Percent: 

## Test Cases

| **Test ID** | **Feature / Functionality** | **Expected Result** | **Actual Result** | **Status (Pass/Fail)** | **Remarks /  |
|--------------|-----------------------------|----------------------|--------------------|-------------------------|---------------------------|
| TC-001 | Page Load | Game loads correctly, all UI elements visible | Works as expected | ✅ Pass |  |
| TC-002 | New Puzzle | “New Puzzle” button changes scrambled word | Works as expected | ✅ Pass |  |
| TC-003 | Submit Guess (Correct) | Shows “Correct! +10 points” and updates score | Works as expected | ✅ Pass |  |
| TC-004 | Submit Guess (Incorrect) | Shows “Incorrect, try again!” | Works as expected | ✅ Pass |  |
| TC-005 | Hint Use | Deducts 2 points and displays hint | works as expected | ☐ Pass / ☐ Fail |  |
| TC-006 | Bonus Round | After 3 solves, score doubles | Works correctly | ✅ Pass |  |
| TC-007 | Reset Game | Resets score, solved count, and clears word | Works as expected | ✅ Pass |  |
| TC-008 | Leaderboard | Saves top 3 scores in browser | Works as expected | ✅ Pass |  |



## Defects

| ID | Issue Title | Severity | Risk ID | Status | GitHub Link |
|----|-------------|----------|---------|--------|-------------|
| | | | | | |

## Metrics

- Test Case Pass Percent: 
- Defect Density: 
- Risk Coverage Percent: 
- Regression Success Rate: 

### Defect Summary

- Total Defects Logged: 
- Critical High: 
- Fix Rate: 

## Test Control & Project Management

### Phases

| Phase | Deliverable | Actual Output | Variance | Owner |
|-------|-------------|---------------|----------|-------|
| | | | | |

**Progress Tracking Method:**  
**Change Control Notes:**

## Lessons Learned

- Most Defect Prone Feature: 
- Risk Analysis Impact: 
- Team Communication Effectiveness: 
- Improvements for Next Cycle: 

## Attachments

- 

## Sign Off

| Name | Role | Initials | Date |
|------|------|-----------|------|
| Denis Kyalo | Test Manager | | 24 10 2025|
| Bramwel Mutugi | Risk Analyst | | 26 10 2025 |
| Gideon Bethwel| Test Executor | |26 10 2025 |

## Overall Summary

**Statement:** 

**Test Status:** ☐ Completed / ☐ In Progress / ☐ Deferred

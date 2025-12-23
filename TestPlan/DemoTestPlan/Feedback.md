# Introduction

- **Feature name: Feedback**
- **Feature target:** Allows users to send tickets about errors or features they want to improve to the admin, so that the admin can receive and easily manage tickets that need to be processed.
- **Link specs:** 
- **Version**: 2.0
- **Test Plan Version**: 1.0
- **Date**: Sep 23, 2025


# Objectives
To verify the functionality, usability, and reliability of the Feedback feature, ensuring users can submit, manage, and interact with tickets effectively, while admins can receive, process, and respond to them. This includes validating user and admin flows, UI elements, error handling, and basic security to confirm the feature meets its target of easy ticket management without critical issues.
# Scope

### In-Scope

- User: (site portal)
    - Send ticket
    - Close and reopen ticket
    - Search, filter ticket
    - Reply ticket
- Admin: (site admin-portal)
    - Receive ticket
    - Search, filter, sort tickets
    - Close and reopen ticket
    - Add note for ticket
    - Reply ticket
- UI validation, error handling and basic security checks

### Out-of-Scope
- Regression testing on unrelated features
- Performance testing

# Test Approach
- **Equivalence partitioning** for input validation
- **Boundary value analysis** for edge cases (e.g., ticket limits, field lengths)
- **State transition testing** for ticket lifecycle (e.g., open/close/reopen states)
- Testing will cover user flows, admin interactions, regression flows, and integrated fields/services as outlined in the test context mindmap. Basic automation may be considered for repetitive checks if time allows, but primary focus is manual execution with defect logging in a tracking tool.

# Test Criteria
- **Entry Criteria**: Feature deployed to qa/develop/prod, test environment stable, test cases approved.
- **Exit Criteria**: 100% coverage of in-scope items, all high/medium priority test cases passed, no critical/severe defects open, defect retest completed.
- **Suspension/Resumption**: Testing suspended if environment unstable or blockers found.

# Resource
- Personnel list (Team): Duc, Hieu, Anh, Thuy
- Roles & Responsibilities:
    - Build test plan: Duc
    - Build test design: Duc
    - Write testcase: Hieu
    - Execute test: Anh, Thuy
    - Report test result: Duc
    - Report progress: Duc

# Schedule

- **Phases:**
    - Planning
    - Execution
    - Reporting
- **Task & ETA**
    - Build Test Plan: 2 points
    - Build Test Design: 2 points
    - Write Test Cases: 2 points
    - Execute Test on Staging: 3 points
    - Execute Test on Prod: 2 points
    - Report
# Risks
- Changing requirement while the sprint
# Approval
- **Prepared by:** Ducbt
- **Review & Approved by:**
- **Date:**
# Test context

[https://atlas.mindmup.com/2025/12/a5a5ee20d19611f092fbc7e1d3793e0c/test_context/index.html](https://atlas.mindmup.com/2025/12/5a7c9a10d1b011f09a05bfbfd789dc77/test_context/index.html)




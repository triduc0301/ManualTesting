# Introduction
- Brief introduction to the feature, its main objective, version, and plan date.
- <i>Example:</i>
    - Feature name: Feedback
    - Feature target: Allows users to submit tickets for bugs or improvement suggestions so admins can easily receive and manage them.
    - Version: 2.0
    - Test Plan Version: 1.0
    - Date: 23/12/2025

# Objectives
- State the testing objectives concisely (functionality, usability, reliability, error handling, etc.).
- <i>Example:</i>  
  Verify that the Feedback feature works correctly, is user-friendly, handles errors properly, and enables admins to manage tickets effectively.

# Scope
### In-Scope
- Clearly list what will be tested.
- <i>Example:</i>
    - Testing the core functionalities of the feature, including:
    - User flow (user portal): submit ticket, close/reopen ticket, search/filter tickets, reply to ticket.
    - Admin flow (admin portal): receive tickets, search/filter/sort, close/reopen ticket, add notes, reply to ticket.
    - UI validation, error handling, and basic security checks.

### Out-of-Scope
- Functions or flows that do not need to be tested.
- <i>Example:</i>
    - Performance/load testing.
    - Detailed device/mobile compatibility testing.
    - Regression testing of unrelated features.

# Test Approach
- Describe the main testing methods and execution approach (manual or automation).
- <i>Example:</i>
    - Main methods: Equivalence partitioning, Boundary value analysis, State transition testing.
    - Primarily manual execution.

# Test Criteria
- Conditions for starting and completing testing.
- <i>Example:</i>
    - Entry: Test environment stable, test cases approved.
    - Exit: 100% coverage of in-scope items, no open critical/severe defects.

# Resource
- List team members and assigned responsibilities.
- <i>Example:</i>
    - Team: Duc, Hieu, Anh, Thuy
    - Roles:
        - Build plan & design: Duc
        - Write test cases: Hieu
        - Execute test: Anh, Thuy
        - Report: Duc

# Schedule
- Time estimation in story points or days for each phase.
- <i>Example:</i>
    - Build Test Plan: 2 points
    - Build Test Design: 2 points
    - Write Test Cases: 2 points
    - Execute Staging: 3 points
    - Execute Prod: 2 points

# Risks
- Briefly list potential risks.
- <i>Example:</i>
    - Requirement changes during the sprint.
    - Unstable test environment.

# Approval
- Person who prepared the plan and approver.
- <i>Example:</i>
    - Prepared by: Ducbt
    - Approved by:
    - Date:

# Test Context
- Link to test context, test design (e.g., mindmap or related documents).
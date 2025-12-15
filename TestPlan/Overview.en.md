# Overview of Test Strategy, Test Plan, Test Design

In software testing, these three concepts form the foundation for effectively planning and executing testing. They are built in sequence: Strategy (overall approach) → Plan (detailed plan) → Design (specific design). Below is a concise, easy-to-remember overview.

### Test Strategy vs Test Plan

| Criteria          | Test Strategy                          | Test Plan                              |
|-------------------|----------------------------------------|----------------------------------------|
| **Definition**    | High-level document describing the overall testing approach for the entire project. | Detailed document describing how testing will be executed for a specific release or phase. |
| **Purpose**       | Provide general direction, manage risks, align with development models (Agile/Waterfall). | Plan activities, assign tasks, track progress, and ensure product quality. |
| **Key Content**   | Objectives, scope, preliminary resources, risk strategy. | Introduction, specific resources, schedule, test types, deliverables. |
| **Characteristics**| High-level, rarely changes, general guidance. | Detailed, can vary by project, more practical. |
| **Pros/Cons**     | Pros: Flexible; Cons: Lacks execution details. | Pros: Specific guidance; Cons: Time-consuming to update. |

- **Test Strategy**: Use in the early project planning phase, when a overall framework is needed for the entire testing process (e.g., large, multi-phase projects). Ideal for long-term direction and high-level risk management.
- **Test Plan**: Use in the detailed planning phase, for specific sprints/releases (e.g., in Agile, during Sprint Planning). Suitable when immediate execution plans and progress tracking are required.

# Test Strategy (Testing Strategy)
- **Definition**: High-level document describing the overall testing approach, based on project requirements, risks, and business objectives. It guides the entire testing process without going into details.
- **Purpose**:
  - Define testing scope, types (manual/automation), tools, and pass/fail criteria.
  - Ensure alignment with development models (Agile, Waterfall) and risk management.

- **Key Content**:
  - Testing objectives.
  - Scope (in-scope/out-of-scope).
  - Resources (team, tools like Selenium, JIRA).
  - High-level schedule and entry/exit criteria.
  - Risk strategy (risk-based testing).

- **Characteristics**: High-level, rarely changes, usually drafted by Test Manager. Example: "Prioritize automation for regression testing in Agile".
- **Pros/Cons**: Pros: General guidance; Cons: Lacks execution details.
- **Usage**: Early project planning phase.

### Test Plan (Testing Plan)
- **Definition**: Detailed document based on the Test Strategy, describing how testing will be performed for a specific project or release.
- **Purpose**:
  - Plan activities, assign tasks, and track progress to ensure product quality.
  - Identify specific risks and mitigation measures.

- **Key Content** (per IEEE 829 standard):
  - Introduction (objectives, scope).
  - Resources (team, test environment).
  - Schedule and milestones.
  - Test types (unit, integration, system, acceptance).
  - Suspension/resumption criteria.
  - Deliverables list (test cases, reports).

- **Characteristics**: More detailed than Strategy, can vary by project. Example: "Achieve 80% coverage with 500 test cases in 2 weeks".
- **Pros/Cons**: Pros: Practical guidance; Cons: Time-consuming to update if project changes.
- **Usage**: Detailed planning phase, often in Sprint Planning (Agile).

# Test Design (Testing Design)
- **Definition**: The process of creating specific testing elements from requirements, including test scenarios, test cases, and test data.
- **Purpose**:
  - Ensure full coverage and early bug detection.
  - Convert requirements into executable tests.

- **Key Content**:
  - Analyze requirements → Create test scenarios (high-level).
  - Design test cases (detailed: steps, input, expected output).
  - Apply techniques: Equivalence Partitioning, Boundary Value Analysis.
  - Prepare test data and environment setup.

- **Characteristics**: Focuses on "how" to test, often automated where possible. Example: From "Login" requirement, design 10 test cases for positive/negative scenarios.
- **Pros/Cons**: Pros: Improves bug detection efficiency; Cons: Requires experience to avoid redundancy.
- **Usage**: Design and test execution phase, linked to Test Plan.
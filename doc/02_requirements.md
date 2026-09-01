# Requirements & Specification

This document reconstructs the requirements for the onboarding solution introduced in response to the pain points identified in [`01_problem_and_scenario.md`](./01_problem_and_scenario.md).

> [!NOTE]
> The requirements below were not formally documented in this format during the original project. They have been reconstructed retrospectively for this portfolio case study based on the implemented solution.

---

## 1. Functional Requirements

| ID | Requirement | 
|---|---|
| **FR-01** | The training application shall replicate all user-facing screens and functionality of the production application, including the login process. |
| **FR-02** | The training application shall provide guidance screens covering common application usage questions identified in the FAQ. |
---

## 2. Business Rule

### BR-01 — Production Application Usage

The training version may be used only for onboarding and practice.
Real customer surveys must be collected using the production application.

---

## 3. Example User Stories & Acceptance Criteria

### User Story — US-01: Pre-Shift Application Practice

> As a new hostess,  
> I want to practice using the application before my first field shift,  
> so that I can become familiar with the workflow before using it with customers.

```gherkin
Feature: Pre-Shift Application Training

  Scenario: Practicing the application before the first shift
    Given a new hostess has not yet started independent field work
    When she opens the training application
    Then she can practice the core application workflow
    And her actions do not create or modify production survey data
```
Traceability: BR-01 → FR-03 → US-01

### User Story — US-02: Self-Service Support

> As a new hostess,
> I want to find answers to common application questions,
> so that I can resolve basic issues without contacting helpdesk.

```gherkin
Feature: Self-Service Support

  Scenario: Finding an answer to a common question
    Given the hostess has access to the onboarding materials
    When she encounters a common application usage problem
    Then she can consult the FAQ
    And find the relevant guidance without contacting helpdesk
```
Traceability: FR-02 → US-02

### User Story — US-03: Standardized Onboarding

> As a Team Leader,
> I want new hostesses to receive standardized onboarding materials,
> so that their preparation does not depend only on my individual explanation.

```gherkin
Feature: Standardized Onboarding

  Scenario: Preparing a new hostess for application use
    Given a new hostess joins the team
    When the onboarding process begins
    Then she receives the user guide
    And she has access to the FAQ
    And she can use the training application before independent field work
```
Traceability: FR-01 → FR-02 → FR-03 → US-03

## 4. Requirements Traceability Summary

| Pain point                             | Requirement         | User Story / Rule   |
| -------------------------------------- | ------------------- | ------------------- |
| Frequent first-week support requests   | FR-01, FR-02, FR-03 | US-01, US-02, US-03 |
| Team Leader-dependent onboarding       | FR-01, FR-02        | US-03               |
| First hands-on use during real work    | FR-03               | US-01               |
| Training in the production environment | FR-03               | BR-01, BR-02, US-01 |

These requirements derive from the AS-IS workflow described in [`01_problem_and_scenario.md`](./01_problem_and_scenario.md) and are reflected in the AS-IS and TO-BE process models in [`03_process_diagrams.md.md`](./03_process_diagrams.md).

# 2. Requirements & Specification

This document reconstructs the requirements for the onboarding solution introduced in response to the pain points identified in [`01_problem_and_scenario.md`](./01_problem_and_scenario.md).

> [!NOTE]
> The requirements below were not formally documented in this format during the original project. They have been reconstructed retrospectively for this portfolio case study based on the implemented solution.

---

## 2.1. Functional Requirements

| ID | Category | Requirement | 
|---|---|---|
| **FR-01** | **Environment Fidelity** | The training application shall replicate all user-facing screens and functionality of the production application, including the login process. |
| **FR-02** | **In-App Guidance** | The training application shall provide guidance screens covering common application usage questions identified in the FAQ. |
| **FR-03** | **Training Data Separation** | The training application shall store training activity separately from production survey data. |
| **FR-04** | **Training Completion Tracking** | The training application shall record the completion status of the core training scenario in the training database.|

---

## 2.2. Business Rule

### BR-01 — Training and Production Application Usage

The training version may be used only for onboarding and practice.
Real customer surveys must be collected using the production application.

### BR-02* - NEW BUSSINES RULE? A new hostess must complete the core training scenario before her first independent field shift.

---

## 2.3. Example User Stories & Acceptance Criteria

### User Story — US-01: Pre-Shift Application Practice

> As a new hostess,  
> I want to practice using the application before my first field shift,  
> so that I can become familiar with the workflow before using it with customers.

```gherkin
Feature: Pre-Shift Application Training

Scenario: Practicing the application before the first shift
  Given a new hostess has not yet started independent field work
  When she opens the training application
  Then she can log in and access the same user-facing screens and functionality as in the production application
  And her actions do not create or modify production survey data
```
Traceability: FR-01, FR-03, BR-01

### User Story — US-02: In-App Guidance

> As a new hostess,  
> I want to access guidance within the training application,  
> so that I can learn how to handle common application usage situations while practicing.

```gherkin
Feature: In-App Guidance

  Scenario: Accessing guidance during training
    Given a new hostess is using the training application
    When she opens the guidance section
    Then she can view guidance covering common application usage questions identified in the FAQ
```

Traceability: FR-02

### User Story — US-03: Training Completion Record

> As application support,  
> I want the system to record whether a hostess has completed the training scenario,  
> so that completion status can be verified when needed.

```gherkin
Feature: Training Completion Tracking

Scenario: Recording training completion
  Given a hostess completes the core training scenario
  When the scenario is finished
  Then the system records the training as completed in the training database
```
Traceability: FR-04

## 2.4. Requirements Traceability Summary

> [Warning] Zmiana tabeli na | Pain point | Functional requirement | Business Rule | User Story |

| Pain point                             | Requirement         | User Story |
| -------------------------------------- | ------------------- | ------------------- |
| 📞 Frequent first-week support requests   | FR-01, FR-02        | US-01, US-02 |
| 👤 Team Leader-dependent onboarding       | FR-01, FR-02        | US-01, US-02            |
| 🏪 Learning happened during real work | FR-01               | US-01               |
| 🧪 Training in the production environment | FR-03               | US-01|
| ❓ No visibility of training completion   | FR-04               | US-03|

These requirements derive from the AS-IS workflow described in [`01_problem_and_scenario.md`](./01_problem_and_scenario.md) and are reflected in the AS-IS and TO-BE process models in [`03_process_diagrams.md`](./03_process_diagrams.md).

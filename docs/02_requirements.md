# 2. Requirements & Specification

This document reconstructs the requirements for the onboarding solution introduced in response to the pain points identified in [`01_problem_and_scenario.md`](./01_problem_and_scenario.md).

---

## 2.1. Functional Requirements

| ID | Category | Requirement | 
|---|---|---|
| **FR-01** | **Environment Fidelity** | The training application shall replicate all user-facing screens and functionality of the production application, including the login process. |
| **FR-02** | **In-App Guidance** | The training application shall provide guidance screens covering common application usage questions identified in the FAQ. |
| **FR-03** | **Training Data Separation** | The training application shall store training activity separately from production survey data. |
| **FR-04** | **Training Completion Tracking** | The training application shall record the completion status of the core training scenario in the training database.|

---

## 2.2. Business Rules

### BR-01 — Training and Production Application Usage

The production application may be used only during actual field work. Training activity must be performed in the training environment.

### BR-02 — Training Completion

New hostesses are expected to complete the core training scenario before their first independent field shift.

---

## 2.3. User Stories & Acceptance Criteria

### User Story — US-01: Application Practice
.
> **As a** new hostess, <br>
> **I want** to practice using the application in a training environment, <br>
> **so that** I can learn or revisit the workflow without affecting production data.

```gherkin
Feature: Application Training

Scenario: Practicing in the training environment
  Given a hostess has access to the training application
  When she uses the training application
  Then she can access the same user-facing screens and functionality as in the production application
  And her actions do not create or modify production survey data
```
Traceability: FR-01, FR-03, BR-01

### User Story — US-02: In-App Guidance

> **As a** new hostess,  
> **I want** to access guidance within the training application,  
> **so that** I can learn how to handle common application usage situations while practicing.

```gherkin
Feature: In-App Guidance

  Scenario: Accessing guidance during training
    Given a new hostess is using the training application
    When she opens the guidance section
    Then she can view guidance covering common application usage questions identified in the FAQ
```

Traceability: FR-02

### User Story — US-03: Training Completion Record

> **As** application support,  
> **I want** the system to record whether a hostess has completed the training scenario,  
> **so that** training completion data is available for future reporting and audit purposes.

```gherkin
Feature: Training Completion Tracking

Scenario: Recording training completion
  Given a hostess completes the core training scenario
  When the scenario is finished
  Then the system records the training as completed in the training database
```
Traceability: FR-04, BR-02

---

## 2.4. Requirements Traceability Summary

| Pain point                             | Requirement         |Business Rule | User Story |
| -------------------------------------- | ------------------- | --------------|----- |
| 📞 Frequent first-week support requests   | FR-01, FR-02     |BR-02    | US-01, US-02 |
| 👤 Team Leader-dependent onboarding       | FR-01, FR-02      |  | US-01, US-02            |
| 🏪 Learning happened during real work | FR-01             |BR-02  | US-01               |
| 🧪 Training in the production environment | FR-03         |BR-01      | US-01|
| ❓ No reliable visibility of individual training completion  | FR-04          |     | US-03|

These requirements derive from the AS-IS workflow described in [`01_problem_and_scenario.md`](./01_problem_and_scenario.md).

---
### 2.5. Illustrative NFRs

> The NFRs below are hypothetical examples created for this portfolio case study. They were not formally specified during the original project and are included to demonstrate how non-functional requirements could be defined for the onboarding solution.

| ID     | Category       | Illustrative NFR                                                                                                                 |
| ------ | -------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| NFR-01 | Compatibility      | The training application shall run on the same device models and Android versions as the production application, to ensure the practice experience matches real field conditions. |
| NFR-02 | Response times | Response times in the training application shall be representative of production application, to avoid setting unrealistic performance expectations. |

---

[← README](../README.md) · [← 01 Problem & Scenario](./01_problem_and_scenario.md) · **02 Requirements & Specification**


# Field App Onboarding & Support Optimization

### Business Analysis Mini Case Study

`Status: In Progress` `Type: Real-World Case Study` `Domain: Retail / Field Operations` `Methods: User Stories / Gherkin`

A focused BA case study of a real process improvement introduced for a tablet application used by approximately 150 field hostesses and 12 Team Leaders across Poland.

The case study focuses on one recurring operational problem: onboarding new hostesses to the application. It traces the process from an informal, support-heavy onboarding model to a structured approach based on user documentation, FAQ and a safe training version of the application.

> **Confidentiality:** Company, client, application and brand names have been anonymised. No confidential screens, customer data or commercially sensitive information are reproduced.

---

## 1. Where This Fits in the Wider Process

This case study focuses only on application onboarding before a new hostess begins independent field work. Recruitment, campaign planning, ongoing workforce management and the broader customer-survey process are outside the scope of the analysis.

`Hostess recruitment / assignment` → **Application onboarding (this case study)** → `Work scheduling` → `First field shift` → `Customer survey collection` → `Performance monitoring & ongoing support`

---

## 2. Actors

| Actor                                     | Involved in this workflow?             | Role                                                                                               |
| ----------------------------------------- | -------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **New Hostess**                           | ✅                                      | Learns how to use the application and prepares to use it independently during field work           |
| **Team Leader**                           | ✅                                      | Introduces new hostesses to the application and supervises their work                              |
| **Application Support / Project Manager** | ✅                                      | Provides user support, identifies recurring onboarding issues and coordinates process improvements |
| **Customer / Survey Participant**         | ❌ (downstream / outside this workflow) | Completes a survey during a hostess's field shift after purchasing selected products               |

---

## 3. Illustrative Scenario

A new hostess needs to learn how to use the tablet application before her first independent field shift.

Before the improvement, onboarding depended mainly on the Team Leader, and the hostess often used the application independently for the first time during real work.

`New hostess joins` → `Team Leader explains the application` → `First use during real work` → `User encounters difficulties` → `Helpdesk contact`

In some cases, training was performed in the production application, creating test records that later had to be manually removed.

A detailed AS-IS scenario and identified pain points are described in [`01_problem_and_scenario.md`](docs/01_problem_and_scenario.md).

---

## 4. Problem & Goal

There was no standardized onboarding process for new hostesses. As a result, new users often learned the application during their first shift, generated frequent support requests and, in some cases, practiced in the production environment.

The goal was to create a more structured onboarding process that would reduce helpdesk dependency and allow new hostesses to learn and practice before starting independent field work.

The solution included a separate training version of the application.

---

## 5. Success Measures & Illustrative NFRs

### Success Measures

* **First-week support reduction:** After introducing the new onboarding approach, the number of support calls from a newly onboarded hostess during her first week decreased from approximately 10 to no more than 3 — a reduction of at least approximately 70%.
* **Pre-shift practice adoption:** 100% of new hostesses completed the core training scenario in the training environment before their first field shift (previously 0%).
* **Test data elimination:** Production survey records requiring manual removal due to training activity dropped from a recurring issue to 0 after the training environment was introduced.

### Illustrative NFRs

> The NFRs below are hypothetical examples created for this portfolio case study. They were not formally specified during the original project and are included to demonstrate how non-functional requirements could be defined for the onboarding solution.

| ID     | Category       | Illustrative NFR                                                                                                                 |
| ------ | -------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| NFR-01 | Usability      | At least 90% of new hostesses should be able to complete the core training scenario without assistance after reviewing the onboarding materials. |
| NFR-02 | Response times | Response times in the training application shall not be faster than in the production application, to avoid setting unrealistic performance expectations.  |

---

## 6. Scope

**In scope:** onboarding process design (training environment) for new hostesses, up to their first independent field shift.

**Out of scope:** production application redesign and any process steps outside this workflow, including recruitment, scheduling and campaign planning.
FAQ content is treated as an existing input; this case study covers its integration into in-app guidance screens, not FAQ authoring.

---

## 7. Requirements

The onboarding improvement is documented through functional requirements, business rules, user stories and acceptance criteria.

Full specification and traceability: ➡️ [`02_requirements.md`](docs/02_requirements.md)

---

## 8. Case Study Contents

| Document                                                        | Purpose                                                                                     |
| ----------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| [`01_problem_and_scenario.md`](docs/01_problem_and_scenario.md) | AS-IS problem, scenario, recurring support issues and pain points                           |
| [`02_requirements.md`](docs/02_requirements.md)                 | Functional requirements, business rules, user stories, acceptance criteria and traceability |
| [`03_process_diagrams.md`](docs/03_process_diagrams.md)         | AS-IS and TO-BE                                                        |

---

## 💡 Skills Demonstrated

`AS-IS / TO-BE process analysis` 
`Requirements analysis, business rules & traceability`
`User Stories & Acceptance Criteria (Gherkin)`
`Stakeholder & user needs analysis`
`Solution evaluation using operational results`

---

## 📬 Contact

Kamila Woronicz
Business Analyst | Product Manager (career transition)

* Email: [kamila.woronicz@gmail.com](mailto:kamila.woronicz@gmail.com)
* Location: Gdańsk, Poland

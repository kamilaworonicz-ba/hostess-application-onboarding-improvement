# Field App Onboarding & Support Optimization

### Business Analysis Mini Case Study

`Status: In Progress` `Type: Real-World Case Study` `Domain: Retail / Field Operations` `Methods: BPMN 2.0 / User Stories / Gherkin`

A focused BA case study of a real process improvement introduced for a tablet application used by approximately 150 field hostesses and 12 Team Leaders across Poland.

The case study focuses on one recurring operational problem: onboarding new hostesses to the application. It traces the process from an informal, support-heavy onboarding model to a structured approach based on user documentation, FAQ and a safe training version of the application.

---

## 🗺️ Where This Fits in the Wider Process

This case study focuses only on application onboarding before a new hostess begins independent field work. Recruitment, campaign planning, ongoing workforce management and the broader customer-survey process are outside the scope of the analysis.

`Hostess recruitment / assignment` → **Application onboarding (this case study)** → `Work scheduling` → `First field shift` → `Customer survey collection` → `Performance monitoring & ongoing support`

---

## 👥 Actors

| Actor                                     | Involved in this workflow?             | Role                                                                                               |
| ----------------------------------------- | -------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **New Hostess**                           | ✅                                      | Learns how to use the application and prepares to use it independently during field work           |
| **Team Leader**                           | ✅                                      | Introduces new hostesses to the application and supervises their work                              |
| **Application Support / Project Manager** | ✅                                      | Provides user support, identifies recurring onboarding issues and coordinates process improvements |
| **Customer / Survey Participant**         | ❌ (downstream / outside this workflow) | Completes a survey during a hostess's field shift after purchasing selected products               |

---

## ℹ️ Context & Disclaimer

* **Domain background:** This case study is based on my real professional experience managing the maintenance and development of a tablet application used by approximately 150 hostesses and 12 Team Leaders across Poland. I also acted as the first-line application support within a small project team.

* **Real-world implementation:** Unlike a purely conceptual portfolio case, both the problem and the main improvement described here are based on an actual implemented solution. User instructions with FAQ were introduced together with a training version of the application that allowed new hostesses to practice before their first real shift.

* **Confidentiality:** The company, client, application and brand names have been anonymised. The case study focuses only on the onboarding and support process and does not reproduce confidential application screens, customer data or commercially sensitive information.

---

## 🧩 Illustrative Scenario

A new hostess joins a field team and needs to learn how to use the tablet application before working independently in a retail location.

Before the process improvement, application onboarding depended largely on the individual Team Leader. In many cases, the hostess used the application independently for the first time during her first actual shift.

`New hostess joins` → `Team Leader explains the application` → `First use during real work` → `User encounters difficulties` → `Helpdesk contact` → `Issue explained / resolved`

In some cases, Team Leaders allowed new hostesses to practice using their own production application before the first shift. This generates non-production survey records that later had to be manually removed by support.

A detailed AS-IS scenario and identified pain points are described in [`01_problem_and_scenario.md`](docs/01_problem_and_scenario.md).

---

## 🎯 Problem & Goal

There was no standardized application onboarding process for new hostesses.

This created several recurring problems:

* new users often encountered the application for the first time while already working with customers,
* onboarding quality depended on the individual Team Leader,
* new hostesses repeatedly contacted helpdesk with basic usage questions,
* a single new hostess could generate approximately 10 support calls during her first week,
* practicing in the production application could create test records that later required manual removal.

Because hostess turnover was relatively high, the same onboarding and support effort had to be repeated frequently.

The goal was to create a more structured and scalable onboarding process that would allow new users to understand and practice the basic application workflow before their first shift, while reducing dependence on Team Leaders and helpdesk support.

The implemented solution combined:

* a structured user guide,
* FAQ based on recurring support questions,
* a separate training version of the application for safe hands-on practice.

---

## 📊 Success Measures & Illustrative NFRs

### Success Measures

* **First-week support reduction:** After introducing the new onboarding approach, the number of support calls from a newly onboarded hostess during her first week decreased from approximately 10 to no more than 3 — a reduction of at least approximately 70%.
* **Pre-shift practice:** New hostesses gained the ability to practice the main application workflow before their first real field shift.
* **Training data separation:** Application training no longer required using a Team Leader's production environment and creating test survey records that later had to be manually removed.

### Illustrative NFRs

> The NFRs below are hypothetical examples created for this portfolio case study. They were not formally specified during the original project and are included to demonstrate how non-functional requirements could be defined for the onboarding solution.

| ID     | Category       | Illustrative NFR                                                                                                                 |
| ------ | -------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| NFR-01 | Usability      | At least 90% of new hostesses should be able to complete the core training scenario without assistance after reviewing the onboarding materials. |
| NFR-2 | Security / Data Isolation | The training environment must not expose production customer data or allow training users to access production records.  |

---

## 📐 Scope

**In scope:** onboarding process design (user guide, FAQ, training environment) for new hostesses, up to their first independent field shift.

**Out of scope:** production application redesign and any process steps outside this workflow, including recruitment, scheduling and campaign planning.

---

## 📋 Requirements

The onboarding improvement is documented through functional requirements, business rules, user stories and acceptance criteria.

Full specification and traceability: ➡️ [`02_requirements.md`](docs/02_requirements.md)

---

## 📚 Case Study Contents

| Document                                                        | Purpose                                                                                     |
| ----------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| [`01_problem_and_scenario.md`](docs/01_problem_and_scenario.md) | AS-IS problem, scenario, recurring support issues and pain points                           |
| [`02_requirements.md`](docs/02_requirements.md)                 | Functional requirements, business rules, user stories, acceptance criteria and traceability |
| [`03_process_diagrams.md`](docs/03_process_diagrams.md)         | AS-IS and TO-BE BPMN process models                                                         |

---

## 💡 Skills Demonstrated

`AS-IS / TO-BE process analysis & BPMN modelling` 
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

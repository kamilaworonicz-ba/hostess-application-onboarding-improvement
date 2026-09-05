# Field App Onboarding & Support Optimization

### Business Analysis Mini Case Study

`Status: In Progress` `Type: Real-World Case Study` `Domain: Retail / Field Operations`<br> `Methods: Requirements Analysis / User Stories / Gherkin / Traceability`

A focused BA case study of a real process improvement introduced for a tablet application used by approximately **150 field hostesses and 12 Team Leaders across Poland**.

New hostesses had no standardized application onboarding process and often used the application independently for the first time during real field work. This resulted in frequent support requests and, in some cases, training activity being performed in the production environment.

The improvement introduced a structured onboarding approach combining user guidance with a separate training version of the application, allowing new hostesses to practice the core workflow before their first independent shift.

A detailed AS-IS scenario and identified pain points are described in [`01_problem_and_scenario.md`](docs/01_problem_and_scenario.md).


## 📈 Results
- **First-week support:** approximately 10 → no more than 3 calls per newly onboarded hostess
- **Pre-shift practice:** 100% completion of the core training scenario before the first field shift
- **Training data in production:** recurring issue → 0 records requiring manual removal

## 🎯 Scope

**In scope:**
- Onboarding process design (training environment) for new hostesses, up to their first independent field shift
- Recording training completion data in the database for future reporting and audit purposes

**Out of scope:**
- FAQ authoring (already exists as an input)
- In-app Team Leader visibility of training completion status
- Automatic blocking of production access for hostesses who have not completed the training

---

## 📂 Case Study Contents

| Document                                                        | Purpose                                                                                     |
| ----------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| [`01_problem_and_scenario.md`](docs/01_problem_and_scenario.md) | AS-IS problem, scenario, recurring support issues and pain points                           |
| [`02_requirements.md`](docs/02_requirements.md)                 | Functional requirements, business rules, user stories, acceptance criteria and traceability |

> **Confidentiality:** Company, client, application and brand names have been anonymised. No onfidential screens, customer data or commercially sensitive information are reproduced.

---

## 📬 Contact

Kamila Woronicz
Business Analyst | Product Manager (career transition)

* Email: [kamila.woronicz@gmail.com](mailto:kamila.woronicz@gmail.com)
* Location: Gdańsk, Poland

---
**README** · [01 Problem & Scenario →](./01_problem_and_scenario.md) · [02 Requirements & Specification →](./02_requirements.md)

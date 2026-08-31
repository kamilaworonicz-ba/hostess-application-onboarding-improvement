# Problem & Scenario: Hostess Application Onboarding

## 1. AS-IS Problem

New hostesses needed to learn how to use the tablet application before working independently in retail locations. However, there was no standardized application onboarding process.

> [!WARNING]
> In the process this case study is based on, onboarding depended mainly on the **Team Leader**. A new hostess was shown how the application worked, but often used it independently for the first time during her first actual field shift.

This created several recurring problems:

- 📞 **Frequent first-week support requests.** A newly onboarded hostess could contact application support approximately **10 times during her first week**, often with basic usage questions.
- 👤 **Onboarding depended on the individual Team Leader.** The amount and quality of training varied depending on the Team Leader's availability and approach.
- 🏪 **Learning happened during real work.** New hostesses often encountered unfamiliar application functions while already working with customers.
- 🧪 **Training sometimes took place in the production application.** Team Leaders occasionally allowed new hostesses to practice using their own application, which could create test survey records that later had to be manually removed by support.

The scenario below illustrates a typical onboarding path before the process improvement.

---

## 2. Illustrative Scenario: New Hostess Onboarding

> [!NOTE]
> The sequence below illustrates a typical onboarding path. The exact number and type of support requests varied between users.

```mermaid
flowchart LR
    A["New hostess joins the team"] --> B["Team Leader explains the application"]
    B --> C["First independent use during field work"]
    C --> D{"User encounters a problem?"}
    D -- Yes --> E["Contact application support"]
    E --> F["Issue explained or resolved"]
    F --> C
    D -- No --> G["Continues field work"]

    style E fill:#c0392b,stroke:#333,stroke-width:2px,color:#fff
    style G fill:#2e7d32,stroke:#333,stroke-width:2px,color:#fff

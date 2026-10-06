```mermaid
flowchart TD
    A[Legacy Healthcare Portal] --> B[Patient Care Context]
    A --> C[Billing & Insurance Context]
    A --> D[Diagnostics Context]

    B --> E[Patient]
    B --> F[Appointment]
    B --> G[Provider]
    B --> H[Medical Record]

    C --> I[Invoice]
    C --> J[Payment]
    C --> K[Insurance Claim]
    C --> L[Insurance Provider]

    D --> M[Lab Order]
    D --> N[Lab Test]
    D --> O[Specimen]
    D --> P[Lab Result]
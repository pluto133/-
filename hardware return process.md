``` mermaid
flowchart TD
    A[Initiation] -->|Employee Notification| B[Return Request Form]
    B --> C[Authorization]
    C -->|Manager Approval| D[IT Department Notification]
    D --> E[Scheduling]
    E -->|Schedule Return Date and Time| F[Send Return Instructions]
    F --> G[Hardware Collection]
    G -->|Physical Return| H[Initial Inspection]
    H --> I{Data Backup Required?}
    I -->|Yes| J[Perform Data Backup]
    I -->|No| K[Data Wiping]
    J --> K[Data Wiping]
    K -->|Prepare for Wiping| L[Execute Data Wiping]
    L --> M[Verify Data Wiping]
    M --> N[Final Inspection and Documentation]
    N -->|Functional Testing| O[Update Asset Management]
    O -->|Generate Destruction Certificate| P[Refurbishment/Disposal]
    P -->|Refurbishment| Q[Prepare for Re-Deployment]
    P -->|Disposal| R[Prepare for Disposal]
    Q --> S[Confirmation and Reporting]
    R --> S[Confirmation and Reporting]
    S -->|Notify Employee and Manager| T[Generate Summary Report]

    subgraph Initiation
        A --> B
    end

    subgraph Authorization
        C --> D
    end

    subgraph Scheduling
        E --> F
    end

    subgraph Hardware Collection
        G --> H
    end

    subgraph Data Wiping
        K --> L
        L --> M
    end

    subgraph Final Inspection and Documentation
        N --> O
        O --> P
    end

    subgraph Refurbishment/Disposal
        P --> Q
        P --> R
    end

    subgraph Confirmation and Reporting
        S --> T
    end
```

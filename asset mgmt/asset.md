flowchart TD
    A[Start] --> B[Asset Identification]
    B --> C[Asset Acquisition]
    C --> D[Asset Registration]
    D --> E[Asset Inventory and Tagging]
    E --> F[Asset Assignment and Deployment]
    F --> G[Asset Monitoring and Maintenance]
    G --> H[Asset Reassessment and Updates]
    H --> I{Is Asset Still in Use?}
    I -->|Yes| G
    I -->|No| J[Asset Decommissioning]
    J --> K[Asset Disposal or Recycling]
    K --> L[Update Asset Records]
    L --> M[End]

    %% Styling for clarity
    style A fill:#f9f,stroke:#333,stroke-width:2px
    style M fill:#f96,stroke:#333,stroke-width:2px
    style I fill:#ff9,stroke:#333,stroke-width:2px

``` mermaid
sequenceDiagram
    participant C as End-user
    participant SA as UHD engineer
    participant ITC as IT Custodian
    participant W as Storage Area
    participant F as Vendor

    C->>SA: Request to return hardware
    SA->>C: Provide return authorization
    SA->>SA: Perform hardware factory reset
    SA->>ITC: Provide Hardware List
    ITC->>ITC: Request IT hardware disposal
    SA->>W: Ship hardware to Storage Area
    #W->>SA: Receive hardware and check condition
    W->>F: Verify hardware quantity
    F->>W: Confirm hardware recevied
    # SA->>C: Confirm return and process refund
    # C->>SA: Acknowledge refund receipt

```

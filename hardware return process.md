``` mermaid
sequenceDiagram
    participant C as End-user
    participant SA as UHD engineer
    participant W as Warehouse
    participant F as Vendor

    C->>SA: Request to return hardware
    SA->>C: Provide return authorization
    SA->>SA: Perform hardware factory reset
    SA->>W: Ship hardware to warehouse
    W->>SA: Receive hardware and check condition
    W->>F: Verify hardware reset status
    F->>W: Confirm hardware is reset
    # SA->>C: Confirm return and process refund
    # C->>SA: Acknowledge refund receipt

```

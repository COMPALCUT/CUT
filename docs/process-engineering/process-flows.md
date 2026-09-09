# Process Flows

**Owner:** Process Engineering  
**Review frequency:** At NPI launch and after major process changes

## Standard Flow Rules

- Normal production flow should read left-to-right.
- Pass paths continue forward.
- Fail paths move downward to inspection, rework or reject.
- Rework loops return to the correct validated point in the process.
- MES transactions should be shown where product status or routing changes.

## Example Server Assembly Flow

```mermaid
flowchart LR
    A[Receive Material] --> B[Kit / Stage]
    B --> C[Mechanical Assembly]
    C --> D[Component Installation]
    D --> E[Torque Verification]
    E --> F[Functional Test]
    F --> G{Pass?}
    G -- Yes --> H[Final Inspection]
    H --> I{Pass?}
    I -- Yes --> J[Pack / Ship]
    G -- No --> R[Repair / Troubleshoot]
    I -- No --> R
    R --> V[Verification]
    V --> F
```

## Required Information

A controlled process flow should identify:

- Process/station number
- Station name
- Input and output
- Inspection or decision points
- Pass/fail routing
- Rework/repair loops
- MES/system transactions
- Special process controls
- Responsible function where needed

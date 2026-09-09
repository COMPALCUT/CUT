# Conveyors & Material Handling

Document conveyor sections, transfer stations, lifts, sensors, interlocks and routing logic here.

## Key Controls

- Product presence sensors
- Stop positions
- Transfer confirmation
- Lift up/down permissives
- Jam detection
- Emergency stop behavior
- PLC/MES handshake
- Manual recovery method

## Flow Example

```mermaid
flowchart LR
    A[Infeed] --> B[Presence Detect]
    B --> C[Transfer Station]
    C --> D{Destination Ready?}
    D -- Yes --> E[Release Product]
    D -- No --> F[Hold / Wait]
    F --> D
```

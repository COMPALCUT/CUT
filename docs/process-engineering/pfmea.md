# PFMEA

A Process Failure Mode and Effects Analysis identifies how a manufacturing process can fail, the impact of the failure, potential causes, current controls, and actions to reduce risk.

## Minimum PFMEA Fields

| Field | Description |
|---|---|
| Process Step | Operation or station being analyzed |
| Process Function | What the step is intended to accomplish |
| Failure Mode | How the process could fail |
| Failure Effect | Impact on product, customer, safety or next process |
| Severity | Impact rating |
| Potential Cause | Why the failure could occur |
| Occurrence | Likelihood rating |
| Prevention Control | Control intended to prevent the cause |
| Detection Control | Control intended to detect the failure |
| Detection | Detection rating |
| Action | Risk-reduction activity |
| Owner / Due Date | Accountability |

## Example

| Step | Function | Failure Mode | Effect | Cause | Prevention | Detection | Action |
|---|---|---|---|---|---|---|---|
| GPU Install | Install GPU correctly | GPU not fully seated | No POST / functional failure | Uneven insertion force | Defined insertion method and fixture | Functional test / visual check | Add force-controlled insertion aid or measurable acceptance criteria |
| Torque | Secure fastener | Under-torque | Loose assembly | Incorrect tool setting | Programmed torque tool | Torque result logged by serial number | Lock recipe by product configuration |

!!! warning "PFMEA discipline"
    The PFMEA should represent the real manufacturing process—not an idealized process. Update it when failures, escapes, or significant process changes reveal new risk.

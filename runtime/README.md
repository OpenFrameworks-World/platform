# OpenFrameworks Runtime

OpenFrameworks Runtime is the executable implementation of the OpenFrameworks Foundation contract.

It consumes the Foundation specifications and makes framework authoring, validation, publishing, graph updates, decisions, temporal history, and trust execution operational.

## Source of Truth

The runtime must consume, not redefine, the Foundation contract.

Foundation repository:

```text
https://github.com/OpenFrameworks-World/foundation
```

Canonical foundation entry point:

```text
FOUNDATION.md
```

## Runtime Goal v0.1

Make this operation executable end-to-end:

```text
publish framework-card identity-governance
```

The runtime must:

1. compile the language statement
2. validate the artifact against the Meta Contract
3. evaluate Meta Policy
4. create or link a Decision Record
5. transition lifecycle state
6. create Event and Action records
7. create Temporal Records
8. update the Graph
9. publish the artifact
10. return an auditable Execution Result

## Runtime Modules

```text
runtime/
├── registry/        # artifact storage
├── graph/           # nodes, edges, traversal, impact analysis
├── validator/       # meta contract and artifact validation
├── policy/          # meta policy evaluation
├── state-machine/   # lifecycle transitions
├── decision/        # decision records
├── temporal/        # time, validity, history
├── compiler/        # language statement to operation plan
├── execution/       # operation plan execution
├── publishing/      # publishing gate and published artifacts
├── trust/           # evidence, risk, confidence, trust computation
├── search/          # discovery and query
├── api/             # runtime API surface
└── cli/             # runtime command interface
```

## Minimum Runtime Flow

```text
Language Statement
  -> Compiler
  -> Operation Plan
  -> Meta Validator
  -> Meta Policy
  -> Decision Record
  -> State Transition
  -> Event Record
  -> Action Record
  -> Temporal Record
  -> Graph Update
  -> Published Artifact
```

## Implementation Principle

Start deterministic and local.

Do not begin with distributed architecture.

Runtime v0.1 should run locally, validate local artifacts, and write deterministic graph records before becoming a service mesh or hosted platform.

## Non-Negotiable Invariants

- No artifact without identity.
- No framework without capability.
- No published artifact without policy approval.
- No material transition without decision.
- No state change without time.
- No graph edge without relationship type.
- No trust claim without evidence.
- No runtime behavior that contradicts Foundation.

## Status

Runtime scaffold initialized.

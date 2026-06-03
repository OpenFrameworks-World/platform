# Runtime Registry Module

The Registry Module is the local system of record for OpenFrameworks runtime artifacts.

It stores artifacts that satisfy the OpenFrameworks Foundation Meta Contract and exposes deterministic read/write operations for runtime execution.

## Source of Truth

The Registry consumes Foundation definitions. It does not redefine artifact meaning.

Foundation contract:

```text
OpenFrameworks-World/foundation
  FOUNDATION.md
  schemas/meta.contract.schema.json
  specs/meta.contract.md
  specs/graph.schema.md
```

## Responsibilities

The Registry stores:

- framework cards
- framework blueprints
- operating models
- architecture models
- systems
- value models
- evidence records
- trust records
- decision records
- temporal records
- published artifacts
- operations
- validation results
- policy results

## Minimal Data Model

```ts
Artifact {
  id: string
  type: string
  version: string
  lifecycleState: string
  publishingState: string
  payload: object
  createdAt: string
  updatedAt: string
}
```

## Required Operations

```text
createArtifact(artifact)
getArtifact(id)
updateArtifact(id, patch)
listArtifacts(filter)
getArtifactHistory(id)
```

## Invariants

- No artifact without identity.
- No artifact without type.
- No artifact without version.
- No published artifact may be silently overwritten.
- Every mutation must be auditable.

## Runtime v0.1 Goal

Support storing and retrieving a Framework Card that can later be validated, published, and inserted into the graph.

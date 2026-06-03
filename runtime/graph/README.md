# Runtime Graph Module

The Graph Module is the runtime representation of the OpenFrameworks graph.

The Registry stores artifacts.

The Graph connects artifacts through typed relationships, states, events, actions, decisions, and time.

## Source of Truth

The Graph Module consumes the Foundation graph contract.

Foundation references:

```text
OpenFrameworks-World/foundation
  specs/runtime.kernel.md
  specs/canonical.vocabulary.md
  specs/graph.schema.md
  specs/temporal.record.md
```

## Responsibilities

The Graph Module stores and queries:

- nodes
- edges
- relationship types
- lifecycle states
- publishing states
- event records
- action records
- decision links
- temporal relationships
- evidence links
- trust links

## Runtime Kernel Mapping

```text
Entity       -> Node
Relationship -> Edge
State        -> Node State
Event        -> Event Record
Action       -> Action Record
Decision     -> Decision Link
Time         -> Temporal Metadata
```

## Minimal Data Model

```ts
GraphNode {
  id: string
  type: string
  artifactId?: string
  version?: string
  lifecycleState?: string
  publishingState?: string
  createdAt: string
  updatedAt: string
}

GraphEdge {
  id: string
  source: string
  target: string
  relationshipType: string
  direction: "directed"
  rationale?: string
  confidence?: number
  evidenceRefs?: string[]
  createdAt: string
}
```

## Required Operations

```text
createNode(node)
getNode(id)
updateNode(id, patch)
createEdge(edge)
getEdge(id)
listEdges(filter)
traverse(startNode, options)
impact(nodeId)
pointInTime(nodeId, timestamp)
```

## Required Queries

The graph must answer:

```text
Why does this framework exist?
What capability does this framework provide?
What frameworks compose this blueprint?
What breaks if this framework changes?
What evidence supports this trust score?
Why was this artifact published?
What was true at this point in time?
What value was realized?
What did adoption teach us?
```

## Invariants

- No node without type.
- No edge without canonical relationship type.
- No material edge without direction.
- No published graph mutation without validation and policy approval.
- No silent mutation of published graph records.
- Every material mutation must be time-bound.

## Runtime v0.1 Goal

Support creating a graph node for a Framework Card and a typed edge from the Framework Card to its published artifact.

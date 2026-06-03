# OpenFrameworks Platform

OpenFrameworks Platform is the open-core product implementation that operationalizes the OpenFrameworks Foundation.

The platform discovers, stores, validates, searches, compares, governs, benchmarks, publishes, recommends, certifies, and accredits frameworks, standards, protocols, methodologies, operating models, governance models, maturity models, benchmarks, reference architectures, and implementation patterns.

## Relationship to Foundation

Canonical meaning lives in the foundation repository.

```text
OpenFrameworks Foundation
  -> defines ontology, schemas, vocabulary, governance rules, trust model, scoring dimensions, certification, accreditation, and traceability model

OpenFrameworks Platform
  -> implements registry, graph, validation, search, workflows, APIs, publishing, benchmarking, recommendations, dashboards, and enterprise operating surfaces
```

Foundation repo:

```text
https://github.com/OpenFrameworks-World/foundation
```

This repository must consume foundation definitions, not redefine them.

## North Star

Make every useful framework discoverable, comparable, governable, certifiable, accreditable, composable, and operationally useful.

## Product Positioning

OpenFrameworks Platform is a vendor-neutral framework intelligence and governance platform.

It helps organizations answer:

- Which framework should we use?
- Why should we trust it?
- What evidence supports it?
- What alternatives exist?
- What are the risks?
- Which capabilities and outcomes does it support?
- Who approved it?
- Is it certified or accredited?
- Is it still creating value?

## Open-Core Boundary

### Open Platform Capabilities

The open platform should include:

- public framework registry
- framework card rendering
- foundation schema validation
- public graph model
- public search
- public benchmark definitions
- public scoring views
- public publishing templates
- community reports
- GitHub-native contribution workflows

### Commercial / Enterprise Capabilities

Commercial or private extensions may include:

- private enterprise catalogs
- organization-specific accreditation workflows
- SSO and SCIM
- RBAC, ABAC, and approval workflows
- private evidence management
- portfolio rationalization
- compliance mapping
- executive dashboards
- audit exports
- advanced recommendation assistant
- enterprise integrations
- managed deployments and support

## Platform Runtime Modules

```text
registry/       # framework and asset catalog implementation
graph/          # relationship graph and traversal engine
validation/     # validation against foundation schemas and policies
search/         # search and discovery
benchmarks/     # benchmark execution and reporting runtime
scoring/        # runtime score calculation using foundation dimensions
trust/          # trust, confidence, and risk calculation runtime
workflows/      # review, approval, certification, accreditation workflows
publishing/     # static and dynamic publishing surfaces
api/            # public and internal APIs
apps/web/       # public web experience
apps/admin/     # admin and governance console
integrations/   # connectors and import/export pipelines
extensions/     # extension boundaries for enterprise/private capabilities
```

## What Belongs in Foundation, Not Here

The following canonical definitions belong in OpenFrameworks Foundation:

- ontology
- JSON-LD context
- JSON Schemas
- glossary
- taxonomy
- vendor-neutrality policy
- trust model
- scoring dimensions
- certification levels
- accreditation vocabulary
- capability model
- outcome model
- stakeholder model
- decision model
- action model
- lifecycle model
- traceability model

The platform may keep generated copies, pinned versions, or imported packages for runtime use, but foundation remains the source of truth.

## First Implementation Milestones

1. Import foundation schemas and context.
2. Add framework card validation.
3. Add public registry folder and sample cards.
4. Build graph ingestion from cards.
5. Add search and filtering.
6. Add scoring runtime.
7. Add trust and risk runtime.
8. Add publishing output.
9. Add governance workflow skeleton.
10. Add API and web UI.

## Status

Early platform draft.

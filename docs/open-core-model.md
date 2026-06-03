# OpenFrameworks Open Core Model

OpenFrameworks follows an open core model.

The public platform provides the open foundation, open schemas, open registry model, open governance rules, open validation logic, open framework cards, open benchmark definitions, and community publishing surface.

Enterprise capabilities are built as private or commercial extensions on top of the open core.

## Open Core Principles

- The canonical language is open.
- The ontology is open.
- The schemas are open.
- The governance model is open.
- The vendor-neutrality policy is open.
- The trust model is open.
- The scoring dimensions are open.
- The public registry model is open.
- The validation rules are open.
- Enterprise workflow automation may be commercial.
- Private catalogs may be commercial.
- Advanced analytics may be commercial.
- Enterprise integrations may be commercial.

## Open Source Core

The open core includes:

- foundation documentation
- glossary and taxonomy
- JSON Schema
- JSON-LD context
- SurrealDB schema
- public framework card model
- public capability model
- public outcome model
- public stakeholder model
- vendor-neutrality policy
- trust model
- certification model
- community registry structure
- validation scripts
- public benchmark definitions
- public scoring dimensions
- GitHub Pages publishing templates

## Commercial / Enterprise Extensions

Enterprise extensions may include:

- private framework catalogs
- organization-specific accreditation workflows
- SSO and SCIM integration
- role-based approval workflows
- advanced policy engine
- private benchmark execution
- internal evidence management
- portfolio rationalization
- executive dashboards
- audit exports
- compliance mapping
- enterprise search
- AI recommendation assistant
- private deployment support
- SLA-backed managed service
- premium integrations

## Boundary Rule

The open core must be useful on its own.

The enterprise edition may improve scale, governance, privacy, automation, reporting, integrations, and operational readiness, but must not make the open foundation artificially incomplete.

## Repository Strategy

Recommended repository layout:

```text
OpenFrameworks-World/platform
  public open core platform
  foundation
  schemas
  docs
  validation
  public registry
  community publishing

OpenFrameworks-World/enterprise-platform
  private or commercial enterprise extensions
  tenant management
  private catalogs
  enterprise workflows
  SSO/SCIM
  dashboards
  integrations
  managed service modules
```

If only one repository is used initially, enterprise-only code must stay behind clearly marked extension boundaries and must not pollute the open core.

## Product Tiers

### Community

Free and open.

Includes:

- public framework registry
- framework cards
- validation
- public scoring dimensions
- public benchmark definitions
- public reports
- GitHub Pages publishing

### Team

Commercial lightweight tier.

Includes:

- small private catalogs
- team workflows
- private reports
- collaboration
- limited integrations

### Enterprise

Commercial enterprise tier.

Includes:

- private enterprise catalog
- accreditation workflows
- SSO/SCIM
- RBAC/ABAC
- audit exports
- compliance mapping
- portfolio rationalization
- executive dashboards
- managed deployment

## Licensing Guidance

The open core should use a permissive or source-available license only after legal and business review.

Enterprise modules should use a commercial license.

The license boundary must be documented before accepting external contributions.

## Non-Negotiable Rule

Vendor neutrality, schemas, ontology, public governance language, and public validation rules must remain open.

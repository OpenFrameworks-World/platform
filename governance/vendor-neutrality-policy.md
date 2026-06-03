# Vendor Neutrality Policy

OpenFrameworks World is vendor-neutral, framework-aware, evidence-driven, and governance-first.

## Policy Statement

The platform must describe, compare, benchmark, and recommend frameworks using transparent criteria, evidence, constraints, and governance decisions.

No recommendation may be based only on vendor popularity, sponsorship, sales relationship, ecosystem pressure, analyst preference, or commercial incentive.

## Mandatory Separation

Every framework card must separate:

1. Framework capability
2. Vendor implementation
3. Open standard
4. Commercial distribution
5. Hosted service
6. Ecosystem dependency
7. Licensing and lock-in risk

## Required Fields

Every framework card must include a `vendor_neutrality` section with:

- `neutrality_required`
- `vendor_specific`
- `vendor_name`
- `open_standard_available`
- `open_source_available`
- `portable_implementations`
- `lock_in_risks`
- `commercial_relationships`
- `neutrality_review_status`

## Recommendation Rules

A framework cannot be marked `recommended` unless:

- neutrality review is approved
- lock-in risks are documented
- alternatives are listed when applicable
- evidence sources are declared
- commercial relationships are disclosed
- vendor-specific claims are separated from framework-level claims

## Anti-Bias Rules

The following are prohibited as sole justification for recommendation:

- vendor popularity
- market share
- sponsorship
- paid partnership
- analyst ranking
- sales relationship
- default cloud marketplace availability
- internal preference without evidence

## Required Review Outcomes

- `approved`
- `needs-evidence`
- `vendor-specific`
- `rejected`

## Examples

Kubernetes is a framework/platform standard.

EKS, AKS, GKE, OpenShift, and Rancher are implementations, distributions, or management platforms.

The platform must not collapse these into one concept.

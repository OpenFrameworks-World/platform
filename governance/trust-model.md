# OpenFrameworks Trust Model

OpenFrameworks trust is evidence-driven, governance-first, vendor-neutral, and reproducible.

## Trust Equation

```text
Trust = Evidence Quality + Governance Quality + Operational Validation + Review Quality - Risk Exposure
```

Trust is not popularity. Trust is not market share. Trust is not sponsorship.

## Core Scores

### Overall Score

A normalized 0-100 assessment of framework fitness against the scoring model.

### Confidence Score

A normalized 0-100 assessment of how reliable the evaluation is.

Confidence depends on:

- evidence quality
- evidence recency
- source diversity
- reviewer credibility
- benchmark reproducibility
- governance completeness

### Risk Score

A normalized 0-100 assessment of exposure.

Risk includes:

- security risk
- compliance risk
- lock-in risk
- operational risk
- maturity risk
- maintenance risk
- ecosystem risk
- migration risk

## Evidence Quality Levels

| Level | Meaning |
|---|---|
| none | No evidence supplied |
| low | Weak, old, partial, or self-reported evidence |
| medium | Some credible evidence but incomplete coverage |
| high | Multiple credible sources or reproducible evaluations |
| verified | Independently reviewed, reproducible, and current evidence |

## Recommendation Gates

### Adopt

Requires:

- overall score >= 80
- confidence score >= 75
- risk score <= 40
- neutrality review approved
- governance review approved
- alternatives documented
- lock-in risks documented

### Trial

Requires:

- overall score >= 60
- confidence score >= 50
- risk score <= 65
- neutrality review not rejected

### Monitor

Used when the framework is promising but evidence, maturity, governance, or adoption is incomplete.

### Avoid

Used when risk is high, governance is weak, evidence is poor, or neutrality concerns are unresolved.

### Insufficient Evidence

Used when claims cannot be supported.

## Non-Negotiable Rules

- No recommendation without evidence.
- No recommendation without alternatives.
- No recommendation without lock-in analysis.
- No recommendation without vendor-neutrality review.
- No score without reproducible inputs.
- No framework can be recommended based only on popularity, sponsorship, analyst ranking, or vendor preference.

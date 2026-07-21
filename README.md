# Methodology Engineering

> **Status:** Minimum Methodology-Engineering Contract v0.1

## Methodology Engineering Overview

This visual overview introduces the purpose, lifecycle, engineering principles, ecosystem position, and long-term vision of the Methodology Engineering repository.

### Methodology Engineering

![Research Methodology](assets/slides/slide-01-research-methodology.png?raw=1)

### Methodology Lifecycle

![Methodology Lifecycle](assets/slides/slide-02-methodology-lifecycle.png?raw=1)

### Why Methodology Engineering Matters

![Why Methodology Engineering Matters](assets/slides/slide-03-why-methodology-matters.png?raw=1)

### Where Methodology Engineering Fits

![Continufy Research Pipeline](assets/slides/slide-04-research-pipeline.png?raw=1)

### Long-Term Vision

![Long-Term Vision](assets/slides/slide-05-long-term-vision.png?raw=1)

## Purpose

This repository develops the principles, object models, transformation contracts, and scientific instruments for engineering reproducible methodologies.

Its central determination is:

> **A methodology is a normative object transformation system.**

A methodology defines which objects exist, how they may be transformed, what evidence and rules each transformation requires, how outputs are verified, and how provenance, uncertainty, and failure are preserved.

Research methodology is the first reference specialization developed within this repository.

This repository does not conduct research or execute methodologies itself.

## What is Methodology Engineering?

Methodology Engineering is the discipline of designing, validating, and evolving methodologies that systematically transform complex reality into reproducible evidence, validated understanding, and better decisions.

It provides the object models, transformation contracts, scientific instruments, lifecycle rules, and verification principles required to build reusable methodologies without collapsing methodology definition into methodology execution.

## Governing Question

> **How should methodologies be engineered to systematically transform complex reality into reproducible evidence, validated understanding, and better decisions?**

## Canonical Methodology-Engineering Contract

This repository now defines the **Minimum Methodology-Engineering Contract v0.1** as its first canonical documentation for methodology engineering. The canonical contract is maintained in [Methodology Engineering Canon](METHODOLOGY_ENGINEERING_CANON.md).

The contract explains how reusable research methodologies and scientific instruments are defined, versioned, reviewed, executed, calibrated, improved, and superseded without executing any particular study. It also establishes the required distinction ledger, minimum methodology object, methodology lifecycle, instrument lifecycle, repository boundary, known limitations, and explicit non-goals.

This repository also defines the **Cross-Domain Structology Transfer Audit v0.1** as a named methodology definition maintained in [Cross-Domain Structology Transfer Audit v0.1](CROSS_DOMAIN_STRUCTOLOGY_TRANSFER_AUDIT_V0_1.md). The audit definition specializes the generic contract for transfer assessment methodology only; it does not execute the audit or produce empirical findings.

Residual methodology-conformance outcomes, negative-capability and interaction boundaries, and non-mutating cross-registry reconciliation are defined in the [Residual Conformance, Negative Capability, and Reconciliation Contract v1.0](RESIDUAL_CONFORMANCE_NEGATIVE_CAPABILITY_AND_RECONCILIATION_CONTRACT_V1_0.md). That contract does not authorize execution, repair, synchronization, or scientific claims.

Residual generic evidence objects, lifecycle transitions, admissibility and sufficiency, projections, validated emission, and evidence-specific cross-repository conformance are defined in the [Residual Generic Evidence Lifecycle and Conformance Contract v1.0](RESIDUAL_GENERIC_EVIDENCE_LIFECYCLE_AND_CONFORMANCE_CONTRACT_V1_0.md). This repository owns only that reusable definition; concrete evidence and executions remain in their investigation or evidence repositories.

## General Model

```text
Complex Reality
        ↓
Objects
        ↓
Methodology
Defines valid transformations
        ↓
Execution
Applies transformations
        ↓
Evidence
        ↓
Understanding
        ↓
Decision
```

Research methodology is the first specialization of this general methodology-engineering model.

## Research Methodology Specialization

```text
Research Need
        ↓
Research Request
        ↓
Investigation Protocol
        ↓
Observations
        ↓
Evidence
        ↓
Analysis
        ↓
Decision
        ↓
Finding
        ↓
Publication
```

This sequence is not merely a workflow. Each step represents a typed object transformation governed by declared rules.

## Object, Methodology, and Execution

```text
Object
≠
Execution
```

An object represents a bounded state or artifact.

Execution is an activity or event that creates, consumes, or transforms concrete object instances.

Methodology Engineering defines the transformation contract:

```text
Object
        ↓
Methodology
Defines valid transformations
        ↓
Execution
Applies a transformation
        ↓
New Object
```

Therefore:

```text
Methodology
≠
Execution
```

```text
Transformation Contract
≠
Transformation Event
```

## Research Transformation Contract

Every valid research transformation should define:

```text
Research Transformation {
  source object type
  admissible source state
  required inputs
  governing rule
  operation
  target object type
  resulting state
  preserved invariants
  permitted changes
  verification
  provenance
  uncertainty
  failure modes
  responsible roles
}
```

A transformation is valid only when its required inputs exist, its governing rule applies, its provenance resolves, its uncertainty is preserved, and its output satisfies the declared contract.

## First-Class Methodology Objects

Every first-class methodology object should have a consistent shape:

```text
Methodology Object {
  identity
  type
  purpose
  inputs
  outputs
  lifecycle
  relationships
  version
  provenance
  uncertainty
  verification
  failure state
}
```

Research-specific object types include:

- Research Request
- Investigation Protocol
- Observation Record
- Evidence Item
- Instrument
- Calibration Record
- Collection Run
- Transformation or Analysis Record
- Decision Record
- Finding
- Replication Attempt
- Verification Result
- Publication Record

These are type definitions. A specific investigation produces concrete instances.

## Current Scope

- Methodology object systems
- Methodology lifecycle engineering
- Transformation contracts
- Methodology specialization
- Scientific instrument design
- Research-object definitions
- Investigation lifecycle and stage gates
- Evidence planning and admissibility
- Observation, derivation, measurement, and analysis boundaries
- Decision rules and adjudication
- Scientific instrument interfaces
- Calibration and improvement
- Replication and reproduction
- Verification and conformance
- Provenance, traceability, and lineage
- Missingness, uncertainty, and limitations
- Publication and transfer boundaries
- Failure, deviation, withdrawal, and supersession semantics

## Non-Scope

This repository does not contain:

- empirical study executions;
- methodology executions;
- investigation-specific evidence;
- Cross-Domain Structology Transfer Audit executions or any other domain-specific instrument execution;
- domain-specific methodologies except as bounded reference specializations;
- domain-specific research protocols;
- evidence models for specific studies;
- schemas, validators, runtime behavior, or methodology compilers;
- formal domain theory;
- deterministic analysis engines;
- operational execution systems;
- domain-specific research conclusions;
- authority to accept scientific claims;
- runtime object mutation;
- modifications to Structology.

Those artifacts remain in their respective repositories and executions.

## Methodology Engineering and Structology

Structology defines domain-neutral structural primitives.

Methodology Engineering specializes those primitives into methodology and instrument contracts. Research methodology is the first reference specialization.

```text
Structology
Objects, stages, relations, transformations,
verification, provenance, and failure
        ↓
Methodology Engineering
Methodology and instrument contracts
        ↓
Research Methodology
Research-specific transformation contracts
        ↓
Architectural Boundary Research
Investigation-specific executions, evidence, assessments, and findings
```

Methodology Engineering must not redefine domain-neutral structure as though it were unique to methodology or research.

## Relationship to Research Execution

Methodology Engineering defines types and valid transformations.

Research execution creates instances and performs transformations under the research methodology specialization.

For example:

```text
Research Methodology
Defines Observation Record
        ↓
Investigation
Creates BOR-001
```

```text
Research Methodology
Defines Evidence-to-Analysis transformation
        ↓
Investigation
Executes one analysis over frozen evidence
```

A completed object or transformation instance is evidence of execution. A methodology definition alone is not.

## Relationship to the Continufy Ecosystem

```text
Structology
Defines domain-neutral structure
        ↓
Methodology Engineering
Defines methodology transformation contracts
        ↓
MindShift
Produces candidate abstractions and research requests
        ↓
Architectural Boundary Research
Executes empirical investigations
        ↓
Structural Analysis Foundations
Produces formal theory
        ↓
SYNAPSE
Produces deterministic structural evidence
```

ContinuityOS remains outside the scientific-method execution path. It governs execution legitimacy where mutation-capable actions require authorization.

Each repository owns a distinct transformation and produces a distinct class of artifact.

## Boundary Principles

```text
Methodology
≠
Execution
```

```text
Object Type
≠
Object Instance
```

```text
Analyst Activity
≠
Object Transformation
```

```text
Transformation
≠
Verification
```

```text
Verification
≠
Scientific Warrant
```

```text
Evidence
≠
Decision
```

```text
Publication
≠
Canonical Evidence
```

This repository defines how reproducible methodologies may be structured. It does not conduct, formalize, implement, operationalize, or authorize domain executions itself.

## Current Status

This repository defines the architectural boundary for Methodology Engineering while the discipline continues to emerge through reference specializations and active investigations.

Research methodology is the first reference specialization. Additional methodology domains should be introduced only when reusable methodology-engineering patterns are supported by repeated execution evidence.

Content should be promoted here only when it is reusable across multiple methodology or research domains and no longer belongs exclusively to `architecturalboundary-research` or another domain-specific repository.

## Historical Methodology Completeness Audit

`METHODOLOGY_COMPLETENESS_AUDIT.md` records an assessment performed on
2026-07-17 against repository baseline `f1a3b3e`.

The audit identifies the information, rules, transformations, and artifacts that
were missing or underspecified at that historical baseline. Its findings are
preserved as audit evidence and are not the current repository completeness
determination.

See [Methodology Completeness Audit](METHODOLOGY_COMPLETENESS_AUDIT.md).

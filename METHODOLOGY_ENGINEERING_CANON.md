# Methodology Engineering Canon

**Canonical status:** Minimum Methodology-Engineering Contract v0.1  
**Scope:** reusable methodology and instrument contracts for research  
**Boundary:** definition only; no methodology execution and no domain-specific audit instrument

## 1. Purpose

This canon defines the minimum methodology-engineering contract required to create reusable research methodologies and scientific instruments. It does not define a specific research methodology, execute research, or evaluate scientific correctness.

The contract stops at **Minimum Methodology-Engineering Contract v0.1**. A future issue may define a Cross-Domain Structology Transfer Audit Instrument, but that instrument is not defined here.

## 2. Relationship to Structology

Research Methodology assumes Structology Candidate Model v0.1 already exists. Structology supplies candidate structural concepts; Research Methodology specializes those concepts for research contracts.

```text
Structology
Candidate structural concepts
        ↓
Research Methodology
Defines research methodology contracts
        ↓
Research Execution
Executes one methodology
```

Research Methodology references Structology. It does not redefine Structology, modify Structology, or claim ownership over domain-neutral structural concepts.

## 3. Repository Boundary

```text
Research Methodology
Defines methodologies
        ↓
Architectural Boundary Research
Executes methodologies
        ↓
Structology
Defines candidate structural concepts
```

Research Methodology owns methodology definitions, instrument definitions, lifecycle contracts, review expectations, versioning semantics, calibration semantics, and supersession semantics. It does not own investigations, study evidence, empirical conclusions, or execution systems.

Architectural Boundary Research may execute a methodology by creating methodology instances, instrument executions, evidence, deviations, limitations, and findings. Those execution artifacts are not stored or governed as empirical truth by this repository.

Structology owns candidate structural concepts. Research Methodology may specialize those concepts into research-methodology meanings, but must not redefine the underlying structural model.

## 4. Required Definitions

### Methodology

A **Methodology** is a reusable, versioned research contract that defines how research objects may be transformed into reviewable research artifacts under declared rules, uncertainty, verification, failure, calibration, and supersession semantics.

### Methodology Definition

A **Methodology Definition** is the canonical specification of a methodology: its identity, purpose, research question form, scope, object types, transformation contracts, evidence requirements, verification rules, uncertainty rules, failure semantics, version, calibration history, and supersession status.

### Methodology Instance

A **Methodology Instance** is the investigation-supplied use of a particular methodology version in a bounded execution context. It binds the methodology definition to concrete investigation inputs, but it does not mutate the methodology definition.

### Methodology Version

A **Methodology Version** is an immutable, identifiable state of a methodology definition. It records what contract was in force at a point in time and is the target against which executions are interpreted.

### Methodology Lifecycle

A **Methodology Lifecycle** is the minimum sequence by which a methodology need becomes a reviewed, reference-executed, calibrated, versioned, and eventually superseded methodology definition.

### Methodology Contract

A **Methodology Contract** is the set of minimum obligations a methodology definition imposes on compliant executions, including required objects, transformations, evidence, verification, uncertainty handling, failure semantics, version identity, calibration status, and supersession rules.

### Methodology Calibration

**Methodology Calibration** is the reviewable comparison of a methodology version against reference execution results, limitations, deviations, and observed failure modes to determine whether the methodology contract needs refinement. Calibration may produce a new methodology version; it does not silently mutate an existing version.

### Methodology Improvement

A **Methodology Improvement** is a proposed or accepted change to a methodology definition that clarifies, strengthens, constrains, or corrects the methodology contract. Accepted improvements create a new methodology version.

### Methodology Supersession

**Methodology Supersession** is the explicit replacement of one methodology version by a later version for future use. Supersession does not invalidate or rewrite executions that were performed under the earlier version.

### Research Instrument

A **Research Instrument** is a reusable mechanism, protocol, tool, questionnaire, model, rubric, device, or procedure used to produce or transform observations, measurements, classifications, or evidence under a methodology contract.

### Instrument Definition

An **Instrument Definition** is the canonical specification of a research instrument: identity, purpose, applicable methodology context, inputs, outputs, operating rules, calibration requirements, limitations, version, and improvement path.

### Instrument Execution

An **Instrument Execution** is a concrete use of a specific instrument version in a bounded research execution. It produces observations, transformations, logs, deviations, or evidence records, but does not mutate the instrument definition.

### Instrument Calibration

**Instrument Calibration** is the comparison of an instrument version or configuration against declared references, tolerances, benchmark cases, or review criteria to establish fitness for a stated execution context.

### Instrument Version

An **Instrument Version** is an immutable, identifiable state of an instrument definition or configuration. It determines which instrument contract governed a pilot execution, reference instrument, or research execution.

### Investigation Methodology

An **Investigation Methodology** is the methodology version selected and bound for one investigation. It is an instance-level commitment to follow a reusable methodology contract in a specific research context.

### Reference Execution

A **Reference Execution** is a controlled execution of a methodology version used to expose ambiguities, failures, calibration needs, and review questions. It is evidence about the methodology contract's operational clarity, not evidence for a domain-specific research claim.

### Pilot Execution

A **Pilot Execution** is an initial controlled use of an instrument definition to test operating clarity, calibration needs, limitations, and execution risks before designating a reference instrument.

### Verification

**Verification** is the rule-governed determination that a methodology definition, methodology instance, instrument definition, execution artifact, or transformation satisfies its declared contract.

### Deviation

A **Deviation** is a recorded difference between the declared methodology or instrument contract and what occurred in an execution. It must identify the expected rule, actual event, cause, authorization status, and impact.

### Limitation

A **Limitation** is a declared boundary on applicability, interpretation, measurement, inference, execution reliability, or evidentiary strength.

### Assumption

An **Assumption** is a declared condition accepted for a methodology definition, instrument definition, or execution context without being fully established by the methodology itself. It must have scope, rationale, and review status.

## 5. Canonical Distinction Ledger

| Distinction | Canonical meaning |
| --- | --- |
| Methodology Definition ≠ Methodology Execution | A definition specifies reusable rules; an execution performs those rules in a concrete context. |
| Methodology ≠ Research Study | A methodology is a reusable contract; a research study is one bounded investigation that may use a methodology. |
| Research Instrument ≠ Research Execution | An instrument is a reusable means of producing or transforming research objects; execution is one concrete use of that means. |
| Reference Execution ≠ Evidence | A reference execution calibrates or tests the methodology contract; it is not evidence for a domain-specific research claim. |
| Calibration ≠ Methodology Mutation | Calibration evaluates a version and may justify a new version; it never silently changes the calibrated version. |
| Methodology Version ≠ Historical Rewrite | A new version changes future interpretation and use; it does not rewrite earlier methodology versions, executions, or evidence. |

These distinctions are canonical for this repository.

## 6. Minimum Methodology Contract

A methodology definition must expose the following minimum object. Each field is classified by its role in the contract.

| Field | Classification | Minimum contract meaning |
| --- | --- | --- |
| Identity | foundational | Stable name or identifier for the methodology. |
| Purpose | foundational | The research-methodological need the methodology addresses. |
| Research Question | investigation supplied | The question form or binding rule that an execution must supply. |
| Scope | foundational | Inclusions, exclusions, applicability boundaries, and repository boundary assumptions. |
| Object Types | foundational | Research object classes governed by the methodology. |
| Transformation Contracts | foundational | Permitted object transformations and their required inputs, outputs, invariants, and failure states. |
| Evidence Requirements | foundational | Minimum requirements for admissible evidence within executions. |
| Verification Rules | foundational | Rules for determining conformance to the methodology contract. |
| Uncertainty Rules | foundational | Rules for recording, preserving, and propagating uncertainty, assumptions, limitations, and unresolved conditions. |
| Failure Semantics | foundational | Required handling of invalid inputs, unmet evidence requirements, failed verification, deviations, and unusable outputs. |
| Version | foundational | Immutable methodology version identity and change boundary. |
| Calibration History | derived | Record derived from reference executions, review findings, deviations, limitations, and improvement decisions. |
| Supersession | optional | Replacement relationship to later methodology versions; absent when no superseding version exists. |

No field in the minimum contract is currently classified as unresolved. Additional methodology-specific fields may be optional or investigation supplied, but they must not weaken the foundational fields.

## 7. Minimum Methodology Lifecycle

```text
Need
↓
Methodology Definition
↓
Review
↓
Reference Execution
↓
Calibration
↓
Version
↓
Supersession
```

### Need

Owns the research-methodological gap, reusable purpose, intended class of investigations, and reason a methodology definition is needed.

### Methodology Definition

Owns the written methodology contract, required definitions, object types, transformations, evidence requirements, verification rules, uncertainty rules, failure semantics, and version identity.

### Review

Owns inspection of clarity, consistency, boundary adherence, minimum contract completeness, non-goal compliance, and readiness for reference execution.

### Reference Execution

Owns controlled execution against the methodology definition to reveal ambiguity, missing requirements, impractical steps, deviations, limitations, and calibration needs. It does not own domain-specific evidence claims.

### Calibration

Owns interpretation of review and reference-execution results against the methodology contract. Calibration determines whether the current methodology version remains usable, requires limitations, or should produce an improved version.

### Version

Owns immutable publication of a methodology definition state. A version freezes the contract for future execution references.

### Supersession

Owns replacement of an earlier methodology version for future use. Supersession records the successor version and reason for replacement without rewriting earlier versions or executions.

## 8. Minimum Instrument Lifecycle

```text
Instrument Definition
↓
Pilot Execution
↓
Calibration
↓
Reference Instrument
↓
Research Executions
↓
Evidence
↓
Instrument Improvements
```

### Instrument Definition

Owns the reusable instrument contract, including identity, purpose, operating rules, required inputs, expected outputs, calibration requirements, limitations, and version identity.

### Pilot Execution

Owns bounded trial use of the instrument to identify ambiguity, operating risks, missing instructions, required references, and calibration needs.

### Calibration

Owns comparison against references, tolerances, benchmark cases, expected outputs, or review criteria. Calibration establishes whether the instrument is fit for a stated use and version.

### Reference Instrument

Owns the designated instrument version and configuration considered sufficiently specified and calibrated for repeated research executions.

### Research Executions

Own concrete uses of the reference instrument in investigations. They record instrument version, execution context, outputs, deviations, and limitations.

### Evidence

Owns investigation-specific observation or transformation records produced by instrument executions. Evidence belongs to the execution context, not to the instrument definition.

### Instrument Improvements

Own proposed and accepted changes to the instrument definition. Accepted improvements create new instrument versions and do not rewrite earlier instrument executions.

This lifecycle does not define any specific instrument.

## 9. Historical Preservation

The preservation chain is:

```text
Methodology Version
↓
Execution
↓
Evidence
```

An execution is interpreted against the methodology version and instrument version in force at the time of execution. Later methodology or instrument versions must not rewrite, relabel, or silently reinterpret earlier executions or evidence.

Calibration produces a new methodology version when it changes the contract. Calibration records may explain why a version was improved or superseded, but they do not mutate the prior version.

## 10. Known Limitations

- This canon defines a minimum methodology-engineering contract, not a complete research methodology.
- It does not define the Cross-Domain Structology Transfer Audit.
- It does not execute any methodology or instrument.
- It does not define domain-specific research protocols, schemas, validators, runtime behavior, compilers, or evidence models for specific studies.
- It does not claim methodological correctness.
- It relies on Structology Candidate Model v0.1 as an external conceptual reference and does not restate that model.
- It leaves future issues to define concrete methodology definitions, concrete instrument definitions, and conformance artifacts.

## 11. Explicit Non-Goals

This repository change does not:

- define the Cross-Domain Structology Audit;
- execute any methodology;
- define domain-specific research protocols;
- define evidence models for specific studies;
- build schemas;
- build validators;
- build runtime behavior;
- build methodology compilers;
- claim methodological correctness;
- modify Structology.

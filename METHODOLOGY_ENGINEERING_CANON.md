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
Reusable research methodology and instrument contracts
        ↓
Architectural Boundary Research
Concrete methodology executions, evidence, assessments, and findings
```

Research Methodology references Structology. It does not redefine Structology, modify Structology, or claim ownership over domain-neutral structural concepts.

## 3. Repository Boundary

```text
Structology
        ↓
Research Methodology
        ↓
Architectural Boundary Research
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


## 6A. Complete Methodology Object

A complete methodology object must be sufficient for an execution repository to identify the governing contract, bind inputs, perform bounded transformations, record provenance, and determine whether execution may continue. The minimum object is:

```text
Methodology Object {
  identity
  version
  governing question
  admissible inputs
  procedure
  decision rules
  provenance requirements
  deviation semantics
  failure and stopping rules
  outputs
  limitations
  supersession lineage
}
```

| Field | Required meaning |
| --- | --- |
| Identity | Stable methodology name or identifier. |
| Version | Immutable version of the methodology contract. |
| Governing question | The reusable question form the methodology is designed to answer or structure. |
| Admissible inputs | Input classes, required attributes, exclusion criteria, admissibility thresholds, and minimum completeness conditions. |
| Procedure | Ordered transformation steps, stage gates, required records, and completion criteria. |
| Decision rules | Deterministic rules, precedence rules, or required adjudication records for material choices. |
| Provenance requirements | Minimum source, custody, actor, timestamp, version, configuration, and derivation records required for replay and review. |
| Deviation semantics | Required classification, authorization, impact assessment, and disposition for departures from the contract. |
| Failure and stopping rules | Conditions that require rejection, suspension, amendment, continuation with limitation, or termination. |
| Outputs | Required artifacts, completion criteria, verification requirements, and publication or handoff boundaries. |
| Limitations | Applicability, inference, measurement, operational, evidentiary, and interpretation boundaries. |
| Supersession lineage | Prior version, successor version, reason for replacement, effective boundary, and preservation rule for earlier executions. |

A methodology definition is incomplete if any field is absent, if execution cannot identify the exact version in force, or if stopping and failure conditions are left to unrecorded judgment.

## 6B. Execution Binding Contract

Execution is not part of the methodology definition, but a compliant execution must bind itself to the exact methodology contract it applies:

```text
Execution
        ↓
Exact methodology identity
Exact version
Declared inputs
Declared scope
Provenance
Deviations
Artifacts
Verification result
Stopping determination
```

| Binding element | Required meaning |
| --- | --- |
| Exact methodology identity | The stable methodology identifier used by the execution. |
| Exact version | The immutable methodology version in force for the execution. |
| Declared inputs | Concrete inputs accepted for the execution, including admissibility determinations and exclusions. |
| Declared scope | The execution boundary, exclusions, assumptions, and interpretation limits. |
| Provenance | Source, custody, actor, timestamp, version, configuration, and derivation records sufficient for review. |
| Deviations | Recorded departures from the methodology or instrument contract, including authorization and impact. |
| Artifacts | Durable records produced or consumed by the execution. |
| Verification result | The conformance determination against the bound methodology version. |
| Stopping determination | The recorded decision to continue, stop, suspend, fail, or complete under the declared stopping rules. |

The validated object must be the executed object: an execution may not claim conformance to a methodology version unless its bound inputs, artifacts, deviations, verification result, and stopping determination are the objects reviewed.

## 6C. Reusable Transformation Classes

Methodology engineering in this repository uses these reusable transformation classes:

```text
Research Need → Research Request
Research Request → Methodology Definition
Methodology + Inputs → Execution
Observations → Evidence Records
Evidence Records → Assessment
Instrument Observations → Calibration Proposal
Calibration Decision → New Version
```

| Transformation class | Source object | Target object | Minimum rule |
| --- | --- | --- | --- |
| Research Need → Research Request | Stated methodological gap or investigation need | Bounded research request | Convert an unbounded need into a reviewable request with question form, scope, constraints, and acceptance disposition. |
| Research Request → Methodology Definition | Accepted request | Versioned methodology definition | Define the contract that can answer the request class without embedding a particular execution. |
| Methodology + Inputs → Execution | Methodology version and declared inputs | Bound execution record | Bind exact identity, version, scope, inputs, provenance obligations, artifacts, verification, deviations, and stopping determination. |
| Observations → Evidence Records | Raw or derived observations | Evidence records | Admit observations only when provenance, source, admissibility, uncertainty, and derivation requirements are satisfied. |
| Evidence Records → Assessment | Evidence records | Assessment or decision outcome | Apply declared decision rules and record strength, uncertainty, alternatives, limitations, and disposition. |
| Instrument Observations → Calibration Proposal | Instrument execution observations and deviations | Calibration proposal | Identify whether instrument behavior supports continuation, limitation, repair, or a new version. |
| Calibration Decision → New Version | Accepted calibration decision | New methodology or instrument version | Create a new immutable version when the contract changes; preserve earlier versions and executions. |

## 6D. Required Supporting Models

### Evidence and Decision Outcomes

Evidence records must identify source, observation or derivation method, admissibility status, provenance, uncertainty, limitations, relationship to the claim or question, and retention location. Decision outcomes must identify the decision rule applied, evidence considered, evidence excluded, confidence or strength statement, unresolved uncertainty, dissent or adjudication record when applicable, and disposition.

### Deviations

A deviation record must identify expected rule, actual event, object affected, time detected, cause, authorization status, corrective action, impact on evidence or output, reviewer, and disposition. Permitted dispositions are: accepted with limitation, corrected, rejected, escalated, execution suspended, or execution failed.

### Failure and Stopping Rules

Failure and stopping rules must distinguish invalid input, missing provenance, unmet evidence requirement, failed verification, unauthorized deviation, instrument failure, irrecoverable ambiguity, and scope breach. Each rule must specify the required response: reject input, pause for amendment, continue with limitation, rerun, supersede, terminate, or mark output unusable.

### Calibration Proposals

A calibration proposal must identify the methodology or instrument version evaluated, reference or pilot execution basis, observed limitation or failure, affected rule, proposed change, expected effect, backward-compatibility assessment, historical-preservation impact, reviewer decision, and whether a new version is required.

### Historical Preservation

Historical preservation requires immutable version identity, immutable execution binding, preserved evidence records, explicit supersession links, and no retroactive rewrite of earlier methodology versions, instrument versions, executions, evidence, assessments, or findings. Later versions may reinterpret future use; they may not silently relabel past objects.

### Named-Instrument Extension

A methodology may define a named instrument as an extension object when a reusable procedure, tool, rubric, questionnaire, model, device, or protocol needs independent identity. The named-instrument extension must include instrument identity, version, applicable methodology context, inputs, outputs, operating rules, calibration requirements, limitations, deviation rules, provenance requirements, execution binding requirements, improvement path, and supersession lineage.

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

- This canon defines a generic methodology-engineering contract and required binding models, not a domain-specific audit instrument or empirical study.
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

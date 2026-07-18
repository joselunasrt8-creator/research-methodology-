# Residual Generic Evidence Lifecycle and Conformance Contract v1.0

**Canonical status:** Residual generic evidence-lifecycle contract v1.0

**Issue:** #4 — Define the Residual Generic Evidence Lifecycle and Conformance Model

**Boundary:** definition only; no methodology execution, empirical evidence, schema, validator, registry, runtime, synchronization, projection engine, repair, scientific determination, authority grant, or execution permission

## 1. Purpose and canonical ownership

This document is the single canonical source for the repository's residual generic evidence objects, lifecycle, admissibility, quality and sufficiency distinctions, contestation and contradiction records, negative and limiting result objects, canonical projections, validated-evidence emission, and evidence-specific cross-repository conformance record.

It extends, but does not restate or supersede, the generic methodology objects, execution binding, provenance, deviation, failure and stopping, calibration, versioning, supersession, and historical-preservation rules in the [Methodology Engineering Canon](METHODOLOGY_ENGINEERING_CANON.md). Those rules remain authoritative for their subjects.

The [Cross-Domain Structology Transfer Audit v0.1](CROSS_DOMAIN_STRUCTOLOGY_TRANSFER_AUDIT_V0_1.md) owns the audit-specific evidence chain and transfer semantics defined in its sections 9 and 16. This contract neither generalizes that mapping chain nor changes the frozen audit.

The [Methodology-to-Instrument Conformance Review v1.0](METHODOLOGY_TO_INSTRUMENT_CONFORMANCE_REVIEW_V1_0.md) is a historical execution artifact. This contract does not rewrite its vocabulary, determination, or calibration observations.

The [Residual Conformance, Negative Capability, and Reconciliation Contract v1.0](RESIDUAL_CONFORMANCE_NEGATIVE_CAPABILITY_AND_RECONCILIATION_CONTRACT_V1_0.md) owns generic conformance outcomes, negative capability, interaction distinctions, authority boundaries, and reconciliation outcomes. This contract references those outcomes and adds only the evidence-specific comparison record required by Issue #4.

Issue #20 retains ownership of maturity evaluation and carry-forward closure. Issue #21 retains ownership of Pattern Hypothesis, Abstraction Candidate, and Primitive Candidate. Neither subject is defined here.

## 2. Artifact classes and repository boundary

| Artifact class | Meaning in this repository |
| --- | --- |
| Canonical artifact | A versioned, normative methodology contract maintained by this repository, including this document and the other documents identified as canonical above. |
| Frozen artifact | A canonical reference surface bound to an immutable revision for a declared use. The Methodology Engineering Canon v0.1 and Cross-Domain Structology Transfer Audit v0.1 remain frozen for their recorded reference surface and are not modified here. |
| Historical artifact | A preserved record of a prior review, audit, execution, or determination. It is evidence about its bound historical state and is not silently updated by a later contract. |
| Execution artifact | A concrete source, observation, evidence record, result, assessment, claim, validation record, or other object created by a methodology execution. Execution artifacts belong in the executing investigation or evidence repository, not in this definition repository. |

Research Methodology owns the reusable contracts in this document. It does not own investigation-specific evidence, execute transformations, accept claims, establish scientific truth, or authorize action. Artifact location, copying, or exchange does not change that boundary.

## 3. Governing distinctions and common object rules

The following distinctions are mandatory:

```text
Source Material
        ≠
Observation
        ≠
Interpretation
        ≠
Evidence
        ≠
Validated Evidence Artifact
```

```text
Observation ≠ Interpretation
Evidence ≠ Claim
Missing Evidence ≠ Negative Evidence
Contradiction ≠ Methodology Failure
Observed Evidence ≠ Canonical Projection
Validated Evidence ≠ Scientific Truth ≠ Authority ≠ Execution Permission
Artifact Exchange ≠ Evidence Equivalence ≠ Authority Transfer
```

**Evidence** is the bounded evidentiary role assigned to an admissible Evidence Record relative to an identified question, claim, transformation, or decision rule. Neither source custody, observation, interpretation, computation, quantity, repository location, nor validation automatically grants that role.

**Negative Evidence** is Evidence whose admitted content supports a bounded proposition of absence, failure to meet a criterion, or incompatibility under a declared rule. It requires the same provenance, admissibility, quality, and purpose-specific sufficiency review as other Evidence; a missing or inaccessible record is not Negative Evidence.

**Observed Evidence** is Evidence whose evidentiary contents remain bound to one or more observations without replacement by a normalized or derived comparison representation. It may include declared interpretation fields, but those fields remain typed as interpretations.

Every object defined here must have a stable identity and declared type. Transfer, copying, projection, validation, citation, or storage in another repository must preserve the original identity and type. A changed object receives a new identity or immutable version and an explicit derivation or supersession link; it must not silently change type merely because it moves to another repository.

The canon's execution-binding, provenance, versioning, stopping, and historical-preservation rules apply to all objects below. The fields in section 4 are the additional evidence-specific minimums.

## 4. Generic evidence object contracts

### 4.1 Source Material

- **Identity:** A stable identity for a bounded pre-observation object, source, dataset, document, signal, specimen reference, system output, or other accessible material.
- **Purpose:** Preserve the exact material from which an observation may be made without treating the material itself as an observation or as evidence for every possible question.
- **Required inputs:** The material or an immutable reference to it; source identity; acquisition or access context; and the applicable scope and custody boundary.
- **Minimum contents:** Source type, locator, creator or origin when known, acquisition time, applicable time period, content version or digest, access conditions, and known integrity state.
- **Provenance requirements:** Origin, custody or access path, acquisition actor or mechanism, timestamps, revisions, transformations already applied before acquisition, and digest or equivalent immutable binding when available.
- **Uncertainty requirements:** Record uncertainty about origin, completeness, authenticity, stability, sampling, access, or content interpretation without converting uncertainty into a source fact.
- **Limitations:** May be inaccessible, mutable, partial, biased, redacted, transformed, duplicated, dependent on another source, or outside the required temporal or semantic scope.
- **Admissibility or validation status:** Unreviewed source material has no evidentiary admissibility status. Its use requires an Evidence Admissibility Review for the specified purpose.
- **Permitted downstream use:** Observation, source-quality review, provenance review, admissibility review, or bounded transformation when a governing methodology permits it.
- **Prohibited interpretation:** The source is an observation, supports a claim, is independent, is complete, or is authoritative merely because it exists or is stored locally.
- **Version or immutable binding requirements:** Bind the exact content revision, snapshot, digest, release, retrieval event, or other immutable state used. A changed source state is a new bound version.

### 4.2 Observation

- **Identity:** A stable identity for a bounded record of what was detected, measured, read, or otherwise registered from identified Source Material or an identified observation context.
- **Purpose:** Record what was observed separately from the meaning, explanation, or inference later assigned to it.
- **Required inputs:** Bound Source Material or declared direct-observation context; observation method or instrument; actor or execution identity; and applicable method version and configuration.
- **Minimum contents:** Observed feature or value, units or representation, time and location or logical context, method, source binding, recorder, and any selection, sampling, or filtering condition.
- **Provenance requirements:** Trace to exact source or observation context, method or instrument identity and version, configuration, actor, time, custody, and any preprocessing that occurred before recording.
- **Uncertainty requirements:** Record measurement, sampling, transcription, detection, classification, temporal, and method uncertainty applicable to the observed content.
- **Limitations:** An observation may be partial, noisy, dependent, method-bounded, inaccessible for replay, or irrelevant to a later question.
- **Admissibility or validation status:** An Observation is not Evidence until its Evidence Admissibility Review assigns an applicable outcome and an Evidence Record binds its evidentiary role.
- **Permitted downstream use:** Admissibility review, interpretation, comparison, contestation, exclusion review, Evidence Record creation, or methodology-permitted transformation.
- **Prohibited interpretation:** An explanation, causal account, assessment, claim, proof, or validated artifact; observed absence is not automatically evidence of absence.
- **Version or immutable binding requirements:** Preserve the original record and exact source, method, and configuration bindings. Correction creates a successor record and retains the prior observation.

### 4.3 Interpretation

- **Identity:** A stable identity for a bounded assignment of meaning to identified Source Material, Observations, Evidence Records, or Computed Results.
- **Purpose:** Make reasoning, categorization, explanation, or semantic judgment explicit rather than embedding it in an observation.
- **Required inputs:** The objects interpreted; interpretation rule, framework, vocabulary, or rationale; interpreter identity; and intended scope.
- **Minimum contents:** Interpreted proposition or meaning, input identities, reasoning trace, alternatives considered, assumptions, scope, and interpreter or adjudicator.
- **Provenance requirements:** Trace to every interpreted object, the exact interpretive rule or framework and version, interpreter, time, and any prior interpretations used.
- **Uncertainty requirements:** Record ambiguity, judgment uncertainty, competing interpretations, assumption sensitivity, and unresolved semantic questions.
- **Limitations:** Interpretation is framework-, actor-, scope-, and time-dependent and may be contested or contradicted without changing the underlying Observation.
- **Admissibility or validation status:** An Interpretation may be reviewed or admitted as an interpretive input, but it does not inherit the admissibility of its source objects and is not Evidence merely by being recorded.
- **Permitted downstream use:** Assessment, computation, contestation, comparison, claim construction, or Evidence Record creation when the governing methodology explicitly permits interpretive evidence.
- **Prohibited interpretation:** A direct Observation, source fact, inevitable meaning, consensus, or scientific truth.
- **Version or immutable binding requirements:** Bind the exact input versions and interpretation rule. A changed meaning, rule, or input set requires a new Interpretation linked to the prior record.

### 4.4 Evidence Record

- **Identity:** A stable identity for the durable record that assigns specified source-bound content an evidentiary role relative to a stated question, claim, transformation, or decision rule.
- **Purpose:** Preserve what is being used as Evidence, why it is relevant, and under what admissibility, provenance, uncertainty, and limitation boundary.
- **Required inputs:** One or more bound Source Materials, Observations, Interpretations, or methodology-permitted derived objects; an Evidence Admissibility Review; and the target question, claim, transformation, or decision rule.
- **Minimum contents:** Evidence identity and type, exact input identities, evidentiary proposition, target relation, admissibility outcome, provenance, uncertainty, limitations, retention location, and current status.
- **Provenance requirements:** End-to-end trace from the record to every source, observation, interpretation, prior transformation, recorder, review, custody event, and applicable version.
- **Uncertainty requirements:** Carry forward all material input uncertainty and add uncertainty introduced by selection, combination, interpretation, or recording. Reduction requires an explicit rule and supporting evidence.
- **Limitations:** Admissibility is purpose-specific; the same record may be irrelevant or insufficient for another question, claim, transformation, or rule.
- **Admissibility or validation status:** Must carry exactly one admissibility outcome from section 6 for its bound purpose. Admissibility is not sufficiency and is not validation.
- **Permitted downstream use:** Quality review, sufficiency review, transformation, computation, assessment, claim support or contradiction, projection, or validation when permitted by the governing methodology.
- **Prohibited interpretation:** A claim, conclusion, scientific truth, complete evidence set, independent corroboration, or execution permission.
- **Version or immutable binding requirements:** Bind exact evidence contents, inputs, target relation, and review version. Any material change creates a new record and preserves the earlier record and supersession history.

### 4.5 Computed Result

- **Identity:** A stable identity for the output of an identified transformation or computation over bound inputs.
- **Purpose:** Separate a derived result from its inputs, the assessment of that result, and any later validated emission.
- **Required inputs:** Exact input objects and versions, transformation or computation identity and version, configuration, execution identity, and declared procedure.
- **Minimum contents:** Result value or representation, input bindings, operation, parameters and configuration, environment when material, execution time, logs or trace reference, and completion or failure status.
- **Provenance requirements:** Full derivation trace to exact inputs, operation version, configuration, execution identity, environment, intermediate objects when material, and any deviations.
- **Uncertainty requirements:** Propagate input uncertainty and record numerical, model, algorithmic, approximation, configuration, and execution uncertainty introduced by computation.
- **Limitations:** Correct execution may still produce an irrelevant, biased, non-reproducible, insufficient, or scientifically unwarranted result.
- **Admissibility or validation status:** A Computed Result is not automatically admissible Evidence and is not validated until the emission contract in section 11 is satisfied.
- **Permitted downstream use:** Verification, reproducibility review, quality or sufficiency review, assessment, projection, claim support, or validated-artifact emission.
- **Prohibited interpretation:** An Assessment, Claim, Validated Evidence Artifact, scientific truth, authority, or permission merely because computation completed.
- **Version or immutable binding requirements:** Bind exact inputs, code or transformation version, configuration, environment when material, and output digest. Re-execution or changed inputs create a distinct result identity.

### 4.6 Canonical Projection

- **Identity:** A stable identity for a bounded, versioned representation derived from identified evidence for declared comparison, conformance, aggregation, or transfer.
- **Purpose:** Make heterogeneous evidence comparable without overwriting, replacing, or relabeling its source evidence.
- **Required inputs:** Exact source evidence identities; projection rule and version; field mapping; intended comparison scope; and applicable normalization or derivation rules.
- **Minimum contents:** Every projection field required by section 10.2, the source-to-projection trace, and exactly one projection outcome from section 10.3.
- **Provenance requirements:** Trace every projected field to source evidence and the rule that preserved, omitted, normalized, or derived it, including actor or execution identity and time.
- **Uncertainty requirements:** Carry source uncertainty and record uncertainty, ambiguity, or comparability risk introduced by mapping, normalization, omission, derivation, or information loss.
- **Limitations:** Validity is restricted to the intended comparison scope and projection version; a projection may be lossy even when valid.
- **Admissibility or validation status:** Projection validity is determined separately from source-evidence admissibility and artifact validation. A valid projection is not proof of source correctness or evidence equivalence.
- **Permitted downstream use:** Declared comparison, conformance, aggregation, or transfer analysis within the intended scope.
- **Prohibited interpretation:** The source evidence itself, a replacement for it, an unbounded canonical truth, an authority transfer, or evidence equivalence across repositories.
- **Version or immutable binding requirements:** Bind exact source versions, rule version, field mapping, and projection digest. Any change requires a new projection and outcome record.

### 4.7 Assessment

- **Identity:** A stable identity for a rule-governed evaluation of identified evidence or results against an identified question, criterion, transformation, or decision rule.
- **Purpose:** Record the evaluative step between evidence or results and a bounded disposition or Claim without duplicating a methodology-specific assessment type.
- **Required inputs:** Bound Evidence Records and, when applicable, Computed Results or Canonical Projections; assessment rule and version; scope; assessor; and required quality and sufficiency determinations.
- **Minimum contents:** Inputs considered, inputs excluded, rule applied, rationale, quality findings, sufficiency outcome, contradictions, unresolved uncertainty, limitations, alternatives, and disposition.
- **Provenance requirements:** Trace to every considered and excluded object, the rule version, assessor or adjudicator, time, and any dissent or contestation records.
- **Uncertainty requirements:** Preserve material input uncertainty and record assessment, decision-rule, disagreement, and residual uncertainty.
- **Limitations:** An Assessment is bounded to its inputs, rule, scope, and time and may be superseded without retroactively changing those inputs.
- **Admissibility or validation status:** Assessment validity depends on its governing methodology and exact input bindings; it does not convert insufficient or inadmissible evidence into sufficient evidence.
- **Permitted downstream use:** Claim formation, validation review, stopping determination, proposal, escalation, or a methodology-specific outcome.
- **Prohibited interpretation:** Direct Observation, Evidence, scientific truth, authority, execution permission, or any methodology-specific assessment unless that methodology explicitly specializes this object.
- **Version or immutable binding requirements:** Bind exact input and rule versions. Any changed evidence set, rule, rationale, or disposition requires a new Assessment with supersession linkage.

### 4.8 Claim

- **Identity:** A stable identity for a bounded proposition asserted for review, acceptance, rejection, qualification, withdrawal, or other methodology-defined disposition.
- **Purpose:** Keep what is asserted distinct from the Evidence Records and reasoning offered in support of or opposition to it.
- **Required inputs:** Claim statement and scope; supporting, contradicting, and missing-evidence relations; relevant Assessment; decision or acceptance rule when applicable; and claimant identity.
- **Minimum contents:** Proposition, type, scope, status, evidence relations, assessment references, uncertainty, limitations, counterexamples, decision owner when applicable, and historical lineage.
- **Provenance requirements:** Trace to claimant, exact supporting and contradicting objects, assessment and rule versions, creation time, reviews, amendments, and dispositions.
- **Uncertainty requirements:** State epistemic and scope uncertainty, sensitivity to assumptions, unresolved conflicts, and limitations on inference.
- **Limitations:** A Claim may be supported, contradicted, unsupported, indeterminate, or withdrawn and remains bounded by the method and evidence available.
- **Admissibility or validation status:** Claim status must be separately determined under a methodology-specific rule. Evidence admissibility, sufficiency, artifact validation, or conformance does not itself accept the Claim.
- **Permitted downstream use:** Review, contestation, decision, publication consideration, validation packaging, proposal, or future reassessment within an authority boundary.
- **Prohibited interpretation:** Evidence itself, scientific truth, authority, execution permission, or acceptance merely because the Claim is recorded or has a validated supporting artifact.
- **Version or immutable binding requirements:** Preserve each claim version and status transition. Amendment or withdrawal creates a successor state without erasing prior identity or evidence relations.

### 4.9 Validated Evidence Artifact

- **Identity:** A stable identity for the exact emitted object produced when the validated-evidence emission contract in section 11 is satisfied.
- **Purpose:** Bind a Computed Result to exact inputs, transformation, verification evidence, provenance, uncertainty, limitations, digest, execution identity, and stopping determination for bounded downstream reliance.
- **Required inputs:** Computed Result, bound inputs, transformation identity, exact configuration, verification evidence, verification rule, execution identity, and stopping determination.
- **Minimum contents:** Every binding required by section 11.2 and the emitted artifact itself or its immutable locator.
- **Provenance requirements:** End-to-end trace from emitted artifact through result, execution, transformation, configuration, exact evidence inputs, verification, and custody.
- **Uncertainty requirements:** Preserve input and result uncertainty and explicitly state uncertainty introduced, reduced, or unresolved by verification.
- **Limitations:** Validation establishes satisfaction of a declared verification rule for the exact artifact, not scientific truth, universal fitness, authority, or permission.
- **Admissibility or validation status:** Must carry the exact verification result and validation scope. Failed, blocked, or indeterminate verification does not emit a Validated Evidence Artifact.
- **Permitted downstream use:** Bounded evidence exchange, review, comparison, conformance, assessment, or claim support when the receiving methodology separately admits it.
- **Prohibited interpretation:** Scientific truth, authority, execution permission, automatic claim acceptance, evidence equivalence, or validation of any changed artifact.
- **Version or immutable binding requirements:** Bind the artifact digest and all exact versions. Any artifact or binding change requires a new validation record and, if successful, a new emitted artifact identity.

## 5. Generic evidence lifecycle

The generic composable lifecycle is:

```text
Source Material
        ↓
Observation
        ↓
Evidence Admissibility Review
        ↓
Evidence Record
        ↓
Transformation or Computation
        ↓
Computed Result
        ↓
Assessment
        ↓
Claim or Validated Evidence Artifact
```

Interpretation may occur as an explicit branch after Source Material, Observation, Evidence Record, or Computed Result. Canonical Projection may occur as an explicit branch from Evidence Record or Validated Evidence Artifact for bounded comparison. Neither branch changes the type of its inputs.

This lifecycle is a reusable vocabulary, not a mandatory universal pipeline. A methodology may omit inapplicable stages, stop earlier, accept a Validated Evidence Artifact as an input, or specialize a transition. It must record the applicable stages and preserve every distinction, input binding, uncertainty, limitation, stopping rule, and historical obligation used here. It must not use omission to bypass an admissibility, sufficiency, verification, or authority gate that applies to its intended output.

### 5.1 Transition contract

| Transition | Entry criteria and required inputs | Transition rule and required evidence or records | Permitted outputs | Stop, reject, or block conditions |
| --- | --- | --- | --- | --- |
| Source Material → Observation | Exact source identity and version or observation context; accessible content; declared method, actor, scope, and configuration. | Record the observed content without embedding interpretation; create the Observation. Required evidence is the source binding, access or acquisition record, method and configuration binding, and observation provenance. | Observation; Missing Evidence Record; Evidence Gap; source limitation or exclusion proposal. | Stop when the requested observation is complete or out of scope. Reject a source for this transition only when sufficient evidence establishes a source or method exclusion rule. Use `BLOCKED` when required access, identity, version, method, or provenance is unavailable. |
| Observation → Evidence Admissibility Review | Bound Observation, target question/claim/transformation/rule, admissibility criteria, provenance, uncertainty, and known limitations. | Apply section 6 without treating missing evidence as failed evidence. Required evidence is the observation and source provenance, criteria binding, target relation, uncertainty, limitations, and applicable contestation, contradiction, or exclusion records. | One admissibility outcome and its review record. | Stop on `INADMISSIBLE` or `NOT_APPLICABLE` for the bound purpose. Pause on `BLOCKED`; fail closed on `INDETERMINATE`. Rejection requires evidenced failure of an admissibility requirement. |
| Admissibility Review → Evidence Record | Review outcome, exact reviewed object, target evidentiary relation, recorder, retention location, and version bindings. | Create an Evidence Record only for `ADMISSIBLE` or `ADMISSIBLE_WITH_LIMITATIONS`; carry every limitation and uncertainty. Required evidence is the complete review record, rule trace, provenance, and exact reviewed-object binding. | Evidence Record; or preserved non-admission review record. | Stop if the review is `INADMISSIBLE` or `NOT_APPLICABLE`. Pause for `BLOCKED`. Reject Evidence Record creation for an evidenced inadmissible object. Do not create an evidentiary role for `INDETERMINATE`. |
| Evidence Record → Transformation or Computation | Admitted Evidence Records; transformation identity and version; required configuration; input sufficiency rule; execution identity; scope. | Bind exact inputs before execution. Required evidence is each admissibility record, the input sufficiency determination, transformation and configuration binding, provenance, deviations, intermediate records, and stopping rule. | Computed Result; Unsupported Result; Indeterminate Result; methodology-failure record; execution logs. | Reject invalid inputs only when an applicable rule is demonstrably failed. Block when a required input, dependency, configuration, or authority is unavailable. Stop on declared terminal, failure, safety, scope, or sufficiency conditions. |
| Transformation or Computation → Computed Result | Completed or terminal execution record with bound inputs and operation identity. | Emit a typed Computed Result even when its scientific direction is negative, null, limiting, or indeterminate. Required evidence is the complete execution and derivation trace, input and operation bindings, uncertainty and limitations, deviations, and stopping determination. | Computed Result and, when applicable, a section 9 result object. | Stop when the operation reaches a declared terminal state. Reject a result classification when sufficient evidence establishes that its required execution record is invalid. Block when a known prerequisite prevents a terminal execution record. A failed execution produces a methodology-failure record, not a scientific Negative Result. |
| Computed Result → Assessment | Bound result, contributing Evidence Records, assessment rule and version, quality review, sufficiency question, contradictions, exclusions, and assessor. | Apply declared assessment rules. Required evidence is result provenance, considered and excluded evidence, quality findings, sufficiency review, rule trace, contradictions, uncertainty, limitations, and alternatives. | Assessment; contestation or conflict records; request for additional evidence; stopping determination. | Stop when the assessment rule reaches a terminal disposition. Reject a proposed conclusion only under an evidenced rule. Block on an identified preventing prerequisite; use `INDETERMINATE` for unresolved evidentiary interpretation. |
| Assessment → Claim | Completed Assessment, claim statement and scope, supporting and contradicting evidence, sufficiency outcome, claimant, and applicable decision rule. | Create or update a Claim without merging it with Evidence. Required evidence is the Assessment and rule trace, exact supporting and contradicting records, sufficiency outcome, uncertainty, limitations, conflicts, and authority boundary. | Claim with methodology-defined status; Unsupported, Withdrawn, or Indeterminate Result when applicable. | No supported claim may issue from `INSUFFICIENT`, `BLOCKED`, or `INDETERMINATE` evidence sufficiency. Reject a proposed status only under an evidenced decision rule; block when a known prerequisite prevents status determination. Stop or narrow scope as the governing rule requires. |
| Computed Result → Validated Evidence Artifact | Computed Result plus every exact binding and verification input in section 11. | Verify the exact emitted object under the declared rule. Required evidence is every binding, verification record, verification result, artifact digest, execution identity, limitation, uncertainty, and stopping determination required by section 11. | Validated Evidence Artifact only on successful verification; otherwise a verification, blocked, indeterminate, or failure record. | Reject emission when verification evidence establishes failure. Block or stop without emission when verification is blocked, indeterminate, incomplete, or targets a different artifact. A changed artifact requires a new validation record. |

### 5.2 Lifecycle-wide rules

- **Entry criteria:** The applicable methodology, intended question or purpose, source or input identity, required versions, provenance expectation, and authority boundary must be declared before the first applicable transition.
- **Required records:** Each applied transition records its exact inputs, output identity and type, rule and version, actor or execution identity, time, provenance, uncertainty, limitations, deviations, and stopping determination. Existing canon owns the generic execution-binding shape.
- **Permitted outputs:** Only the typed outputs declared for the transition or a methodology-specific specialization may issue. A record of failure, blocking, missingness, contradiction, exclusion, or indeterminacy is an output; it is not permission to fabricate the expected success object.
- **Stopping conditions:** Stop at the methodology's declared terminal stage, when the bounded question is answered with required sufficiency, when a terminal non-applicability or rejection rule applies, when a required withdrawal occurs, or when the canon's stopping rules require suspension or termination.
- **Rejection conditions:** Rejection requires admissible evidence that an applicable requirement failed. Missing, inaccessible, ambiguous, or insufficiently discriminating evidence alone does not establish rejection.
- **Blocked conditions:** Use a blocked outcome when a known required prerequisite prevents the transition. Identify the prerequisite, affected scope, responsible boundary when known, unblock condition, and permitted non-executing follow-up.
- **Fail-closed rule:** Required missing or inaccessible evidence produces a Missing Evidence Record and the applicable `BLOCKED`, `INDETERMINATE`, or `INSUFFICIENT` outcome. It never defaults to admissible, sufficient, valid, conforming, negative, or not applicable.
- **Uncertainty propagation:** Every transition carries material input uncertainty and limitations forward. It may add uncertainty. It may reduce or resolve uncertainty only under an explicit rule with cited evidence; the prior uncertainty remains in historical lineage.
- **Version binding:** Every transition binds exact input objects, governing rule, method, transformation, configuration, and output version or digest. A changed binding requires a new transition record.
- **Historical preservation:** Records are append-only for their bound state. Correction, reassessment, supersession, withdrawal, transfer, or projection preserves prior identities, contents, statuses, provenance, and lineage.

## 6. Evidence admissibility model

Admissibility asks whether an identified object may serve as Evidence for one stated purpose under one declared rule. It does not ask whether the evidence set is sufficient to answer the question.

Every Evidence Admissibility Review binds the reviewed object and version, intended evidentiary purpose, admissibility criteria and version, evidence considered, reviewer, provenance, uncertainty, limitations, decision trace, time, and exactly one outcome below.

| Outcome | Required evidence | Decision rule | Permitted interpretation | Prohibited interpretation | Continuation rules | Supersession behavior |
| --- | --- | --- | --- | --- | --- | --- |
| `ADMISSIBLE` | Complete review evidence for every applicable admissibility criterion, exact object and rule versions, and no material unresolved limitation. | Every applicable mandatory criterion is satisfied. | The object may serve as Evidence for the bound purpose. | Sufficient, true, independent, complete, accepted, or admissible for another purpose. | Create an Evidence Record or continue to the next declared gate. | A successor cites changed evidence, object, rule, or scope; the original review remains historical. |
| `ADMISSIBLE_WITH_LIMITATIONS` | Evidence satisfying every applicable mandatory criterion plus explicit material limitations and carry-forward requirements. | No criterion fails, but bounded limitations qualify use or interpretation. | The object may serve as Evidence only within the recorded limits. | Unqualified admissibility, waiver of failure, or removal of limitations without evidence. | Continue only within scope and carry every limitation into dependent records. | A limitation is removed only by a successor citing evidence that resolves it; history remains visible. |
| `INADMISSIBLE` | Admissible review evidence identifying each failed mandatory criterion and distinguishing failure from missingness or uncertainty. | At least one applicable mandatory criterion is demonstrably unsatisfied. | The object may not serve as Evidence for the bound purpose. | Scientifically false, useless for all purposes, or failed merely because evidence is missing. | Do not create an Evidence Record for that purpose; exclusion, correction, a new purpose, or new version may be reviewed. | A successor requires a changed object, rule, purpose, or new evidence and preserves the failed review. |
| `BLOCKED` | Evidence identifying an unmet prerequisite, why it is required, what review it prevents, and the unblock condition. | The admissibility review cannot be completed because a known prerequisite is unavailable. | No admissibility determination can presently be made for the blocked scope. | Admissible, inadmissible, indeterminate merely by uncertainty, or permission to bypass the prerequisite. | Pause dependent use; evidence collection, access request, clarification, proposal, or escalation may continue. | A successor cites disposition of the blocker; the blocked record is retained. |
| `INDETERMINATE` | Available review evidence, competing or unsupported interpretations, and the ambiguity or contradiction preventing one defensible result. | Review is possible, but evidence cannot discriminate between admissible and inadmissible. | Admissibility cannot be defensibly selected from current evidence. | Admissibility by default, inadmissibility by suspicion, or a known external blocker. | Do not create an Evidence Record for the unresolved purpose; collect evidence, clarify rules, narrow scope, or escalate. | A successor cites resolution of the ambiguity; unresolved portions remain indeterminate. |
| `NOT_APPLICABLE` | The explicit applicability rule, object facts, and rationale affirmatively excluding this review or criterion. | The evidentiary purpose or criterion does not apply in the recorded scope. | No admissibility determination is required for the excluded scope. | Admissible, inadmissible, waived, ignored, or missing evidence. | Skip only the affirmatively excluded review or criterion; other gates remain. | A successor requires a changed rule, object, purpose, or scope; the original remains historical. |

Missing evidence must not be treated as `INADMISSIBLE` unless sufficient evidence separately establishes failure of an admissibility requirement. When the missing evidence is itself a known prerequisite, use `BLOCKED`; when review can proceed but cannot resolve the outcome, use `INDETERMINATE`.

## 7. Evidence quality and sufficiency model

```text
Evidence Quality ≠ Evidence Sufficiency
```

Evidence Quality describes properties of identified Evidence Records. Evidence Sufficiency determines whether a particular evidence set meets the needs of a specific question, Claim, transformation, or decision rule. High-quality evidence may still be insufficient. A large quantity of evidence may still be low quality. Quantity is neither quality nor sufficiency.

### 7.1 Evidence-quality dimensions

Each quality review binds the Evidence Records, quality rule and version, reviewer, scope, findings by applicable dimension, uncertainty, limitations, contradictions, and provenance. A methodology may specialize thresholds, but it must not collapse distinct dimensions.

| Dimension | Generic question |
| --- | --- |
| Provenance integrity | Can origin, custody, derivation, actors, timestamps, and versions be traced without a material break? |
| Source identity | Is the source stably and correctly identified at the exact state used? |
| Source independence | Are purportedly independent sources genuinely non-dependent under the declared relation and time boundary? |
| Relevance | Does the evidence bear on the exact question, Claim, transformation, or rule being evaluated? |
| Completeness | Are required fields, components, intervals, and associated records present for the evidence object itself? |
| Coverage | Does the evidence represent the required population, cases, conditions, time range, or scope? |
| Freshness | Is the evidence current enough for the declared temporal rule and decision context? |
| Consistency | Are repeated values, representations, or claims internally and externally compatible under the comparison rule? |
| Reproducibility | Can the observation, derivation, or result be independently reconstructed or repeated to the degree required? |
| Uncertainty | Are material uncertainties identified, bounded where possible, and carried without unjustified reduction? |
| Limitation severity | How materially do recorded limitations restrict use, confidence, scope, or inference? |
| Contradiction status | Are supporting and contradictory records visible, classified, materiality-assessed, and unresolved conflicts preserved? |
| Transformation traceability | Can each transformation, configuration, field change, omission, normalization, and derivation be traced to exact inputs and rules? |

A quality finding must state the rule and scale used; this contract defines dimensions, not a universal score or maturity model.

### 7.2 Evidence-sufficiency outcomes

Every sufficiency review binds one specific question, Claim, transformation, or decision rule; the exact Evidence Records considered and excluded; applicable quality findings; required coverage or threshold; contradictions; Missing Evidence Records and Evidence Gaps; reviewer; provenance; uncertainty; limitations; and exactly one outcome below.

| Outcome | Decision rule and required evidence | Permitted interpretation and continuation | Prohibited interpretation and supersession |
| --- | --- | --- | --- |
| `SUFFICIENT` | Complete admissible evidence meets every applicable requirement for the bound question or rule, with no material unresolved gap, contradiction, or limitation. | The evidence set is sufficient only for the bound purpose; the next declared assessment or decision gate may proceed. | Not scientific truth, claim acceptance, universal sufficiency, or permission. A successor must cite changed evidence, rule, or scope and preserve this record. |
| `SUFFICIENT_WITH_LIMITATIONS` | Every mandatory sufficiency requirement is met, but explicit material limitations restrict scope or interpretation without concealing a failed requirement. | Proceed only within the limited scope and carry limitations into every dependent object. | Not unqualified sufficiency or waiver. Removal of a limitation requires a successor with resolving evidence. |
| `INSUFFICIENT` | Review is complete enough to establish that the current evidence set does not meet one or more stated sufficiency requirements, without implying the underlying proposition is false. | Do not make the dependent supported Claim or decision; collect evidence, narrow the question, or issue an Unsupported Result as permitted. | Not `INADMISSIBLE`, Negative Result, methodology failure, or scientific falsity. A successor cites the added or changed evidence and preserves history. |
| `BLOCKED` | A known required prerequisite prevents the sufficiency review from being completed; the prerequisite and unblock condition are recorded. | Pause the dependent determination; evidence collection, access request, clarification, proposal, or escalation may continue. | No underlying sufficiency result may be inferred. A successor cites blocker disposition and retains the blocked record. |
| `INDETERMINATE` | Review is possible, but ambiguity, contradiction, uncertainty, or insufficiently discriminating evidence prevents one defensible sufficient or insufficient result. | Do not make the dependent supported Claim; clarify, collect evidence, narrow scope, or escalate. | Not sufficiency by default, insufficiency by suspicion, or a known blocker. A successor cites resolution; unresolved portions remain. |
| `NOT_APPLICABLE` | An explicit rule affirmatively excludes a sufficiency review for the bound object or scope. | Skip only the excluded review; independent applicable gates remain. | Not sufficient, insufficient, waived, blocked, or inferred from missing evidence. A successor requires a changed applicability boundary. |

## 8. Contestation, contradiction, exclusion, and missingness

The records in this section are first-class execution objects. Each record must identify the affected evidence identities and versions; relevant source and provenance; reason; reviewer or recorder; materiality; impact on Assessment or Claim; required follow-up; status; and complete supersession history. It must also record creation time, scope, uncertainty, limitations, and related records when applicable.

| Record | Distinct purpose | Minimum additional contents and rules |
| --- | --- | --- |
| Evidence Contestation | Records a reasoned challenge to evidence identity, provenance, admissibility, quality, relevance, interpretation, use, or status. | Challenger identity, contested proposition or field, basis and supporting evidence, response owner when known, response, adjudication status, and affected downstream objects. Contestation does not by itself invalidate or erase evidence. |
| Contradiction Record | Records materially incompatible evidence contents, observations, interpretations, results, or claims under a declared comparison rule. | All contradictory object identities, conflicting propositions or fields, comparison rule, contradiction type, materiality rationale, and whether the contradiction is resolved, bounded, or unresolved. Contradictory evidence remains visible even after adjudication. |
| Evidence Exclusion | Records that identified material was not used for a specified evidentiary purpose. | Exclusion rule and version, decision evidence, excluded scope, whether exclusion occurred before or after review, and downstream effect. Excluded evidence remains traceable and may be reviewed for another purpose. |
| Missing Evidence Record | Records required evidence that is absent, inaccessible, not produced, lost, mutable when immutability is required, or otherwise unavailable. | Expected evidence identity or class, requirement source, discovery method, availability state, responsible boundary when known, and unblock or recovery condition. Missingness is not negative evidence. |
| Evidence Gap | Records the difference between the evidence required for a specific purpose and the admissible evidence currently available. | Bound question, Claim, transformation, or rule; required evidence; available evidence; gap materiality; effect on sufficiency; and closure evidence required. A gap may exist even when every available item is high quality. |
| Unresolved Evidence Conflict | Records a material contradiction or contestation that applicable review cannot resolve to one defensible evidentiary disposition. | Linked contestation and Contradiction Records, competing interpretations, attempted resolution, reason resolution failed, affected scope, stopping effect, and evidence or rule clarification needed. It must remain visible in every dependent Assessment and Claim. |

No contradiction, exclusion, contestation, or missingness record may overwrite the affected evidence. Resolution creates a successor status or adjudication record and preserves the original record, all competing evidence, and the complete reasoning history.

## 9. Negative and limiting result objects

```text
Negative Result ≠ Missing Evidence ≠ Methodology Failure
```

Every object in this section must identify its stable identity and type; exact question or expected effect; bound inputs and Evidence Records; governing method, decision rule, and versions; result and rationale; provenance; uncertainty; limitations; contradictions and exclusions; reviewer; status; downstream interpretation boundary; and supersession history.

| Object | Decision rule and bounded meaning | Prohibited interpretation and continuation |
| --- | --- | --- |
| Negative Result | Adequate admissible and sufficient evidence supports the bounded determination that the specified expected condition, relation, effect, threshold, or criterion was not met. | Not missing evidence, proof of universal absence, methodology failure, or scientific falsity outside scope. It may support a bounded Assessment or Claim while limitations remain visible. |
| Null Result | Under the declared design and decision rule, adequate evidence does not establish the specified non-null effect or difference at the required threshold. | Not proof of no effect in all contexts, not automatically a Negative Result of every type, and not a failed execution. Preserve power, sensitivity, threshold, and uncertainty limitations. |
| Counterexample | Admissible evidence establishes an in-scope instance incompatible with an identified universal or scope-bounded proposition under its stated applicability rule. | Not automatic rejection of a differently scoped Claim and not proof that all related propositions fail. Record applicability, representativeness limits, and the affected Claim relation. |
| Limiting Case | Evidence establishes a boundary condition, extreme case, or scope edge at which a method, relation, result, or Claim changes, ceases to apply, or cannot be extended. | Not a universal failure or permission to extrapolate beyond the evidenced boundary. It may narrow scope or qualify an Assessment or Claim. |
| Unsupported Result | A proposed result or Claim lacks evidence sufficient for the required support rule, including after a completed `INSUFFICIENT` review. | Not a Negative Result, contradiction, or proof that the proposition is false. Do not advance it as supported; evidence collection or scope revision may continue. |
| Withdrawn Result | A previously identified result is no longer advanced because of cited error, superseding evidence, invalidated input, rule change, conflict, or authorized withdrawal decision. | Withdrawal does not erase the prior identity, content, provenance, citations, or downstream history and does not automatically negate related results. Preserve reason, withdrawer and authority evidence, effective time, affected uses, and successor when any. |
| Indeterminate Result | Available admissible evidence and applicable rules cannot support one defensible positive, negative, null, limiting, or unsupported determination for the bound question. | Not a convenient result selection, known external blocker, or permission to omit uncertainty. Record competing interpretations and required resolution evidence. |

A Negative Result requires adequate evidence for the negative determination. A methodology failure is recorded under the canon's failure semantics and must not be represented as a scientific Negative Result. Missing Evidence produces the records and outcomes defined in sections 5, 6, 7, and 8; it does not establish a Negative Result.

## 10. Observed evidence and canonical projection

### 10.1 Distinction

```text
Observed Evidence ≠ Canonical Projection
```

A Canonical Projection is a bounded representation used for declared comparison, conformance, aggregation, or transfer. Projection creates a new object; it never overwrites, replaces, mutates, or silently normalizes the source Evidence Record or Validated Evidence Artifact.

### 10.2 Canonical Projection record

Every projection must record:

- stable projection identity and status;
- every source evidence identity, type, exact version, and digest when available;
- transformation or projection rule and exact version;
- complete source-to-target field mapping;
- fields preserved without semantic change;
- fields omitted and the reason for omission;
- fields normalized and the normalization rule;
- fields derived and the derivation rule and inputs;
- uncertainty introduced or changed by projection;
- information loss, including loss whose materiality is unknown;
- projection version and artifact digest;
- intended comparison scope and prohibited scopes;
- actor or execution identity, time, configuration, provenance, limitations, and deviations;
- source Evidence Record admissibility status without treating it as projection validity; and
- exactly one projection outcome from section 10.3 with decision-rule trace.

### 10.3 Projection outcomes

| Outcome | Decision rule | Continuation and prohibited inference |
| --- | --- | --- |
| `PROJECTION_VALID` | Complete evidence shows the projection satisfies every applicable mapping, traceability, version, uncertainty, and information-loss rule for its intended comparison scope with no material limitation. | Use only for the declared comparison. Do not infer source correctness, evidence equivalence, scientific truth, or authority. |
| `PROJECTION_VALID_WITH_LIMITATIONS` | Every mandatory projection rule is satisfied, but explicit material mapping, comparability, uncertainty, or information-loss limitations qualify use. | Continue only inside the limited scope and preserve all limitations. No failed mandatory rule may be relabeled as a limitation. |
| `PROJECTION_DRIFT` | Sufficient evidence establishes that the projection no longer matches its bound source, rule, field mapping, version, or intended comparison contract. | Do not use it as a current conforming projection. Create a new projection or bounded proposal; never mutate the historical projection or source evidence. |
| `PROJECTION_BLOCKED` | A known prerequisite prevents projection creation or review; the prerequisite, affected scope, and unblock condition are identified. | Pause dependent comparison. Do not infer validity, drift, or source-evidence status. |
| `PROJECTION_INDETERMINATE` | Projection review is possible, but ambiguity, contradiction, unresolved identity, or insufficiently discriminating evidence prevents one defensible valid or drift result. | Do not use for a projection-dependent claim. Clarify, collect evidence, or narrow scope while preserving unresolved records. |

A changed source, projection rule, mapping, field treatment, scope, configuration, or projected artifact requires a new Canonical Projection and projection outcome. Historical projections remain bound to the states they represented.

## 11. Validated evidence emission

The generic emission contract is:

```text
Computed Result
        +
Bound Inputs
        +
Transformation Identity
        +
Verification Evidence
        ↓
Validated Evidence Artifact
```

### 11.1 Emission rule

The exact object verified must be the object emitted. Validation of a procedure, earlier run, similar object, source repository copy, or pre-change digest does not validate the emitted artifact. Verification failure, blocking, or indeterminacy produces the applicable record and no Validated Evidence Artifact.

### 11.2 Required bindings

A Validated Evidence Artifact must bind:

- exact source evidence identities, types, versions, admissibility outcomes, and digests when available;
- exact input identities, versions, and immutable locators;
- exact transformation or computation identity and version;
- exact parameters, configuration, environment, dependencies, and intermediate objects when material;
- complete provenance and custody path;
- exact Computed Result and result digest;
- propagated and introduced uncertainty;
- all material limitations, exclusions, contradictions, contestations, missing evidence, and unresolved conflicts;
- verification rule and exact version;
- verification evidence and exact verification result;
- emitted artifact identity, version, locator, and digest;
- execution identity, actor or mechanism, time, and applicable deviations;
- stopping determination; and
- validation-record identity, status, and supersession history.

```text
Validated Evidence ≠ Scientific Truth ≠ Authority ≠ Execution Permission
```

Validation establishes only that the exact emitted artifact satisfies the declared verification rule within its recorded scope. Receiving repositories must separately review admissibility, sufficiency, conformance, and authority for their intended use. A changed artifact, digest, input, transformation, configuration, verification rule, or material execution environment requires a new validation record; prior validation remains historical evidence.

## 12. Cross-repository evidence conformance

### 12.1 Boundary and outcome ownership

Cross-repository evidence conformance is an evidence-specific comparison of exact evidence-object states across identified repositories. It does not redefine generic conformance or reconciliation. The comparison record must select and reference exactly one applicable generic conformance outcome from section 3 of the [Residual Conformance, Negative Capability, and Reconciliation Contract v1.0](RESIDUAL_CONFORMANCE_NEGATIVE_CAPABILITY_AND_RECONCILIATION_CONTRACT_V1_0.md); when registry reconciliation is actually required, that document's section 6 remains controlling.

The evidence-specific record may compare source evidence, transferred evidence, projected evidence, Validated Evidence Artifacts, repository-local copies, and referenced external evidence. It records equivalence evidence or discrepancies; it does not grant equivalence, ownership, authority, custody beyond the recorded copy, repair permission, synchronization, or execution permission.

### 12.2 Evidence-Conformance Record

Every cross-repository Evidence-Conformance Record must include:

| Field | Required evidence-specific content |
| --- | --- |
| Identity and status | Stable record identity, creation time, recorder or execution identity, current status, and supersession history. |
| Object identities | Stable identities, types, roles, versions, and digests of every source, transferred, projected, validated, local-copy, or externally referenced evidence object compared. |
| Repositories compared | Exact repository identities and bounded roles, including which object is canonical, copied, transferred, projected, validated, or referenced when that role is evidenced. |
| Exact revisions | Immutable commit, release, snapshot, registry revision, retrieval event, or equivalent state for every repository and external reference actually compared. |
| Digests | Content and artifact digests used to test identity or equivalence, plus algorithms and unresolved digest absence or mismatch. |
| Comparison rules | Declared identity, byte-equivalence, semantic-equivalence, version, field, completeness, materiality, and precedence rules applicable to the evidence types. |
| Provenance | End-to-end source, custody, transfer, copy, derivation, projection, validation, recorder, and comparison provenance required by the canon. |
| Projection rules | Canonical Projection identities, versions, mappings, field treatments, information loss, outcomes, and limitations when comparison uses projected evidence. |
| Missing evidence | Every absent, inaccessible, mutable, unverified, or insufficient required object or binding and its effect on comparison. |
| Discrepancies | Identity, version, digest, content, provenance, admissibility, uncertainty, limitation, projection, validation, scope, or authority discrepancies with materiality. |
| Limitations | Access, temporal, scope, semantic, comparison, provenance, projection, uncertainty, and interpretation limits. |
| Generic conformance outcome | An exact reference to one outcome and its rule trace under Issue #9's generic conformance model; the outcome vocabulary is not redefined here. |
| Authority boundary | What may be compared, recorded, proposed, or escalated and explicit prohibitions on evidence-equivalence inference, ownership or authority transfer, mutation, repair, synchronization, claim acceptance, and execution. |
| Follow-up | `NONE`, bounded evidence collection, clarification, a non-mutating proposal, or escalation; target decision owner or `UNRESOLVED` owner status; required evidence; and stopping condition. |

Every comparison binds exact repository and object states. Artifact movement, matching names, matching locations, successful projection, successful validation, or a prior conformance record does not by itself establish evidence equivalence. A later revision, digest, projection, validation, repository state, or comparison rule requires a new record and preserves the prior comparison.

```text
Artifact Exchange ≠ Evidence Equivalence ≠ Authority Transfer
```

## 13. Specialization and precedence

A methodology-specific contract may:

- omit lifecycle stages that are affirmatively inapplicable;
- add domain-specific evidence types, quality dimensions, thresholds, or decision rules;
- specialize transitions and stopping rules;
- require stricter admissibility, sufficiency, projection, or validation conditions; and
- define methodology-specific assessments, claims, and outcomes.

A specialization must identify this contract and its exact version, declare applicable and omitted stages, map specialized objects to the generic distinctions without merging them, preserve provenance and uncertainty, and state any stricter rule. It must not weaken fail-closed missing-evidence handling, historical preservation, source/projection separation, emitted-object validation, or authority boundaries.

When a named methodology has a more specific rule within its owned scope, that rule governs the execution and this contract supplies only the residual generic semantics. In particular, the frozen Cross-Domain Structology Transfer Audit retains exclusive ownership of its mapping and transfer sequence.

## 14. Intentional deferrals and non-goals

This contract intentionally does not:

- modify the frozen Methodology Engineering Canon v0.1 or Cross-Domain Structology Transfer Audit v0.1;
- rewrite the historical Issue #33 conformance review;
- implement Issues #1, #3, #5, #8, #10, #20, or #21;
- define Pattern Hypothesis, Abstraction Candidate, Primitive Candidate, maturity scoring, or carry-forward closure;
- execute a research methodology or create empirical evidence;
- create schemas, validators, registries, runtimes, synchronization, automatic projection, automatic repair, or deterministic analysis systems;
- select evidence, instruments, designs, or research conclusions for a concrete investigation;
- claim scientific correctness or accept a scientific Claim; or
- grant authority, ownership transfer, mutation permission, or execution permission.

## 15. Version and preservation

This contract is **Residual Generic Evidence Lifecycle and Conformance Contract v1.0**. Its definitions are canonical for the residual Issue #4 scope only.

Any substantive change to object distinctions, lifecycle transitions, admissibility, quality or sufficiency models, contestation and conflict records, result objects, projection rules, validated emission, evidence-specific conformance record, specialization, or boundary requires a new version. Supersession must preserve this version and every execution artifact bound to it under the Methodology Engineering Canon's historical-preservation rules.

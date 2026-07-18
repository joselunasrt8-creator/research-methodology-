# Methodology Completeness Audit

> [!IMPORTANT]
> This is a historical audit of repository baseline `f1a3b3e`, performed on
> 2026-07-17. Later methodology canon and named-instrument changes may resolve
> findings recorded here. This document is preserved as audit evidence and is not
> the current completeness determination.

**Audit date:** 2026-07-17  
**Baseline:** repository state at commit `f1a3b3e`  
**Audit question:** Is the documented methodology sufficient for an independent
researcher, with no prior program knowledge, to conduct and reproduce an
investigation?

## Scope and assessment rule

This is an audit of methodological completeness, not of the merit, validity, or
truth of any research. It treats the repository as the sole source of methodology.
The named research stack and repository boundaries are context, not undocumented
methodological instructions.

A stage is **specified** only when the repository defines all of the following in a
domain-independent way:

1. required inputs and their admissibility criteria;
2. required outputs and their completion criteria;
3. deterministic rules, or a recorded and reviewable procedure, for every material
   decision;
4. durable artifacts sufficient to inspect and replay the stage;
5. failure conditions and the required response to each; and
6. stable links between inputs, decisions, outputs, and later claims.

Under this rule, a stage name or scope bullet is not a procedure. A downstream
repository may instantiate the methodology, but its undocumented conventions cannot
complete this repository's general methodology.

## Executive determination

**The current methodology is not sufficient for an independent reproducible
investigation.** The README establishes purpose, scope, non-scope, and repository
ownership boundaries, but it does not define a research procedure, decision rules,
artifact schemas, stage gates, traceability requirements, or replay conditions.
All nine stages are therefore underspecified. An investigator would have to supply
the operative methodology from personal judgment.

The boundary principle—methodology is not research execution—is compatible with a
complete methodology. Completeness requires this repository to specify the reusable
contracts governing an execution; it does not require this repository to contain an
empirical study or operational software.

## End-to-end stage audit

### 1. Research Request

**Required inputs**

- A question or problem statement, sponsor and intended audience, claimed domain,
  practical constraints, relevant prior knowledge, and declared interests.
- Definitions of the unit of analysis, population or system boundary, desired
  inference, time horizon, and acceptable evidence.

**Required outputs**

- A versioned, uniquely identified request with a bounded research question,
  definitions, scope and exclusions, stakeholders, constraints, success criteria,
  and change history.
- A disposition: accepted, rejected, deferred, or returned for clarification, with
  reasons.

**Decision rules**

- Rules for feasibility, researchability, ethical acceptability, scope adequacy,
  conflicts of interest, and what constitutes a material request change.
- A precedence rule for conflicting sponsor, investigator, and methodological
  constraints.

**Required artifacts**

- Research-request record; terminology register; constraint and assumption log;
  conflict-of-interest declaration; request revision log.

**Failure modes**

- An untestable question, undefined population, solution prescribed as a premise,
  unavailable required evidence, conflicting objectives, or scope drift.

**Sources of ambiguity**

- “Research request” is not currently defined. The requester’s authority, the
  difference between goals and claims, and the threshold for acceptance are unknown.

**Opportunities for standardization**

- A request contract, controlled dispositions, minimum-entry checklist, definition
  format, and stable identifiers.

**Current determination:** Underspecified; no intake contract or acceptance gate is
documented.

### 2. Investigation Design

**Required inputs**

- Accepted request, prior work, candidate explanations, constraints, units of
  analysis, and the intended class of inference.

**Required outputs**

- A preregistered or otherwise time-stamped protocol specifying research questions,
  hypotheses where applicable, design type, cases or sample, variables and
  constructs, controls, comparison logic, analysis plan, validity threats, stopping
  rules, deviations policy, and amendment procedure.

**Decision rules**

- Rules for choosing exploratory versus confirmatory work; selecting cases, samples,
  controls, and comparisons; setting inclusion and exclusion criteria; determining
  sufficiency or saturation; and handling protocol amendments.

**Required artifacts**

- Investigation protocol; design rationale; causal or conceptual model when used;
  sampling frame; validity-threat register; protocol version and amendment log.

**Failure modes**

- Design cannot answer the request, post hoc hypotheses are presented as prior,
  selection is biased, constructs are unobservable, confounders are uncontrolled,
  or stopping is discretionary.

**Sources of ambiguity**

- “Investigation design” is named only as scope. No design taxonomy, selection rule,
  protocol contents, or stage-completion test exists.

**Opportunities for standardization**

- A protocol contract, design-choice record, validity-threat vocabulary, and
  amendment classification.

**Current determination:** Underspecified; independent researchers could reasonably
choose incompatible designs without recording why.

### 3. Evidence Plan

**Required inputs**

- Protocol, claims or hypotheses, constructs, analysis plan, known evidence sources,
  access constraints, and validity threats.

**Required outputs**

- A claim-to-evidence plan that states, for every prospective claim, the required
  observations, source classes, quality thresholds, triangulation needs, negative
  evidence, provenance, retention, and expected analysis.

**Decision rules**

- Admissibility and exclusion rules; evidence hierarchy; independence and
  corroboration tests; freshness and coverage thresholds; treatment of missing,
  contradictory, censored, or duplicated evidence; and a stopping rule.

**Required artifacts**

- Claim–evidence matrix; source register; search or discovery protocol; inclusion and
  exclusion log; provenance requirements; evidence gap and risk register.

**Failure modes**

- Cherry-picking, circular support, source dependence mistaken for corroboration,
  survivorship bias, unbounded collection, or evidence collected without a claim
  relationship.

**Sources of ambiguity**

- “Evidence planning” and “evidence” have no normative definition. There is no rule
  for sufficiency, source quality, contradictory evidence, or negative results.

**Opportunities for standardization**

- Evidence-item and source contracts, a claim–evidence relation vocabulary,
  admissibility criteria, and a reusable evidence-plan structure.

**Current determination:** Underspecified; neither evidence sufficiency nor evidence
provenance can be assessed consistently.

### 4. Instrument Selection

**Required inputs**

- Evidence plan, target constructs and observables, required accuracy and resolution,
  operating context, candidate instruments, resource constraints, and known threats.

**Required outputs**

- Selected instrument and exact version or configuration, selection rationale,
  measurement model, operational definitions, fitness-for-purpose evidence,
  limitations, and planned calibration.

**Decision rules**

- Minimum validity, reliability, sensitivity, specificity, precision, resolution,
  interoperability, and independence thresholds as applicable; tie-breaking and
  substitution rules; and criteria for rejecting an instrument.

**Required artifacts**

- Instrument specification; candidate comparison record; configuration manifest;
  operationalization map; validation record; license or access record; known-limit
  register.

**Failure modes**

- Instrument measures a proxy not the construct, version drift, undocumented
  defaults, observer effects, insufficient resolution, inaccessible proprietary
  dependencies, or selection based solely on convenience.

**Sources of ambiguity**

- “Scientific instrument interfaces” are in scope, but instrument, interface, and
  fitness for purpose are undefined. Human protocols, questionnaires, datasets, and
  software analyzers may or may not count as instruments.

**Opportunities for standardization**

- A general instrument contract, selection record, version/configuration identity,
  operationalization relation, and minimum fitness statement.

**Current determination:** Underspecified; instrument choice and equivalence rely on
author judgment.

### 5. Evidence Collection

**Required inputs**

- Approved protocol and evidence plan, selected and qualified instruments, sampling
  frame, collection environment, authorization, and calibration status.

**Required outputs**

- Immutable or content-addressed raw observations plus metadata, provenance, custody,
  timestamps, collection conditions, exclusions, anomalies, and deviations.

**Decision rules**

- Collection order and randomization; retry and duplicate policy; handling of
  missing, malformed, contaminated, or outlying observations; blinding; redaction;
  quality-control thresholds; and conditions for halting or resuming collection.

**Required artifacts**

- Collection procedure; environment and dependency manifest; sampling and execution
  log; raw evidence; provenance and chain-of-custody record; exclusion, anomaly, and
  deviation logs; integrity checksums; data dictionary.

**Failure modes**

- Irrecoverable provenance, silent transformation of raw data, inconsistent
  environments, noncomparable observations, selective retries, privacy breach,
  instrument failure, or loss of negative observations.

**Sources of ambiguity**

- No collection procedure or raw-versus-derived evidence boundary is defined. The
  non-scope of “research execution” does not identify what an executing repository
  must record to conform.

**Opportunities for standardization**

- A collection-run contract, provenance vocabulary, raw-evidence preservation rule,
  deviation taxonomy, and minimum environment manifest.

**Current determination:** Underspecified; a collection cannot be audited or replayed
from repository guidance.

### 6. Calibration

**Required inputs**

- Instrument identity and configuration, measurement model, reference standards or
  benchmark cases, required tolerance, environmental conditions, and prior
  calibration history.

**Required outputs**

- Calibration record linking instrument, reference, procedure, observations,
  uncertainty, acceptance result, validity interval, and any correction applied.

**Decision rules**

- Reference eligibility and traceability; accuracy/tolerance thresholds; number and
  ordering of trials; drift detection; recalibration triggers; treatment of failed
  calibration; and propagation of uncertainty into findings.

**Required artifacts**

- Calibration protocol; reference specification and provenance; raw calibration
  observations; calculations; calibration certificate or result; drift history;
  invalidation and recalibration log.

**Failure modes**

- Circular calibration, an unsuitable or changed reference, overfitting to benchmark
  cases, expired calibration, hidden correction, unreported uncertainty, or evidence
  gathered while the instrument is out of tolerance.

**Sources of ambiguity**

- “Model calibration” is in scope, while the process diagram says “Calibration.” It
  is unclear whether calibration applies to models, instruments, researchers,
  procedures, or all of these, and whether tuning and validation data must be
  separated.

**Opportunities for standardization**

- Separate definitions for calibration, tuning, validation, and qualification; a
  calibration record; reference hierarchy; tolerance rule; and validity interval.

**Current determination:** Underspecified; calibration scope, pass criteria, and the
effect of failure are absent.

### 7. Research Findings

**Required inputs**

- Protocol, complete evidence set, analysis plan, calibrated instrument records,
  deviations, exclusions, assumptions, and uncertainty estimates.

**Required outputs**

- Versioned findings in which each claim has scope, status, supporting and
  contradicting evidence, analysis, uncertainty, limitations, and a traceable path
  to the protocol and observations.

**Decision rules**

- Analysis execution and transformation rules; claim-support thresholds; distinction
  among observation, interpretation, inference, hypothesis, and conclusion;
  multiplicity and sensitivity treatment; handling of null and contradictory
  results; and criteria for revising or retracting a finding.

**Required artifacts**

- Analysis record; derived-data lineage; claim register; claim–evidence graph or
  matrix; uncertainty and sensitivity records; limitations and deviations statement;
  negative and null findings; review record.

**Failure modes**

- Untraceable claims, analytical flexibility, selective reporting, causal language
  unsupported by design, lost uncertainty, conflation of observation and inference,
  or findings that exceed the sampled scope.

**Sources of ambiguity**

- “Knowledge progression” is named but has no defined states or transition rules.
  There is no finding schema or evidentiary threshold.

**Opportunities for standardization**

- Typed claim statuses, explicit claim–evidence relations, standard uncertainty and
  limitation statements, and a finding revision/retraction procedure.

**Current determination:** Underspecified; findings cannot be reconstructed from a
defined evidence trail.

### 8. Replication

**Required inputs**

- Frozen protocol and amendments, complete artifact inventory, raw evidence,
  instruments and configurations, calibration records, analysis procedure,
  environment, and original findings.

**Required outputs**

- A replication package and independent replication report stating replication type,
  deviations, environment, artifact verification, results, comparison criteria,
  discrepancies, and disposition.

**Decision rules**

- Distinguish computational reproduction, direct replication, and conceptual
  replication; define who is sufficiently independent; specify allowable
  substitutions; define equivalence tolerances and success, partial success,
  inconclusive, and failure; and prescribe discrepancy resolution.

**Required artifacts**

- Artifact manifest with stable identifiers and checksums; replay instructions;
  dependency and environment specification; independent run log; comparison record;
  discrepancy log; replication report.

**Failure modes**

- Missing or mutable inputs, unavailable instruments, undocumented manual steps,
  environment drift, circular “replication” by the original investigator, undefined
  equivalence, or suppression of failed replication.

**Sources of ambiguity**

- “Replication strategy” is in scope but replication is not defined. The required
  independence, replay boundary, acceptable variance, and response to discrepancy
  are unknown.

**Opportunities for standardization**

- A replication taxonomy, package manifest, independence declaration, equivalence
  rule, and discrepancy workflow.

**Current determination:** Underspecified; no artifact set or criterion establishes
whether replication occurred.

### 9. Publication

**Required inputs**

- Reviewed findings, protocol and amendments, full artifact inventory, replication
  status, authorship contributions, conflicts, ethical/privacy constraints, and
  release approvals.

**Required outputs**

- A versioned publication with stable identity, methods and limitations, complete
  artifact references, availability exceptions, contributor and conflict statements,
  replication status, review status, license, and correction/retraction channel.

**Decision rules**

- Readiness and minimum disclosure criteria; authorship and contributor rules;
  redaction and justified non-release; versioning; embargo; peer-review status;
  correction, retraction, and supersession; and preservation period.

**Required artifacts**

- Publication-readiness checklist; manuscript or report; public artifact manifest;
  availability and redaction statement; contributor/conflict declarations; review
  record; release record; version, correction, and retraction history.

**Failure modes**

- Methods insufficient to reconstruct the work, broken artifact links, unpublished
  exclusions or deviations, privacy or licensing violations, ambiguous versions,
  inaccessible evidence, or no correction path.

**Sources of ambiguity**

- Publication is not included in current scope or non-scope and has no stated owner.
  No disclosure, preservation, versioning, or correction requirements are defined.

**Opportunities for standardization**

- A minimum disclosure standard, artifact availability statement, persistent identity
  rule, contributor taxonomy, and correction/retraction procedure.

**Current determination:** Underspecified and ownership-ambiguous.

## Cross-stage controls required for reproducibility

Stage-local descriptions alone are insufficient. A complete methodology also needs:

- **Identity and versioning:** stable identifiers for requests, protocols, runs,
  evidence, instruments, findings, replications, and publications.
- **Traceability:** explicit, typed links from request to question, design, planned
  evidence, collected evidence, analysis, claim, replication, and publication.
- **Change control:** immutable versions, materiality criteria, amendment rationale,
  approval, effective time, and impact analysis.
- **Roles and independence:** accountable owner, executor, reviewer, custodian, and
  replicator, including permitted role combinations and conflict declarations.
- **Stage gates:** entry, exit, rejection, rollback, and reopening criteria.
- **Deviations and exceptions:** a shared classification, recording rule, authority,
  and downstream impact assessment.
- **Provenance and integrity:** origin, custody, transformations, environment,
  timestamps, and integrity verification.
- **Uncertainty and assumptions:** persistent registers linked to affected decisions
  and claims, rather than prose added only at publication.
- **Ethics, privacy, security, and legal constraints:** review and handling rules that
  apply throughout the lifecycle, with justified access limitations.
- **Preservation:** retention periods, durable formats, dependency capture, access
  conditions, and planned handling of unavailable external resources.

None of these controls is currently specified.

## Answers to the audit questions

### 1. Which stages are underspecified?

All nine stages are underspecified. The README names several middle-stage concerns,
but none meets the audit completion rule. Research Request and Publication are not
even clearly included in the current scope. Evidence Collection has an unresolved
ownership tension with the non-scope of execution. Calibration is terminologically
inconsistent with “model calibration.” Replication is named without a type or success
criterion.

This does not mean every future investigation must use identical methods. It means
the methodology must define how contextual choices are bounded, justified, recorded,
reviewed, and propagated.

### 2. Which concepts should become first-class methodology objects?

A first-class methodology object has a stable identity, defined minimum contents,
version, provenance, lifecycle state, and explicit relations to other objects. The
minimum set is:

1. **Research Request** — question, scope, constraints, definitions, and disposition.
2. **Investigation Protocol** — design commitments and amendment history.
3. **Decision Record** — alternatives, rule applied, rationale, authority, and time.
4. **Assumption** — statement, justification, scope, owner, testability, and status.
5. **Validity Threat** — affected inference, mitigation, residual risk, and status.
6. **Claim** — type, scope, status, uncertainty, and evidentiary relations.
7. **Evidence Requirement** — observation needed, admissibility, quality threshold,
   and claim relation.
8. **Evidence Item** — immutable observation or source with provenance and integrity.
9. **Instrument** — identity, version/configuration, measurement role, limitations,
   and qualification status.
10. **Calibration Record** — reference, procedure, result, tolerance, uncertainty, and
    validity interval.
11. **Collection Run** — protocol version, environment, operator, inputs, outputs,
    anomalies, and deviations.
12. **Transformation/Analysis Record** — input lineage, procedure, parameters,
    environment, output, and verification.
13. **Deviation** — planned behavior, actual behavior, cause, authorization, and
    impact.
14. **Finding** — claim set, analysis, evidence links, limitations, and review state.
15. **Replication Attempt** — type, independence, substitutions, comparison rule,
    result, and discrepancies.
16. **Publication Record** — released version, disclosed artifacts, availability,
    review, correction, and supersession state.

The object definitions should be normative, while individual object instances belong
to the repository conducting the investigation.

### 3. Which artifacts are missing?

At minimum, the methodology lacks:

- a normative lifecycle and glossary;
- a research-request contract and intake gate;
- an investigation-protocol specification and amendment log;
- a claim–evidence matrix and evidence-admissibility specification;
- instrument selection, specification, and qualification records;
- a collection procedure, run log, data dictionary, and provenance record;
- a calibration protocol and calibration record;
- an analysis record, claim register, and finding report specification;
- a replication package manifest, run report, and discrepancy record;
- a publication-readiness and minimum-disclosure standard;
- cross-stage role, decision, assumption, threat, deviation, and change records; and
- an end-to-end traceability and artifact-retention specification.

### 4. Which responsibilities belong in Research Methodology?

This repository should own the reusable **normative contracts**:

- lifecycle vocabulary, stage ordering constraints, and stage gates;
- minimum inputs, outputs, artifacts, metadata, and completion criteria;
- definitions and lifecycle rules for the first-class objects above;
- rules for evidence admissibility, provenance, traceability, change, deviation,
  calibration, uncertainty, independence, replication, and disclosure;
- required decision records when domain judgment cannot be eliminated; and
- conformance criteria by which an investigation can claim to follow the methodology.

Downstream investigation repositories should own the **instances and executions**:

- the specific request, protocol, domain definitions, hypotheses, samples, and cases;
- collected observations and domain evidence;
- selected instrument instances and their configurations;
- run-specific calibration, collection, analysis, and deviation records;
- findings, replication attempts, and publications; and
- domain-specific extensions that do not weaken the general contracts.

Formal theory, deterministic analysis engines, and operational legitimacy decisions
remain in their stated repositories. Their outputs may serve as evidence or
instruments, but they do not define this methodology's general conformance rules.

### 5. What is the next smallest addition that most increases reproducibility?

Add one normative **Investigation Protocol specification** with a stable identifier
and version, required before evidence collection. It should require, in one bounded
record:

1. the accepted research request and precisely bounded questions;
2. definitions, units of analysis, scope, exclusions, assumptions, and validity
   threats;
3. chosen design and the recorded rationale for material choices;
4. claims or hypotheses and a claim-to-evidence plan;
5. case/sample selection, instrument selection, calibration, collection, analysis,
   and stopping rules;
6. required artifacts, provenance, environment, roles, and preservation;
7. treatment of missing, contradictory, excluded, and negative evidence;
8. uncertainty, replication type, independence, and comparison criteria;
9. publication and minimum-disclosure commitments; and
10. approval, amendment, deviation, and version history.

This is the smallest high-leverage addition because it creates an inspectable
pre-commitment spanning every stage without conducting research or prescribing a
domain-specific design. It converts hidden author judgment into declared choices and
provides the anchor for traceability. A blank template alone is insufficient: the
specification must define required semantics, completion criteria, and how “not
applicable” is justified.

## Residual risk and audit limit

This audit improves methodological transparency by making gaps and ownership
boundaries explicit; it does not itself fill those gaps. Reproducibility remains
blocked until normative contracts and decision rules are adopted. Because no study,
downstream repository, issue, or pull-request material is present in this repository,
the audit makes no claim about undocumented practices elsewhere.

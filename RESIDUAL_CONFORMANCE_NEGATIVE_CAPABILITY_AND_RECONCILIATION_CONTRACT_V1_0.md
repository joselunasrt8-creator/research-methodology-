# Residual Conformance, Negative Capability, and Reconciliation Contract v1.0

**Canonical status:** Residual methodology contract v1.0

**Issue:** #9 — Define Residual Conformance, Negative Capability, and Reconciliation Contracts

**Boundary:** definition only; no execution, registry implementation, synchronization, repair, mutation, scientific determination, or execution authorization

## 1. Purpose and relationship to existing canon

This document is the single canonical source for the repository's residual methodology-conformance outcomes, negative-capability rules, interaction distinctions, and cross-registry reconciliation contract.

It extends, but does not restate or supersede, the repository boundary, execution binding, provenance, versioning, calibration, deviation, stopping, and historical-preservation rules in [Methodology Engineering Canon](METHODOLOGY_ENGINEERING_CANON.md). Those rules remain authoritative for their subjects.

The frozen Cross-Domain Structology Transfer Audit v0.1 and its frozen conformance review are historical reference surfaces. This contract does not modify them, reinterpret their outcomes, resolve their recorded drift, or replace the Issue #33 review vocabulary.

## 2. Scope

This contract defines only:

- a generic methodology-conformance outcome model;
- the capabilities a repository or methodology may and may not claim;
- ownership-status and interaction vocabularies;
- the evidence boundary for external ownership and authority claims; and
- a non-mutating cross-registry reconciliation record, discrepancy vocabulary, outcome model, and follow-up boundary.

Every determination under this contract is bounded to the identified object, version, criteria, evidence, and comparison scope recorded for that determination.

## 3. Methodology conformance outcome model

### 3.1 Common determination rules

A methodology-conformance determination must identify the assessed object and immutable version, the governing methodology or criteria and version, the assessment scope, the evidence considered, material missing evidence, limitations, and exactly one outcome from this section. Existing canon supplies the provenance, execution-binding, deviation, and historical-preservation obligations; this contract does not replace them.

Outcome precedence is:

1. Use `NOT_APPLICABLE` only when an applicability rule affirmatively excludes the object or criterion.
2. Use `BLOCKED` when an identified unmet prerequisite prevents the required assessment from being completed.
3. Use `INDETERMINATE` when assessment can be performed but the available evidence cannot support one defensible conformance result.
4. Use `NONCONFORMING` when sufficient evidence establishes failure of one or more mandatory criteria.
5. Use `CONFORMING_WITH_LIMITATIONS` when every applicable mandatory criterion is satisfied but material interpretation or applicability limits prevent an unqualified determination.
6. Use `CONFORMING` only when every applicable mandatory criterion is satisfied and no material limitation qualifies the determination.

Absence of a detected defect is not evidence of conformance. Missing evidence is not evidence of nonconformance. A limitation must not be used to conceal failure of a mandatory criterion.

```text
Conformance
        ≠
Scientific Truth
        ≠
Execution Permission
```

A conformance outcome describes satisfaction of a declared contract within a recorded scope. It does not establish empirical truth, scientific warrant, fitness outside that scope, acceptance of a claim, or permission to execute or mutate anything.

### 3.2 `CONFORMING`

- **Required evidence:** Complete, admissible evidence for every applicable mandatory criterion, with the assessed object and governing criteria bound to exact versions; evidence that applicability and material limitations were reviewed.
- **Decision criteria:** Every applicable mandatory criterion is satisfied and no material evidence gap, contradiction, unresolved deviation, or interpretation limitation remains.
- **Permitted interpretation:** The identified object conforms to the identified criteria and versions within the recorded scope.
- **Prohibited interpretation:** The object is scientifically true, universally valid, approved, safe, authorized for execution, or conforming to any unassessed version or scope.
- **Continuation rules:** Conformance-dependent review may continue only when the governing workflow and a separately established authority permit it. The outcome itself grants no continuation or execution authority.
- **Supersession behavior:** A later determination may supersede this outcome only by identifying this record and the changed object, criteria, evidence, or scope. This determination remains valid historical evidence for its original bound state.

### 3.3 `CONFORMING_WITH_LIMITATIONS`

- **Required evidence:** Evidence sufficient to satisfy every applicable mandatory criterion, plus an explicit limitation record identifying the restricted scope, affected interpretations, cause, and carry-forward requirement.
- **Decision criteria:** No mandatory criterion fails, but one or more material limitations restrict applicability, confidence, completeness, transfer, or interpretation.
- **Permitted interpretation:** The object conforms only within the stated boundary and while every recorded limitation is preserved.
- **Prohibited interpretation:** Unqualified conformance; conformance outside the limited scope; waiver of a mandatory criterion; permission to discard or silently resolve a limitation.
- **Continuation rules:** Conformance-dependent review may continue only inside the limited scope, with limitations carried into every dependent record, and only under separately established workflow and authority rules.
- **Supersession behavior:** A later determination may remove a limitation only by citing new evidence that resolves it. Unresolved limitations survive into successor determinations and the original record remains historical evidence.

### 3.4 `NONCONFORMING`

- **Required evidence:** Admissible evidence that identifies each failed mandatory criterion, the assessed object and version, the observed state, and the decision rule establishing failure.
- **Decision criteria:** At least one applicable mandatory criterion is demonstrably unsatisfied. Sufficient evidence exists to distinguish failure from missing evidence or ambiguity.
- **Permitted interpretation:** The identified object does not satisfy the identified contract within the recorded scope.
- **Prohibited interpretation:** The object is scientifically false, worthless, unauthorized in every context, automatically rejected, or already repaired; absence of evidence alone is nonconformance.
- **Continuation rules:** No claim of conformance may continue. The record may support a bounded proposal, correction request, or escalation, but never automatic mutation. Any further use requires an independently recorded rule and authority that explicitly permits nonconforming continuation.
- **Supersession behavior:** A later determination may supersede this outcome only against a changed or corrected object, new version, or materially changed evidence and must cite the failed criteria and their disposition. The nonconforming history is preserved.

### 3.5 `BLOCKED`

- **Required evidence:** Evidence identifying the unmet prerequisite, why it is required, what assessment activity it prevents, the responsible external dependency or boundary when known, and the condition required to unblock it.
- **Decision criteria:** A required assessment step cannot be completed because evidence, access, authority, a required dependency, or another explicit prerequisite is unavailable. The blocker is identifiable; the underlying conformance result is not.
- **Permitted interpretation:** The conformance assessment cannot presently reach a defensible result for the blocked scope.
- **Prohibited interpretation:** The object conforms or does not conform; the blocker is a defect in the assessed object unless separately evidenced; urgency permits bypassing the prerequisite.
- **Continuation rules:** Pause work that depends on the missing determination. Evidence collection, access requests, clarification, bounded proposals, and escalation may continue; execution or mutation does not become permitted.
- **Supersession behavior:** A successor determination must identify the blocker disposition and the evidence or authority that removed it. If the blocker persists, a new record may update status without erasing the earlier blocked record.

### 3.6 `INDETERMINATE`

- **Required evidence:** The available evidence set, the competing or unsupported interpretations, the ambiguity or contradiction preventing a unique result, and the additional evidence or rule clarification that could resolve it when known.
- **Decision criteria:** The assessment was possible, but admissible evidence is ambiguous, contradictory, insufficiently discriminating, or unable to support exactly one of `CONFORMING`, `CONFORMING_WITH_LIMITATIONS`, or `NONCONFORMING`.
- **Permitted interpretation:** No defensible conformance result can be selected from the current evidence within the recorded scope.
- **Prohibited interpretation:** Conformance by default, nonconformance by suspicion, permission to choose the convenient interpretation, or equivalence to a known external blocker.
- **Continuation rules:** Do not make a conformance-dependent claim. Clarification, additional evidence collection, scope refinement, proposal, or escalation may continue without mutation or execution authorization.
- **Supersession behavior:** A successor must cite the resolved ambiguity, contradiction, or evidentiary gap. Narrowing scope may supersede only the newly bounded portion; unresolved portions remain indeterminate.

### 3.7 `NOT_APPLICABLE`

- **Required evidence:** The governing applicability rule, the object attributes or scope facts to which it was applied, and the rationale showing why the criterion or assessment does not apply.
- **Decision criteria:** An explicit rule affirmatively excludes the object or criterion from the assessment scope. Inapplicability is established rather than inferred from missing evidence or effort.
- **Permitted interpretation:** No conformance determination is required for the explicitly excluded object or criterion in the recorded scope.
- **Prohibited interpretation:** The criterion was satisfied, waived, ignored, or blocked; the object is exempt outside the recorded rule and scope.
- **Continuation rules:** Only the inapplicable criterion or object may be skipped. All other applicable criteria and independent authority gates remain in force.
- **Supersession behavior:** A later determination may replace this outcome only when the applicability rule, object, version, or scope changes. The original inapplicability determination remains historical evidence.

## 4. Negative capability contract

Negative capability is the explicit boundary between what a repository or methodology can represent and what it has authority to decide, authorize, execute, or claim. A methodology may define rules for an activity without performing that activity. A repository may hold an artifact without owning the decisions or authority associated with it.

### 4.1 Permitted capabilities

Subject to the existing repository boundary, a repository or methodology may:

| Capability | Bounded meaning |
| --- | --- |
| Own | Define and govern an in-scope methodology object or contract when canonical boundary evidence assigns that responsibility. |
| Reference | Identify and interpret an external object through a stable citation without acquiring custody, decision rights, or authority over it. |
| Consume | Accept an artifact as a declared input under admissibility and provenance rules without acquiring ownership of the source object or source decision. |
| Produce | Create an in-scope artifact or proposed output while preserving its provenance, limitations, and downstream authority boundary. Production does not establish acceptance. |
| Propose | Form and transfer a reviewable recommendation, candidate change, reconciliation action, or escalation for disposition by the decision owner. |

These capabilities are object- and scope-specific. One permitted capability does not imply another.

### 4.2 Prohibited capabilities

Unless a separate, evidenced authority contract explicitly assigns the capability, a repository or methodology may not:

| Prohibited capability | Rule |
| --- | --- |
| Decide | Make a concrete acceptance, rejection, prioritization, scientific, policy, or external ownership decision merely because it defines criteria, produces evidence, or owns a proposal. |
| Authorize | Grant execution, mutation, repair, publication, advancement, or authority transfer merely from conformance, artifact custody, reconciliation, or proposal status. |
| Execute | Treat a methodology definition, procedure, dependency description, or proposed follow-up as the execution event itself. |
| Claim without evidence | Assert conformance, ownership, external ownership, authority, reconciliation, scientific truth, completion, or permission without the evidence required by the applicable contract. |

When authority is not explicitly and immutably evidenced, the contract fails closed: no authority is inferred from repository location, authorship, artifact movement, operational need, or prior practice.

### 4.3 Ownership statuses

An ownership status is assigned relative to an identified repository or methodology, object, version, and scope. The status describes the bounded relationship; it does not transfer authority. Record one status for each claim being evaluated rather than collapsing different objects or scopes into one assertion.

| Status | Required meaning |
| --- | --- |
| `OWNED` | Canonical in-scope evidence assigns the repository or methodology responsibility to define or govern the identified object. |
| `REFERENCED` | The object remains elsewhere and is used only through a stable reference. No custody, decision right, or authority is acquired. |
| `CONSUMED` | The object is accepted as an input. Consumption does not transfer source ownership, decision ownership, or authority. |
| `PRODUCED` | The repository or methodology creates the identified output. Production does not imply acceptance, external ownership, or authority over downstream use. |
| `PROPOSED` | The object is a recommendation or candidate disposition awaiting action by an identified decision owner. The proposer owns the proposal record, not the decision. |
| `EXTERNALLY_OWNED` | Immutable evidence identifies a specific external owner, object, version or effective boundary, and ownership scope. |
| `UNRESOLVED` | Required evidence cannot establish one of the other applicable statuses. No ownership or authority may be inferred while unresolved. |
| `OUT_OF_SCOPE` | An explicit boundary rule excludes the object or ownership question from this repository or methodology. This does not identify who owns it. |

`OUT_OF_SCOPE` must not be converted to `EXTERNALLY_OWNED` without evidence. `PRODUCED` must not be converted to `OWNED` merely because the artifact is stored locally. `REFERENCED` or `CONSUMED` must not be interpreted as transferred custody or authority.

### 4.4 Immutable evidence for external ownership

Every `EXTERNALLY_OWNED` claim requires an immutable evidence reference that identifies:

- the external owner;
- the owned object and stable identity;
- the ownership scope and effective version or time boundary;
- the issuing source with authority to make the assignment; and
- an immutable locator, such as a commit identifier, content digest, signed record, immutable release, or versioned registry record.

A mutable branch, unversioned document, repository name, artifact location, oral convention, or inference from current behavior is insufficient by itself. If any required evidence is missing, inaccessible, contradictory, or not immutable, the status must be `UNRESOLVED`. The repository may propose clarification or escalate the missing claim; it may not supply the missing external decision itself.

## 5. Interaction distinctions

Every material cross-boundary interaction must be classified by its actual dependency or transfer type. More than one type may apply, but each must be recorded separately; none may be inferred from another.

| Interaction | Canonical distinction |
| --- | --- |
| Reference Dependency | Interpretation or conformance depends on an identified external definition, contract, or artifact. The reference must resolve for review, but no live external component is required during execution. |
| Artifact Exchange | A bounded artifact is delivered, received, or made available across a repository or organizational boundary. Custody of the copy changes as recorded; ownership, decision rights, authority, and execution permission do not. |
| Runtime Dependency | A live execution requires an external service, component, interface, or resource to be available and behave under a declared runtime contract. A documentation reference alone is not a runtime dependency. |
| Proposal Transfer | A proposal is delivered to a decision owner for review. The transfer preserves proposer identity, evidence, scope, limitations, and requested disposition; it does not make the proposal a decision. |
| Decision Transfer | An authorized decision record is conveyed for bounded reliance or implementation. The transfer preserves the original decision owner, scope, effective conditions, and supersession status; it does not give the recipient power to alter the decision or make new decisions. |
| Authority Transfer | An evidenced delegation or reassignment gives an identified recipient specified decision or action authority. It requires immutable evidence of the source authority, recipient, scope, effective boundary, conditions, and revocation or supersession behavior. Without that evidence, authority remains unresolved and no transfer occurs. |
| Execution Dependency | A planned execution or stage depends on completion or a qualifying result of another identified execution, stage, or external action. It may be asynchronous and artifact-mediated; unlike a runtime dependency, it does not necessarily require a live component during operation. |

Proposal ownership is responsibility for the proposal's content, provenance, and limitations. Decision ownership is the evidenced responsibility and authority to accept, reject, defer, or otherwise dispose of that proposal. Transferring the proposal does not transfer the decision.

The following invariants are mandatory:

```text
Artifact Exchange ≠ Authority Transfer
Reference Dependency ≠ Runtime Dependency
Proposal Ownership ≠ Decision Ownership
Conformance ≠ Scientific Truth ≠ Execution Permission
```

In addition, decision transfer is not authority transfer, execution dependency is not execution permission, and possession is not ownership.

## 6. Cross-registry reconciliation contract

### 6.1 Purpose and invariant

Cross-registry reconciliation is a documented comparison of identified registry states under declared rules. It determines only whether the compared objects can be reconciled within the recorded versions, evidence, and authority boundary.

```text
Observed discrepancy
        ↓
Reconciliation record
        ↓
Bounded determination
        ↓
Proposal or escalation

Never automatic mutation
```

```text
Reconciliation Evidence ≠ Repair Authority
```

A reconciliation record may describe a proposed repair, but it may not apply one, synchronize a registry, advance a lifecycle, rewrite history, transfer authority, or authorize execution.

### 6.2 Reconciliation record

Every cross-registry reconciliation must produce one durable record containing:

| Field | Required content |
| --- | --- |
| Identity | Stable reconciliation-record identity and record status. |
| Compared registries | Stable identities and bounded roles of every registry included in the comparison. |
| Versions | Immutable registry snapshots, revisions, releases, digests, or equivalent version evidence actually compared. |
| Compared objects | Stable identities, object types, and scoped attributes or relationships compared in each registry. |
| Comparison rules | Declared equivalence, identity, version, boundary, completeness, precedence, and materiality rules used for the comparison. |
| Provenance | References required by the existing canon to trace registry versions, compared objects, evidence, and the creation of this record. |
| Discrepancy classifications | Every observed discrepancy classified using section 6.3, with affected objects and materiality. |
| Missing evidence | Required evidence that is absent, inaccessible, mutable, contradictory, or insufficient, and its effect on the determination. |
| Limitations | Scope, access, temporal, semantic, evidence, and interpretation boundaries on the comparison. |
| Determination | Exactly one reconciliation outcome from section 6.4, with its rule trace and bounded rationale. |
| Follow-up | `NONE`, a bounded proposal, or an escalation; the target decision owner or unresolved owner; required evidence; and stopping condition. |
| Authority boundary | What the reconciler may record, compare, determine, propose, or escalate, and explicit prohibitions on deciding external ownership, repair, mutation, synchronization, advancement, or execution. |
| Supersession history | Prior and successor reconciliation-record references, reason for replacement, effective boundary, and preservation of every earlier record. |

The record compares exact registry states. A later registry version requires a new reconciliation record and does not change the determination made against an earlier state.

### 6.3 Discrepancy classifications

Each observed discrepancy receives one or more of the following classifications. Multiple classifications are permitted when they describe distinct aspects of the same discrepancy.

| Classification | Meaning |
| --- | --- |
| `DRIFT` | Corresponding objects or attributes have diverged from a declared common or expected state without an evidenced intentional replacement that resolves the difference. |
| `ORPHANED_OBJECT` | An object exists in one registry but its required counterpart, owner, parent, source, or governing relationship cannot be resolved in the compared registry set. |
| `CONTRADICTION` | Registries make materially incompatible assertions about the same identified object, relationship, state, or rule. |
| `STALE_REFERENCE` | A reference resolves to a superseded, withdrawn, expired, or no-longer-current target when the comparison rule requires a current target. |
| `MISSING_EVIDENCE` | Evidence required to compare, classify, or determine the object is absent, inaccessible, mutable when immutability is required, or insufficient. |
| `IDENTITY_MISMATCH` | Objects asserted or expected to correspond have incompatible stable identities, or identity equivalence cannot be established under the comparison rule. |
| `VERSION_MISMATCH` | Compared objects or registries use incompatible, unexpected, or non-equivalent versions under the declared version rule. |
| `BOUNDARY_MISMATCH` | Registries assign incompatible scope, repository, lifecycle, ownership, authority, inclusion, or exclusion boundaries to the compared object. |
| `BLOCKED` | An identified access, dependency, authority, or evidence prerequisite prevents the discrepancy from being fully assessed. This classification does not determine the overall outcome by itself. |
| `UNRESOLVED_EXTERNAL_OWNERSHIP` | A required external ownership claim lacks the immutable evidence required by section 4.4 or contains conflicting ownership evidence. The ownership status is `UNRESOLVED`. |

Classification records observation; it does not authorize correction. Materiality and outcome are determined under the recorded comparison rules rather than inferred solely from a class name.

### 6.4 Reconciliation outcomes

- **`RECONCILED`:** Complete required evidence shows that all compared objects satisfy the comparison rules and no material discrepancy or limitation remains. This means the exact compared states reconcile; it does not mean they are correct, current beyond those versions, or authorized for mutation or execution.
- **`RECONCILED_WITH_LIMITATIONS`:** Evidence supports bounded reconciliation, but recorded non-dispositive discrepancies, exclusions, or interpretation limits prevent an unqualified result. Every limitation must be carried into dependent use; no failed mandatory comparison rule may be relabeled as a limitation.
- **`NOT_RECONCILED`:** Sufficient evidence establishes at least one material failure of the comparison rules. The outcome supports a proposal or escalation only and does not select or apply a repair.
- **`BLOCKED`:** An identified unmet prerequisite prevents completion of the required comparison or determination. The record must name the unblock condition; no underlying reconciliation result may be inferred.
- **`INDETERMINATE`:** Comparison was possible, but ambiguity, contradiction, unresolved identity, insufficiently discriminating evidence, or unresolved external ownership prevents one defensible reconciled or not-reconciled result.
- **`NOT_APPLICABLE`:** An explicit comparison rule establishes that the registries or objects require no reconciliation in the recorded scope. Missing counterparts or evidence alone cannot establish this outcome.

Outcome precedence mirrors the conformance model: establish affirmative inapplicability first; otherwise record a known preventing prerequisite as `BLOCKED`, unresolved interpretation as `INDETERMINATE`, evidenced material failure as `NOT_RECONCILED`, bounded alignment as `RECONCILED_WITH_LIMITATIONS`, and complete alignment as `RECONCILED`.

### 6.5 Follow-up and authority boundary

The reconciler may observe, compare, classify, record a bounded outcome, preserve limitations, propose a disposition, and escalate to an evidenced decision owner. The reconciler may not infer external ownership, choose a repair owner, approve a proposal, mutate either registry, synchronize data, authorize execution, or advance an object merely because a discrepancy or outcome exists.

Required follow-up behavior is:

- `RECONCILED` may record `NONE` or a non-mutating monitoring proposal; it grants no advancement or execution permission.
- `RECONCILED_WITH_LIMITATIONS` must identify how limitations are carried forward and may propose evidence collection or clarification.
- `NOT_RECONCILED` must propose a bounded disposition or escalate the material discrepancy to the decision owner.
- `BLOCKED` must identify the unblock condition and responsible boundary when evidenced; otherwise ownership remains `UNRESOLVED`.
- `INDETERMINATE` must identify needed evidence, rule clarification, scope refinement, or escalation.
- `NOT_APPLICABLE` records the applicability basis and requires no reconciliation action for the excluded scope.

If a decision owner cannot be established with the required evidence, follow-up stops at proposal or escalation with ownership status `UNRESOLVED`.

## 7. Supersession and preservation

Conformance and reconciliation records are append-only determinations about bound states. A successor must cite the prior record, identify the changed object, version, criteria, rule, evidence, scope, limitation, or blocker, and state which portions it supersedes. It must not overwrite, relabel, or silently reinterpret the prior determination.

Supersession changes the current applicable determination only within the successor's explicit boundary. It does not retroactively authorize an action, repair a prior discrepancy, erase a limitation, or convert historical uncertainty into certainty.

## 8. Intentional exclusions

This contract does not implement or define:

- runtime behavior, registries, schemas, validators, synchronization, or automatic repair;
- execution permission or mutation authority;
- scientific correctness, empirical truth, or claim acceptance;
- a concrete conformance review or a replacement for Issue #33;
- new repository ownership, execution binding, provenance, versioning, calibration, or historical-preservation rules; or
- the residual contracts assigned to Issues #1, #3, #4, #5, #8, #10, #20, or #21.

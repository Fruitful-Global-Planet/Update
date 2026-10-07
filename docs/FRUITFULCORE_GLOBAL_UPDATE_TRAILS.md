# FruitfulCore Global Update Trails and Governance Threads

**Document status:** Draft for project conclusion and current-state review  
**Prepared for:** Fruitful-Global-Planet/Update  
**Proposed pull request title:** `docs: consolidate FruitfulCore global update trails and governance threads`  
**Scope:** FruitfulCore, Fruitful Portals, Heyns1000 QS Command Center, Fruitful Around Town, GitHub, Supabase, FruitfulApp/Base44, and workspace context  
**Operating doctrine:** Evidence first · append only · explicit authority · approval before projection  
**Classification:** Internal governance documentation — no credentials, customer data, live configuration, or production secrets

---

## 1. Project conclusion

FruitfulCore is the proposed evidence-led control plane for the Fruitful ecosystem. Its purpose is to connect operational evidence, versioned specifications, quantity-surveying controls, commerce records, governance decisions, and downstream projections without treating any one interface, chat session, repository, or application as automatically authoritative for all purposes.

The architecture is deliberately evidence-first:

- Original sources remain identifiable.
- New information is appended rather than silently overwriting prior records.
- Calculations, AI enrichments, reconciliations, and recommendations remain distinguishable from source evidence.
- Approval is a separate, named event.
- A dashboard, report, API response, or channel update is treated as a controlled projection, not as primary truth.

FruitfulCore is not yet demonstrated as a single deployed canonical system of record. The current estate remains distributed across workspace/session context, GitHub, Supabase, FruitfulApp/Base44, the Heyns1000 QS Command Center, Fruitful Portals, Fruitful Around Town, and related operational surfaces.

---

## 2. Unified position

FruitfulCore should operate as a common provenance, governance, and release layer across the ecosystem.

```text
Sources and working systems
        │
        ▼
FruitfulCore evidence, lineage, approval and release controls
        │
        ▼
Approved read-only or operational projections
```

The system must preserve the difference between:

1. A source or event.
2. A captured instruction or workflow trigger.
3. A preserved record.
4. A derived extension, calculation, interpretation, or reconciliation.
5. An authorised projection released for a defined purpose.

No source system should be assumed to be a full substitute for the others. GitHub provides versioned source and review history. Supabase can provide durable structured records. A QS workstream provides professional measurement and cost-control context. User interfaces provide controlled presentation. Workspace sessions provide captured working context. Each role has distinct evidential limits.

---

## 3. Waterfall evidence model

FruitfulCore adopts the append-only Waterfall Memory Flow:

```text
🦍 Origin
    ↓
💧 Captured prompt
    ↓
🌱 Preserved record
    ↓
🌿 Linked extension
    ↓
🌳 Approved projection
```

### 3.1 Stage definitions

| Stage | Meaning | Minimum control |
|---|---|---|
| 🦍 Origin | An identifiable source, event, person, system, document, commit, or site artefact | Source reference, type, actor/system, timestamp, evidence location |
| 💧 Captured prompt | The exact initiating instruction, request, event trigger, or workflow context | Prompt/event content, actor, channel, capture time |
| 🌱 Preserved record | A retained and versioned source/event payload | Record ID, version or object ID, hash where available, retention status |
| 🌿 Linked extension | An extraction, reconciliation, calculation, classification, interpretation, or correction | Parent links, method/version, evidence references, confidence state |
| 🌳 Approved projection | A controlled output made usable outside the ledger | Authority, approver, policy version, scope, approval time, release receipt |

### 3.2 Append-only rule

No new event overwrites an earlier event. A correction, conflict, revocation, or supersession is itself a new linked record.

```text
Original evidence
    ├── supports → extension
    ├── contradicts → exception record
    └── superseded_by → corrected record
                            └── projected_from → approved output
```

---

## 4. Authority boundaries

| Surface | Evidenced role | Must not be assumed |
|---|---|---|
| Supabase / Fruitful ledger | Intended durable operational records, approvals, audit and governed projections | That its current schema already contains the Waterfall Memory Ledger or a verified cross-system graph |
| GitHub | Versioned source, change, review and release evidence | Production state, deployed configuration, credentials, live data, or financial truth |
| Heyns1000 QS Command Center | QS evidence, BoQ/5D-BIM, procurement, site reconciliation and professional gates | That AI may issue certificates, instructions, or binding commercial actions without authorised professional approval |
| Fruitful Portals | Controlled presentation and integration candidates | Source authority, approval authority, or an automatically reconciled ledger |
| Fruitful Around Town | Candidate local-discovery and commerce projection channel | Inventory, identity, consent, finance, or governance authority |
| FruitfulApp/Base44 | Operational entity and workflow API candidate | Verified canonical ledger status until authenticated endpoint and retention controls are evidenced |
| Workspace/session context | Captured working context and research continuity | Durable external ledger, cryptographic hash graph, formal project mapping, or authorised release record |

---

## 5. First demonstrated trace

The first proof should use a harmless, non-secret GitHub specification file pinned to a full immutable commit SHA.

### 5.1 Selected source class

| Candidate source | Priority | Reason |
|---|---:|---|
| GitHub specification file | First | Stable repository identity, immutable commit SHA, reproducible retrieval, low sensitivity, no external business action |
| QS evidence record | Second | Requires contract context, measurement evidence, named QS authority, and explicit professional approval |
| Fruitful product/inventory record | Third | Requires ownership, identity, consent, pricing, stock, tax, finance, and channel-projection controls |

### 5.2 Trace path

```text
GitHub file at immutable commit SHA
    ↓
Evidence event
    ↓
Lineage edge
    ↓
Human approval event
    ↓
Read-only dashboard or API projection
    ↓
Immutable release receipt
```

### 5.3 Minimum evidence metadata

The initial GitHub evidence event must capture:

- Repository URL and repository identity.
- Branch used for capture.
- Full Git commit SHA.
- File path.
- Git blob SHA where available.
- SHA-256 computed from the exact retrieved file bytes.
- Capture time.
- Original author/committer metadata where available.
- Classification and sensitivity.
- Record owner and responsible reviewer.

The GitHub SHA and a SHA-256 content hash serve different purposes. The Git commit/blob identifiers establish Git provenance; the SHA-256 should be independently calculated from the exact preserved content.

---

## 6. Initial governance gates

### Evidence gate

Before preservation, the record must include source reference, actor or system, timestamp, content hash where applicable, classification, and sufficient context to reproduce the retrieval.

### Authority gate

Each record and intended action must identify a responsible owner and defined scope. Source capture does not itself confer approval authority.

### Approval gate

Finance, QS certification, deployments, publishing, external communications, and state-changing integrations require explicit human authorisation from the appropriate authority.

### Projection gate

No downstream display, report, portal update, API release, or operational instruction should be marked approved without a traceable path from source through preservation, extension, approval, and release receipt.

### Security gate

Raw credentials, bearer tokens, API keys, passwords, private keys, client secrets, `.env` content, customer data, payment data, and raw infrastructure configuration are excluded from evidence payloads. Any suspected exposure triggers immediate rotation, containment, and a safe incident record.

### Integrity gate

Hashes, immutable versions, or equivalent preservation receipts are recorded.

### Supersession gate

Corrections and revocations create append-only follow-on records rather than overwriting prior evidence.

---

## 7. Canonical ledger target

The proposed durable FruitfulCore ledger should provide four independently auditable record classes:

| Record class | Purpose |
|---|---|
| `memory_events` | Append-only origin, prompt, preserved-record, extension, and projection events |
| `memory_edges` | Typed parent and cross-record relationships |
| `memory_approvals` | Independent approval, rejection, revocation, and supersession records |
| `memory_release_receipts` | Evidence that an approved projection was released or consumed by a named destination |

Required relationship types should include:

```text
captured_from
preserved_as
extends
supports
contradicts
reconciles_with
supersedes
approved_from
projected_from
mapped_to_project
released_to
```

The ledger must be append-only in behaviour, protected by row-level security, denied public write access by default, and designed to retain correction and revocation evidence rather than erase history.

---

## 8. Security posture

This document does not contain secret values and must not be used to store them.

### Required rule

> Raw credentials are never evidence payloads. Preserve only a provider name, credential label, safe fingerprint or provider identifier, vault reference, scope, expiry, rotation status, and incident/remediation receipt.

If a credential appears in a repository, prompt, session title, chat, issue, log, screenshot, client-side application bundle, or documentation, treat it as compromised. Revoke/rotate it, update protected server-side bindings, search for other copies, and retain only remediation metadata.

Redaction reduces further spread but does not restore trust in an exposed value.

The initial GitHub trace must not interact with DNS, Workers, Pages, Cloudflare configuration, production databases, financial records, payment records, QS records, inventory records, or raw operational logs.

---

## 9. Current state

### Confirmed

- The target GitHub repository is `Fruitful-Global-Planet/Update`.
- Its baseline source is the `main` branch at an immutable commit SHA.
- GitHub can provide a low-risk first source for a read-only lineage demonstration.
- FruitfulCore has an agreed conceptual Waterfall Memory Flow and governance boundary.
- The broader ecosystem includes QS, portal, local-discovery, commerce, API, repository, and database workstreams that need explicit rather than inferred linkage.
- The Heyns1000 QS Command Center requires authorised professional approval for QS certification and binding commercial actions.
- Workspace sessions are useful captured context but are not automatically a durable external ledger.

### Not yet demonstrated

- A deployed, canonical Waterfall Memory Ledger.
- Formal cross-system lineage edges or hash chaining.
- A verified session-to-project or project-to-record mapping.
- A fully defined approval authority matrix.
- An approved external operational projection and immutable release receipt.
- A complete secure integration inventory across all operational surfaces.
- Cryptographic content integrity for all retained records.
- Verified cross-system synchronisation between GitHub, Supabase, FruitfulApp/Base44, Cloudflare, and workspace context.

---

## 10. Open tails

| Priority | Tail | Exact evidence needed |
|---|---|---|
| Critical | Durable ledger implementation | Approved migration receipt, schema verification, RLS posture, and controlled write evidence |
| Critical | Credential-exposure containment | Provider revocation receipt, replacement secret reference, deployment rebinding receipt, and audit-log review |
| High | Canonical lineage | Event IDs, typed edges, timestamps, hashes, parent references, and cross-system mappings |
| High | Approval model | Named authority matrix, policy versions, approval scope, revocation path, and audit requirements |
| High | Release control | Destination, projection ID, approval reference, release timestamp, result, and immutable receipt |
| Medium | QS integration | Contract, BoQ, valuation, procurement, and professional-approval mappings under the Honourable QS standard |
| Medium | Commerce and portal integration | Ownership, consent, pricing, tax, inventory, and customer-data controls before customer-facing projections |
| Medium | Repository controls | Secret scanning, documentation review, CI validation, contribution rules, and protected-branch policy |

---

## 11. Find-the-Tail register

| Priority | Open item | Evidence required |
|---|---|---|
| Critical | Canonical ledger is not yet deployed | Approved migration receipt and post-migration verification |
| Critical | Credential exposure containment may be incomplete | Revocation receipt, replacement-vault reference, deployment update proof, audit-log review |
| High | No formal source-to-ledger mapping | Stored source IDs, event IDs, typed edges, timestamps, and parent references |
| High | No verified approval matrix | Named authority matrix for QS, finance, security, publishing, code, and deployment |
| High | No cryptographic integrity baseline | SHA-256 policy, canonicalisation method, immutable object/version reference, preservation receipt |
| High | No verified release-receipt process | Destination, approval ID, event ID, release result, timestamp, and version reference |
| Medium | GitHub repository documentation remains minimal | Versioned architecture, migration source, schema contract, ownership, and CI validation |
| Medium | D1–D9 division mapping remains incomplete | Updated canonical selector with explicit record references |
| Medium | External integrations remain partly documentary | Authenticated, read-only endpoint inspection and controlled adapter receipts |

---

## 12. Definition of done

FruitfulCore should be considered minimally operational only once it can demonstrate one complete, non-sensitive source-to-projection chain:

1. A source is preserved with verifiable identity and hash.
2. The record has an explicit parent or source relationship.
3. A linked extension is recorded without overwriting source evidence.
4. A properly authorised person approves a defined projection scope.
5. A read-only projection is generated.
6. A release receipt ties the projection back to its source, approval, version, destination, and time.
7. Corrections, conflicts, revocations, and supersessions remain visible.

Until then, FruitfulCore remains a governed architecture and implementation programme—not a completed or automatically unified system of record.

FruitfulCore must not be called operational solely because a dashboard exists, a repository exists, a session is saved, or a database project is active.

### 12.1 Minimum operational readiness

Minimum operational readiness requires:

1. A durable canonical ledger.
2. Append-only event, edge, approval, and release-receipt records.
3. Preserved source references and integrity evidence.
4. Explicit authority and approval controls.
5. No raw credentials in evidence or projections.
6. Tested Row Level Security and least-privilege access.
7. One complete read-only source-to-release trace.
8. Controlled correction, revocation, and supersession handling.
9. A continuously maintained tail register for missing, stale, conflicting, or unverified evidence.

---

## 13. Next controlled move

The shortest safe move is to establish the canonical append-only ledger in the approved durable environment with row-level security and no public write path, then demonstrate one read-only GitHub specification trace end to end.

That first trace must prove mechanics only. It must not be used to claim deployment, financial authority, QS certification, inventory truth, customer consent, external synchronisation, or control of live infrastructure.

---

## 14. Closing position

FruitfulCore is a governed integration architecture in active construction, not yet a proven single deployed system of record.

The immediate safe implementation step is to create the canonical append-only Waterfall Memory Ledger in the approved Supabase environment, then preserve one harmless GitHub source at an immutable commit SHA and prove the full read-only evidence-to-release trace.

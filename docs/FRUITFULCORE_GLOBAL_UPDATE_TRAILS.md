# FruitfulCore Global Update Trails and Governance Threads

**Document status:** Project conclusion and current-state record  
**Scope:** FruitfulCore, Fruitful Portals, Heyns1000 QS Command Center, Fruitful Around Town, GitHub, Supabase, FruitfulApp/Base44, and workspace context  
**Operating doctrine:** Evidence first · append only · explicit authority · approval before projection  
**Classification:** Internal governance documentation

---

## Project conclusion

FruitfulCore is the proposed evidence-led control plane for linking Fruitful Portals, the Heyns1000 QS Command Center, Fruitful Around Town, FruitfulApp/Base44, versioned GitHub artefacts, and future durable ledger records.

It is **not yet evidenced as one deployed canonical system of record**. The estate remains distributed across workspace sessions, GitHub source history, Supabase, FruitfulApp/Base44, and related operational surfaces. Co-location, naming similarity, or sidebar visibility must not be treated as a machine-readable relationship, durable audit record, approved release, or production integration.

FruitfulCore therefore remains an architecture and governance standard until the required durable ledger, typed lineage, integrity, approval, and release evidence are implemented and verified.

---

## Waterfall Memory Flow

The governing lifecycle is:

```text
🦍 Origin
→ 💧 Captured prompt
→ 🌱 Preserved record
→ 🌿 Linked extension
→ 🌳 Approved projection
```

| Stage | Meaning | Minimum required evidence |
|---|---|---|
| 🦍 Origin | The original person, source system, document, photo, API response, commit, contract record, or site event | Source identity, source type, timestamp, source reference |
| 💧 Captured prompt | The instruction, workflow trigger, intake request, or event that initiated work | Exact captured context, actor, channel, capture time |
| 🌱 Preserved record | A retained and versioned source payload or structured record | Record ID, retention status, source link, content hash where available |
| 🌿 Linked extension | Analysis, extraction, reconciliation, classification, calculation, enrichment, or interpretation | Parent references, method/version, evidence links, confidence state |
| 🌳 Approved projection | A controlled report, dashboard, API result, certificate draft, recommendation, or published view | Authoriser, authority, policy version, scope, approval time, release receipt |

A downstream record does not replace its ancestor. Corrections, revocations, and supersessions must remain append-only and link back to the earlier record.

---

## Authority boundaries

| Surface | Evidenced role | Must not be assumed |
|---|---|---|
| Supabase / Fruitful Ledger | Intended durable location for governed records, approvals, audit events, and projections | That the current schema already contains the Waterfall Memory Ledger |
| GitHub | Versioned source, review context, documentation, commits, pull requests, and release evidence | Production state, deployed configuration, credentials, or live operational data |
| Heyns1000 QS Command Center | QS evidence, BoQ/5D-BIM, procurement, site reconciliation, professional review gates | AI authority to issue certificates, valuations, or binding commercial instructions |
| Fruitful Portals | Presentation and workflow surfaces for approved information | A canonical evidence ledger or financial/governance authority |
| Fruitful Around Town | Candidate channel for local discovery and commerce projections | Inventory truth, identity, consent, finance, pricing, or governance authority |
| FruitfulApp/Base44 | Operational entity/API surface | A verified system of record until authenticated endpoint and entity behaviour is evidenced |
| Session/workspace context | Captured working context, research continuity, and discoverability | A durable external ledger, hash graph, approval record, or release receipt |

---

## First demonstrated trace

The first end-to-end trace should use a deliberately harmless, non-secret GitHub specification file at an immutable full commit SHA.

```text
GitHub file at immutable commit SHA
→ preserved evidence event
→ typed lineage edge
→ human approval event
→ read-only projection
→ immutable release receipt
```

This is the lowest-risk test because it proves source identity, repeatability, integrity, lineage, review context, approval separation, and release receipting without touching financial, customer, payment, QS certification, inventory, DNS, Workers, Cloudflare configuration, or production data.

### Candidate order

| Source type | Sequence | Reason |
|---|---:|---|
| GitHub specification file | First | Immutable commit SHA, reproducible retrieval, low sensitivity, no business action |
| QS evidence record | Second | Requires contract context, source validation, reconciliation, and authorised professional approval |
| Fruitful product/inventory record | Third | Requires ownership, consent, pricing, tax, stock, identity, and commerce-projection controls |

### Required source metadata

The first trace must contain:

- Repository URL
- Branch
- Full Git commit SHA
- File path
- Git blob SHA where available
- Independently calculated SHA-256 of exact retrieved file content
- Source actor and capture timestamp
- Classification and sensitivity label
- Record owner
- Separate reviewer or approver
- Typed lineage relationship
- Approval record before external projection
- Release receipt identifying the controlled destination

---

## Governance gates

| Gate | Requirement |
|---|---|
| Evidence gate | Source reference, content hash, actor, timestamp, classification, and record owner are present |
| Authority gate | The action owner and permitted scope are explicitly assigned |
| Approval gate | Finance, QS certification, deployment, publishing, external writes, and binding actions require human authorisation |
| Projection gate | No dashboard, portal, API, report, or channel update is shown without a source-to-release receipt |
| Security gate | Raw secrets remain server-side; credentials, `.env` material, access tokens, customer data, payment data, and raw infrastructure values are excluded |
| Integrity gate | Hashes, immutable versions, or equivalent preservation receipts are recorded |
| Supersession gate | Corrections and revocations create append-only follow-on records rather than overwriting prior evidence |

---

## Canonical ledger model

The intended Waterfall Memory Ledger contains four core record families:

| Record family | Purpose |
|---|---|
| `memory_events` | Stores origin, prompt, preserved record, linked extension, and projection events |
| `memory_edges` | Stores explicit relationships such as `captured_from`, `preserved_as`, `extends`, `supports`, `contradicts`, `supersedes`, and `projected_from` |
| `memory_approvals` | Stores approval, rejection, revocation, and supersession decisions separately from source content |
| `memory_release_receipts` | Stores evidence that an approved projection was released or consumed by a specific destination |

The ledger must be append-only, protected by Row Level Security, and have no public write path. Raw secret values must never be stored in any evidence payload, metadata field, prompt, title, commit, release receipt, or projection.

---

## Current state

### Confirmed

- FruitfulCore is defined as an evidence-led control-plane architecture.
- The Waterfall Memory Flow is the working governance model.
- GitHub is suitable as the first low-risk, read-only demonstration source.
- GitHub, Supabase, FruitfulApp/Base44, workspace sessions, and presentation channels have distinct roles and must not be conflated.
- The Heyns1000 QS Command Center requires authorised professional approval for QS certification and binding commercial actions.
- Workspace sessions are useful captured context but are not automatically a durable external ledger.

### Not yet demonstrated

- A deployed canonical Waterfall Memory Ledger.
- Structured, machine-readable lineage edges across source systems.
- Cryptographic content integrity for all retained records.
- Formal session-to-project mapping.
- Recorded approval authority and policy controls across all projection classes.
- Immutable release receipts for operational dashboards, portals, APIs, reports, or other outputs.
- Verified cross-system synchronisation between GitHub, Supabase, FruitfulApp/Base44, Cloudflare, and workspace context.

---

## Security standard

Raw credentials are never governance evidence.

Store only safe metadata:

- Provider name
- Credential label
- Provider key ID or approved safe fingerprint
- Scope
- Expiry
- Rotation status
- Vault reference
- Revocation and deployment-update receipts

Any credential found in a title, prompt, repository, issue, log, document, screenshot, browser bundle, or chat record must be treated as exposed and rotated. Redaction reduces further spread but does not restore trust in an exposed value.

---

## Find-the-Tail register

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

## Definition of done

FruitfulCore must not be called operational solely because a dashboard exists, a repository exists, a session is saved, or a database project is active.

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

## Closing position

FruitfulCore is a governed integration architecture in active construction, not yet a proven single deployed system of record.

The immediate safe implementation step is to create the canonical append-only Waterfall Memory Ledger in the approved Supabase environment, then preserve one harmless GitHub source at an immutable commit SHA and prove the full read-only evidence-to-release trace.

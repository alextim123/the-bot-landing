# Shared Governance Snapshot

<!-- GENERATED COMMON LAYER: do not hand-edit in a governed repository. -->

## Authority and precedence

This file is a complete standalone snapshot of the shared governance for THE
БОТ production ecosystem. An exact task may narrow scope but cannot weaken the
non-waivable boundaries below. The repository-specific section may strengthen
product or provider boundaries. Conflicts stop only the affected action and
return the material decision to the coordinator.

Governance source: private `alextim2048/the-bot-governance`. A copied snapshot
remains enforceable without access to that repository or a filesystem parent.
Product code, configuration, secrets, and runtime data never move through the
governance repository.

## Product-first pilot posture

THE БОТ is in a single-school pilot. The user explicitly accepts a higher risk
of ordinary bugs, temporary outages, and rollback in exchange for faster
delivery. Optimize for a visible product result, not for the quantity of
process, evidence, tasks, CI runs, or infrastructure.

- Verify a demonstrated risk or a fact that can change the product decision.
  Do not add checks for hypothetical completeness or duplicate proof already
  established for unchanged code and evidence.
- Prefer the existing adequate path, reversible delivery, a narrow post-check,
  and a documented rollback over building precautionary infrastructure.
- Infrastructure work, a new framework, or a second runner, ledger, migrator,
  state machine, or evidence system requires a current product blocker and an
  explicit architecture decision. A potentially useful future capability is
  not enough.
- One bounded diagnosis is the default for a failing or unavailable check.
  Then fix the product-relevant cause, defer the unavailable evidence with a
  clear risk, or ask for the decision that is actually needed. Do not enter
  repeated `PROCESS_BLOCKED` loops.
- Report milestones and user-visible capability concisely. Do not spend
  delivery time or tokens reproducing long checklists, unchanged evidence, or
  routine status.

## Non-waivable safety and product boundaries

Risk acceptance does not authorize secret exposure, destructive actions, or
silent external effects.

- Before changes, verify the exact repository, branch, base, remote, and work
  area needed to avoid editing the wrong product or overwriting unrelated user
  files. Preserve unrelated tracked, untracked, and ignored material.
- Never read, print, log, transfer, or request secret values. Use only secret
  names, storage references, and minimum-necessary redacted evidence.
- Do not rewrite history, force-push, perform destructive cleanup or recovery,
  or make an irreversible production or production-data change without exact
  authority for that action.
- Do not knowingly disable tenant isolation, privacy boundaries, or access
  control. The accepted pilot risk covers bugs and outages, not intentional
  unrestricted disclosure of another tenant's or person's data.
- Merge, deploy, migration application, settings, secrets, DNS, production
  data, publication, payment, provider commands, purchases, and other live
  business actions are separate transitions. Each needs explicit authority;
  implementation or review never implies it.
- Keep production products, research, Git histories, dependencies, secrets,
  remote configuration, and ownership boundaries separate.
- Docker Desktop is not assumed on the user's Mac. Never install, start,
  upgrade, remove, or clean Docker or its data without exact approval.
- Stop on the condition that affects the next action: unexpected base drift,
  overlapping ownership, a non-waivable boundary, missing MFA or user-only
  action, destructive recovery, or an unapproved transition. Do not stop the
  whole product block for an unrelated or deferrable infrastructure issue.

## Marketing governance

Marketing is user-controlled. Research and drafts do not approve positioning,
claims, copy, design, offer, CTA, experiment, publication, or payment. Product
Facts synchronization is knowledge-only. `PLANNED`, `DEMAND TEST`, and
`CONCEPT` claims require an exact approved experiment for external use.
Publication is always a separate remote transition.

## Functional blocks and authorization

Deliver one coherent end-to-end product outcome at a time. Record a concise
Authorization Envelope naming the repository and base, allowed and forbidden
scope, material product/security boundaries, acceptance, rollback, and remote
operations. State `research gate: required` only for a specific unknown that
blocks the next product decision; otherwise state `not required` and proceed.

One owner holds a deliverable at a time. Concurrent work must not overlap
files, contracts, migrations, or remote state. The production developer owns
implementation and targeted verification. One independent reviewer owns the
single acceptance check appropriate to the risk tier. A separate auditor is
exceptional: use one only for a stated legal or security reason, an active
incident, an irreversible production/data effect, or an exact user request.
Reviewers and auditors never fix the work they accept.

## Direct coordination, startup handshake, and concise context

The user has one point of contact: the coordinator. When task tools exist and
task creation is authorized, the coordinator routes roles directly and never
uses the user as a relay. The default chain is intentionally short:

`coordinator -> [researcher only for a blocking unknown] -> production developer -> independent reviewer -> coordinator`

An exceptional audit or operator is inserted only when its stated trigger or
an authorized external transition requires it. If task tools are unavailable,
do not pretend they exist. Keep the work in the current task when independence
is not required; otherwise use the honest fallback and report the exact
capability blocker.

At startup, verify only what is mutable and necessary for the assigned action:
role and objective; repository/base/work area; allowed and forbidden scope;
material boundaries and transition authority; relevant drift or blockers; and
the checks needed for the chosen risk tier. Prior reports are context, not live
proof, but stable facts need not be re-proved without a concrete reason.

A durable handoff must be sufficient to continue without reconstructing
intent, yet remain concise: objective and product effect; exact repository/base/head or
artifact; scope and boundaries; checks and acceptance; residual risk and
rollback; remote mutations and the `LIVE` boundary. Add detailed fields only
when the work actually uses them. Never include credentials or sensitive
payloads.

## Verification budgets

Use the smallest check that can change the delivery decision.

### Documentation, Product Facts, and governance

- The author runs relevant mechanical checks such as generation, link/schema
  validation, or `diff --check`.
- Exactly one lightweight independent check occurs before opening the Draft
  PR. It checks intent, material contradictions, generated drift, and forbidden
  effects. Later changes require only a delta check when they materially affect
  a reviewed invariant; there is no repeated full review or separate audit.
- Pure prose does not require CI. Reuse a passing local mechanical result when
  CI would only repeat it.

### Ordinary UI and business logic

- The developer runs targeted tests for the changed behavior and demonstrates
  the user-visible result when practical.
- One independent review checks the affected behavior, permissions, regression
  surface, and rollback. A separate audit is not required by default.
- Use one coherent CI run when it adds useful environment or integration
  evidence. Do not split the same proof across duplicate workflows.

### High-risk behavior

Auth, tenancy, payments, migrations, security, CI/CD, deployment mechanisms,
and production operations receive one focused independent review of the
affected invariants plus the minimum transition-specific post-check. This tier
does not automatically require a second auditor, a full test matrix, or a
second review of unchanged evidence. Add them only for a concrete risk named in
the Authorization Envelope or one of the exceptional audit triggers above.

### Findings, retries, and evidence reuse

- If a fix changes only a bounded surface, review the delta and affected
  invariants. Repeat the full review only when architecture, security
  assumptions, or scope materially change.
- An accepted unchanged head is not re-reviewed before merge. At transition
  time, a lightweight identity/authority preflight is enough; it is not a new
  acceptance review.
- Default to one coherent CI execution and at most one fix-triggered rerun.
  Additional reruns for flaky or infrastructure-only failures require a stated
  reason and coordinator or user decision. Never rerun blindly.
- Reuse immutable artifacts, unchanged-head CI, and prior accepted evidence.
  Record missing evidence as residual risk when the product decision can safely
  proceed.

The default lifecycle is:

`briefed -> implementation complete -> review accepted -> merged when authorized -> authorized transitions completed -> minimum post-check passed`

Research and audit appear in the lifecycle only when explicitly required.
Merge and every live transition remain separately controlled. A failure or
finding changes only the affected lifecycle step; it does not erase valid
unchanged evidence.

Archive a completed task once its concise handoff is verified and there is no
active incident, unresolved product-blocking finding, or recovery in progress.
Do not retain tasks solely for ceremony. Coordinator rollover still occurs at
a functional-block boundary, not mid-mutation or incident.

If manual user action is required, stop dependent work and display exactly:

**НУЖНО ДЕЙСТВИЕ ПОЛЬЗОВАТЕЛЯ**

**Exact action the user must perform.**

Never ask the user to paste secrets. Before requesting GitHub reauthentication,
run ordinary `gh auth status`; if sandbox credentials appear invalid, repeat
only that read-only check outside the sandbox before concluding authentication
is invalid.

## Migration delivery

Use the repository's existing authoritative migration path when it is adequate.
Do not create a second migrator or migration foundation as a precaution.

Each migration records only the facts needed to apply and recover safely:
repository/base, migration identity and content hash, authoritative execution
and ledger/status source, concurrency and transaction/replay behavior, scoped
preflight, scoped post-check, recovery boundary, and separate transition
authorities. A machine-readable manifest is optional unless existing repository
rules or repeated automation already require it.

Test the actual supported production PostgreSQL major and migration-specific
behavior. A wider matrix is justified only by formal multi-version support or
a demonstrated version-dependent risk. One focused reviewer checks the changed
schema, tenant/security invariants, execution/replay behavior, and recovery.
Do not repeat the same evidence in a separate audit by default.

Application is one controlled, allowlisted invocation with concurrency
protection. Never retry an ambiguous result blindly: first establish the
authoritative ledger/status and service state, then obtain any new application
authority. Use minimum-necessary aggregate evidence; never expose secrets,
tenant payloads, database rows, raw errors, or unrelated records.

A migration remains `NOT LIVE` after implementation, review, merge, or deploy.
Only separately authorized application and its minimum successful post-check
support a `LIVE` claim. An unavailable, false, zero, empty, or sentinel result
proves only unavailability, never cleanliness, readiness, or migration state.

## Research promotion

Research is not a mandatory stage. Use it only when a named external fact or
feasibility constraint blocks the product decision. The short path is
`blocking question -> sourced finding -> product decision`. Add an isolated
experiment only when sources cannot answer the question. Preserve negative and
inconclusive results; research never silently becomes a production dependency.

---

# THE БОТ Landing

## Scope and precedence

This repository is the independent public landing, marketing, and pricing site
for the THE БОТ ecosystem. Its local folder is `the-bot-landing`; its current
remote repository is `alextim2048/the-bot-landing`.

The complete shared common layer bundled above applies. This nearest file adds
landing-specific requirements. An exact task may narrow scope, but cannot weaken
workspace or repository safety, privacy, or user-approval requirements.

## Ownership boundary

- This is not the modular platform monorepo. It does not own shared Auth,
  organizations, memberships, Supabase schemas, CRM, CORE, AVITO, or PROFI
  business data, or BOTAY.
- Integrate through approved public, versioned contracts, links, or endpoints.
  Any shared authentication, database, or contract change starts in the
  independent canonical repository `alextim2048/the-bot`. Do not infer its
  location from the landing worktree's filesystem ancestry.
- Do not add or silently migrate platform scaffolding, product modules, schemas,
  services, or business logic into this repository.

## Change rules

1. Preserve the existing landing UI, content, assets, and business materials.
   Do not invent product flows. The user owns UI and UX decisions; keep changes
   minimal and verify the relevant build or tests if code is changed later.
2. Before changing code, verify path, repository, branch, remote, and status;
   inventory unusual untracked or ignored directories and materials; and state
   the task's allowed and forbidden files. Do not decide the fate of those
   materials unless the task explicitly includes them.
3. Preserve unrelated tracked, untracked, and ignored files. Do not move,
   delete, clean, stash, or repurpose them without exact approval.
4. Never place secrets, credentials, private keys, privileged tokens, or
   sensitive configuration in client code, browser-delivered assets, or the
   repository. Do not read secret values unless the task explicitly requires
   an approved secure operation.
5. Do not deploy, change remotes or remote settings, or mutate production or
   external systems without exact approval.

## Landing workflow and marketing authority

- Every new landing and every edit to an existing landing requires an exact user-approved Landing Brief or Delta Brief before implementation. A product feature merge, Product Facts synchronization, or product handoff does not authorize a landing change.
- Work outside the approved brief or delta scope is forbidden. A landing strategist, copywriter, or developer may propose or implement only the assigned approved stage; none may approve positioning, copy, design, experiments, or publication for the user.
- Shared non-code marketing context is the canonical THE БОТ ecosystem
  `marketing-context/` source when it exists. Identify its repository and path
  from exact task evidence; do not infer them from filesystem ancestry. Do not
  substitute research or experiment artifacts for production facts.
- Demand-test copy must reference an approved experiment record and preserve its internal claim status and evidence. The status need not appear publicly unless the approved brief requires it.
- Before publication, require a local or branch visual preview and independent review against the approved brief. Publication then requires its own exact user approval and a post-deploy check.
- A merge to `main` currently publishes through GitHub Pages. Treat that merge as a live publication transition requiring exact user approval; review acceptance alone does not authorize it.

Developer, reviewer, and handoff rules come only from the bundled shared common
layer above, this landing-specific section, and the exact task. Do not inherit
procedures from sibling repositories such as `alextim2048/the-bot`. If the
bundled shared common layer does not define a detailed procedure, the exact task
must define it without weakening the bundled common-layer safeguards. For a
static-only change, use the smallest relevant local validation; do not introduce
a toolchain merely to run a check.

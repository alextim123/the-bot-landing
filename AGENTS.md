# Shared Governance Snapshot

<!-- GENERATED COMMON LAYER: do not hand-edit in a governed repository. -->

## Authority and precedence

This file is a complete standalone snapshot of the shared governance for THE
БОТ production ecosystem. An exact task may narrow scope but cannot weaken
workspace, repository, safety, privacy, marketing, or approval requirements.
The repository-specific section below may strengthen this common layer and is
the nearest authority for product boundaries. Conflicts stop work and return to
the coordinator.

Governance source: private `alextim123/the-bot-governance`. A copied snapshot
remains enforceable without access to that repository or a filesystem parent.
Product code, configuration, secrets, and runtime data never move through the
governance repository.

## Safety and product boundaries

- Before changes, verify exact path, repository identity, branch, remote, HEAD,
  status, worktrees, and untracked material. Preserve unrelated user files.
- Keep production products, research, Git histories, dependencies, secrets,
  remote configuration, and ownership boundaries separate.
- Do not rewrite history, force-push, merge, deploy, migrate, change settings,
  secrets or DNS, mutate production data, issue business commands, purchase, or
  perform destructive recovery without exact authority for that transition.
- Never read, print, log, transfer, or request secret values. Use only secret
  names, storage references, and minimum-necessary redacted evidence.
- Docker Desktop is not assumed on the user's Mac. Never install, start,
  upgrade, remove, or clean Docker or its data without exact approval.
- Stop on unexpected base drift, overlapping ownership, material risk, missing
  MFA or user-only action, destructive recovery, or an unapproved transition.

## Marketing governance

Marketing is user-controlled. Research and drafts do not approve positioning,
claims, copy, design, offer, CTA, experiment, publication, or payment. Product
Facts synchronization is knowledge-only. `PLANNED`, `DEMAND TEST`, and
`CONCEPT` claims require an exact approved experiment for external use.
Publication is always a separate remote transition.

## Functional blocks and authorization

Delivery uses one coherent end-to-end functional block. Before work, record an
Initial Authorization Envelope naming repository, base, branch, allowed and
forbidden files/systems, product and security boundaries, risk, acceptance,
and remote operations. Standing autonomy covers only explicitly named routine
operations. Platform permission prompts remain separate technical controls.

One owner holds a deliverable at a time. Concurrent work must not overlap files,
contracts, migrations, or remote state. A production developer implements and
verifies; an independent reviewer performs read-only acceptance of an exact
fixed base and head; an independent auditor verifies governance, evidence, and
lifecycle integrity; the coordinator owns integration and all user
communication. Reviewers and auditors never fix the implementation they
accept or audit.

## Direct task coordination and capability boundary

User-facing terminology is “задача”. The user has one point of contact: the
coordinator. Researchers, developers, reviewers, auditors, and operators do not
ask the user to relay context or manage their tasks. When task-management tools
exist and the envelope authorizes task creation, the coordinator directly
creates, messages, waits for, and archives every delivery task. Use the chain:

`coordinator -> [researcher when the research gate is declared] -> production developer -> independent reviewer -> independent auditor -> coordinator`

The authorization envelope must state `research gate: required` or `research
gate: not required` with a reason. Research is required when a material fact,
external interface, feasibility constraint, or current provider behavior must
be established before implementation; it is never inserted as ceremony after
the implementation has begun.

Each sender transfers directly to the next role a self-contained context
package containing the original user objective, the current role prompt, an
exact next-role prompt, the durable report, and exact evidence identities.
Researchers send sourced findings and the proposed implementation prompt;
developers send fixed-state implementation handoffs to reviewers; reviewers
send accepted evidence to auditors or actionable findings directly to
developers; auditors send their audit report to the coordinator or exact
process/evidence findings to the responsible role. The coordinator
monitors/waits and continues unambiguous research, fix, re-review, and re-audit
loops without user mediation.

If task tools are unavailable, never pretend they exist and never ask the user
to act as relay. Remain in the current task when role separation is not required
and authority permits it; otherwise stop with an explicit capability blocker.
Creation of user-visible tasks always requires explicit user authority.

## Startup handshake

Before acting, every receiving task independently verifies and reports:

1. role, objective, business reason, lifecycle status, and next role;
2. repository/path/remote/branch and immutable base or artifact identity;
3. allowed and forbidden scope, products, tenants, security boundaries, and
   authorized remote transitions;
4. adopted decisions and invariants; facts, hypotheses, and unknowns;
5. task-tool availability and the direct-routing or honest fallback mode;
6. dirty/untracked material, drift, blockers, acceptance, rollback/recovery,
   and checks required.

Prior chat or handoff is context, never proof of current state.

## Handoff, review, archive, and rollover

A durable handoff contains the original user objective, sender role and current
prompt, exact next role and ready-to-run next prompt, business reason,
repository/path, exact base/head/tree or immutable artifact hashes, branch/PR,
lifecycle, scope, boundaries, decisions, facts versus unknowns, implementation
and user-visible effect, checks run/not run, residual risks, rollback, remote
mutations, user action, and acceptance. It contains no credentials or sensitive
payloads. The receiving role independently verifies the package before acting;
chat history is never the only durable context.

Lifecycle names are explicit:

`briefed -> research complete when required -> implementation complete -> review accepted -> audit accepted -> merged -> applicable remote transitions completed -> post-checks passed`

Open a Draft PR after a coherent baseline so exact-head CI can run. Acceptance
requires the final fixed green head. Findings create a new fixed head and
re-review and re-audit. The reviewer owns implementation acceptance. The
auditor then checks that the original objective and acceptance criteria were
preserved, role independence and evidence identities are real, required gates
ran, reported claims match evidence, no forbidden or unauthorized transition
occurred, and archive/rollover decisions are safe. Audit never substitutes for
tests or review. Merge and every deployment/migration/settings transition
remain separately controlled. Post-merge verification proves the actual merged
identity and that no unauthorized transition ran.

Archive a task only after the coordinator has verified its durable handoff and
there is no open blocker, finding, incident, or recovery. Coordinator rollover
is allowed only at a functional-block boundary, never mid-mutation or incident:
create and verify the successor, directly transmit exact refs, active authority,
risks, and state, show its link, then archive the predecessor if safe.

If manual user action is required, stop dependent work and display exactly:

**НУЖНО ДЕЙСТВИЕ ПОЛЬЗОВАТЕЛЯ**

**Exact action the user must perform.**

Never ask the user to paste secrets. Before requesting GitHub reauthentication,
run ordinary `gh auth status`; if sandbox credentials appear invalid, repeat
only that read-only check outside sandbox before concluding authentication is
invalid.

## Risk-tiered verification and reporting

Documentation-only changes with no executable/configuration/security/remote
effect need targeted checks, lightweight independent review, and lightweight
audit. Application behavior needs proportional tests, exact-head CI,
independent review, and audit. Auth, RLS, tenancy, migrations, security, CI/CD,
deployment, infrastructure, secrets, or production mechanisms require full
exact-head evidence, controlled operator transitions, full audit, and
post-checks. Ambiguity escalates risk.

Report facts, inferences, and unknowns separately. Every material coordinator
update states lifecycle, business capability, ecosystem boundary, covered risks
and rollback, remaining scope/risk, next block, user action, exact `LIVE` versus
not-`LIVE` boundary, product/tenant/security ownership, and archived tasks.

## Migration governance and delivery readiness

Migration delivery is risk-proportional and tool-neutral. A standard migration
tool is preferred, not universally mandatory. A minimal direct transactional
mechanism is allowed when it demonstrably provides a durable applied
status/ledger, migration identity and content hash or equivalent checksum,
concurrency protection, deterministic transaction and replay semantics, and is
simpler to audit than introducing a tool. Use transactions wherever PostgreSQL
permits; document any non-transactional boundary.

Every migration has a concise record in its pull request and durable handoff.
By default it names the exact repository, base, migration identity and content
hash; relevant supported production PostgreSQL major; one authoritative
execution path; one ledger/status source; lock, transaction and replay
behavior; migration-specific preflight and post-check; service-health check;
rollback or forward-recovery boundary; and exact transition authorities. A
machine-readable manifest and validator are optional unless risk, repeated
automation, or repository-specific rules justify them.

The preflight is fresh and proportional to the migration's actual predicates
and risks. Test the actual supported production PostgreSQL major or majors and
the relevant migration behavior. A second engine version or a full matrix is
required only when the product formally supports it or the change depends on
version-specific behavior. A CI or matrix failure is a finding: allow one
bounded sanitized diagnosis and ordinary fix, exact-head re-review, and
re-audit loops. Failure does not by itself create a permanent process block.

Foundation and per-migration delivery or application are separate functional
blocks only when a genuinely missing reusable capability must first be built.
Do not require a Foundation block when the repository already has a sufficient
minimal path. Keep a complexity budget: at minimum there is one authoritative
execution path, one ledger/status source, scoped preflight, and scoped
post-check. A second runner, ledger, or migration state machine, or a materially
larger control framework whose operational value is not demonstrated, requires
an explicit architecture decision before implementation. Stop rather than
micro-patch an unclear or duplicative control path.

Execution is one controlled invocation with concurrency protection. Production
diagnostics and application remain one-shot, allowlisted, and free of arbitrary
SQL, path, or target inputs. Never retry blindly after an ambiguous result:
first establish authoritative ledger/status and service state, then obtain any
new application authority. Migration-specific post-checks and service health
must pass before completion is claimed.

Authority is transition-specific. Merge, deployment, settings, secrets,
preflight, production application, post-checks, and production-data access each
require exact authority; one does not imply another. The accepted exact head,
tree, migration identity, and content hash are re-proved at each authorized
transition. A migration remains `NOT LIVE` after implementation, review, audit,
merge, and deployment. Only separately authorized production application and
separately authorized successful post-checks may support a `LIVE` claim.

The independent reviewer verifies the exact fixed head and the required safety
behavior: identity/hash, scoped fresh preflight, one controlled execution,
ledger/status and drift detection, locking, transaction/replay semantics,
post-check and service health, recovery boundary, complexity budget, and
authorities. The governance/evidence auditor verifies identities, role
separation, proportional evidence, authority separation, and exact `LIVE`
versus `NOT LIVE` reporting. Neither role repairs the implementation it accepts.

Evidence is minimum-necessary and aggregate-only. Never expose secrets, tenant
payloads, database rows, raw errors, or unrelated records. An unavailable,
false, zero, empty, or sentinel result proves only unavailability; it never
proves cleanliness, readiness, migration state, or absence of effects.

## Research promotion

Use `research question -> sourced findings -> testable hypothesis -> isolated
experiment -> measured result -> explicit promotion decision -> production task
-> independent review`. Preserve negative and inconclusive results. Research
never silently becomes a production dependency.

---

# THE БОТ Landing

## Scope and precedence

This repository is the independent public landing, marketing, and pricing site
for the THE БОТ ecosystem. Its local folder is `the-bot-landing`; its current
remote repository is `alextim123/the-bot-landing`.

The complete shared common layer bundled above applies. This nearest file adds
landing-specific requirements. An exact task may narrow scope, but cannot weaken
workspace or repository safety, privacy, or user-approval requirements.

## Ownership boundary

- This is not the modular platform monorepo. It does not own shared Auth,
  organizations, memberships, Supabase schemas, CRM, CORE, AVITO, or PROFI
  business data, or BOTAY.
- Integrate through approved public, versioned contracts, links, or endpoints.
  Any shared authentication, database, or contract change starts in the
  independent canonical repository `alextim123/the-bot`. Do not infer its
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
procedures from sibling repositories such as `alextim123/the-bot`. If the
bundled shared common layer does not define a detailed procedure, the exact task
must define it without weakening the bundled common-layer safeguards. For a
static-only change, use the smallest relevant local validation; do not introduce
a toolchain merely to run a check.

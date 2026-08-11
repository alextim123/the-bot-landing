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
fixed base and head; the coordinator owns integration and user communication.
Reviewers never fix the implementation they accept.

## Direct task coordination and capability boundary

User-facing terminology is “задача”. When task-management tools exist and the
envelope authorizes task creation, the coordinator directly creates, messages,
waits for, and archives developer, reviewer, and operator tasks. Use the chain:

`coordinator -> production developer -> independent reviewer -> coordinator`

Developers send fixed-state handoffs directly to reviewers; reviewers send
reports directly to the coordinator and findings directly to developers.
The coordinator monitors/waits and continues an unambiguous fix/re-review loop.
The user is never asked to relay prompts, identifiers, findings, or routine
status.

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

A durable handoff contains objective, business reason, repository/path, exact
base/head/tree, branch/PR, lifecycle/next role, scope, boundaries, decisions,
facts versus unknowns, implementation and user-visible effect, checks run/not
run, residual risks, rollback, remote mutations, user action, and acceptance.
It contains no credentials or sensitive payloads.

Lifecycle names are explicit:

`briefed -> implementation complete -> review accepted -> merged -> applicable remote transitions completed -> post-checks passed`

Open a Draft PR after a coherent baseline so exact-head CI can run. Acceptance
requires the final fixed green head. Findings create a new fixed head and
re-review. Merge and every deployment/migration/settings transition remain
separately controlled. Post-merge verification proves the actual merged
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
effect need targeted checks and lightweight independent review. Application
behavior needs proportional tests, exact-head CI, and independent review. Auth,
RLS, tenancy, migrations, security, CI/CD, deployment, infrastructure, secrets,
or production mechanisms require full exact-head evidence, controlled operator
transitions, and post-checks. Ambiguity escalates risk.

Report facts, inferences, and unknowns separately. Every material coordinator
update states lifecycle, business capability, ecosystem boundary, covered risks
and rollback, remaining scope/risk, next block, user action, exact `LIVE` versus
not-`LIVE` boundary, product/tenant/security ownership, and archived tasks.

## Research promotion

Use `research question -> sourced findings -> testable hypothesis -> isolated
experiment -> measured result -> explicit promotion decision -> production task
-> independent review`. Preserve negative and inconclusive results. Research
never silently becomes a production dependency.

---

# THE БОТ Landing — repository-specific governance

This independent repository owns the public landing, pricing and marketing
site, not platform identity, schemas, product modules, or business data. Shared
runtime contracts start in the platform repository.

Preserve UI, content, assets and business materials. Every landing change needs
an exact user-approved Landing Brief or Delta Brief; governance synchronization
does not authorize marketing mutation. Before publication require preview and
independent review. Merge to `main` publishes GitHub Pages and is a live remote
transition requiring separate exact approval.

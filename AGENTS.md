# THE БОТ Landing

## Scope and precedence

This repository is the independent public landing, marketing, and pricing site
for the THE БОТ ecosystem. Its local folder is `the-bot-landing`; its current
remote repository is `alextim123/the-bot-landing`.

The umbrella [`../AGENTS.md`](../AGENTS.md) applies. This nearest file adds
landing-specific requirements. An exact task may narrow scope, but cannot weaken
workspace or repository safety, privacy, or user-approval requirements.

## Ownership boundary

- This is not the modular platform monorepo. It does not own shared Auth,
  organizations, memberships, Supabase schemas, CRM, CORE, AVITO, or PROFI
  business data, or BOTAY.
- Integrate through approved public, versioned contracts, links, or endpoints.
  Any shared authentication, database, or contract change starts in the
  canonical `../the-bot/` repository.
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
- Shared non-code marketing context is expected at [`../marketing-context/`](../marketing-context/) when it exists. Do not substitute research or experiment artifacts for production facts.
- Demand-test copy must reference an approved experiment record and preserve its internal claim status and evidence. The status need not appear publicly unless the approved brief requires it.
- Before publication, require a local or branch visual preview and independent review against the approved brief. Publication then requires its own exact user approval and a post-deploy check.
- A merge to `main` currently publishes through GitHub Pages. Treat that merge as a live publication transition requiring exact user approval; review acceptance alone does not authorize it.

Developer, reviewer, and handoff rules come only from the umbrella instructions
and the exact task. Do not inherit procedures from sibling repositories such as
`../the-bot/`. If the umbrella does not define a detailed procedure, the exact
task must define it without weakening the umbrella safeguards. For a static-only
change, use the smallest relevant local validation; do not introduce a toolchain
merely to run a check.

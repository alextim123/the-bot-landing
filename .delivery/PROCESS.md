# Shared development and release process

This file is canonical for all registered THE БОТ repositories. Product adapters
retain their own commands and security invariants; they cannot weaken this process.

1. Implement one scoped outcome; preserve unrelated work and tenant boundaries.
2. Run targeted author checks and record the fixed source/evidence.
3. Obtain one independent review of that source; review fixes as a delta.
4. Build one immutable candidate from the accepted source. Reuse that artifact;
   deployment verifies its producer, source SHA and archive digest without rebuilding.
5. Merge, production deployment, migration application, provider actions and
   landing publication each require their own explicit scoped authorization.
6. Execute the applicable existing adapter and one narrow post-check. Never
   retry an ambiguous production command before establishing authoritative state.

Draft CI is not release evidence. Documentation does not need a production build.
Authentication, tenancy, payments, migrations and irreversible data changes require
focused invariant checks. Preserve the authoritative product-specific checks.

No production adapter exists in the registered landing or PROFI workflow set.
This distribution does not create one or authorize provider actions. Landing
publication may be driven by repository settings outside these workflows; inspect
those settings before any authorized merge. Reserved BOTAY directories are not
repositories and cannot be enrolled until independently authorized and initialized.

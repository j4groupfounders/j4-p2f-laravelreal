# p2-17-laravelreal — GREEN
Migration: **Laravel 9.17.0 → 10.48.29**.
Why meaningful: Laravel 9 to 10 raises PHP requirements and changes framework contracts, Monolog and companion packages; complete RealWorld authentication/article API suite retained.
Source: https://github.com/f1amy/laravel-realworld-example-app @ c14fb8370b71a42a3a74b8ea936a1f96b2af9d69.
Preregistered jointly before any upgrade branch: https://github.com/j4groupfounders/j4-upgrades-harness/commit/1ce93ac5399d6b1ee6d45e716efd7da315ec20f2.
Frozen baseline SHA 02e1e3a6123ccebec412324cc971e1f2bc14b6f1; CI https://github.com/j4groupfounders/j4-p2f-laravelreal/actions/runs/37663889755.

## Verdict
All five protocol criteria pass.
Project baseline: 121 passes, 0 unchanged upstream skips. Same named inventory on accepted upgrade; no tests deleted or newly skipped.
Upgrade evidence: https://github.com/j4groupfounders/j4-p2f-laravelreal/actions/runs/37664227079.
Seed evidence: https://github.com/j4groupfounders/j4-p2f-laravelreal/actions/runs/37664442750.
Independent faults: project tests 5/5; combined 5/5; infrastructure-clean=True. Required >=4/5 combined AND combined miss rate <=half project miss rate. Infrastructure failures never count.
7 workflow runs (cap 12 including screening); 5.17 actual job-minutes. Seed matrix is five fresh-checkout jobs, not one shared mutation loop. Explicit bash -eo pipefail. Public standard Linux Actions only.
Zero human app/test/config edits. No paid APIs/services/model API calls or customer/upstream contact. Codex session token cost unavailable, not represented as zero measured cost.

## Migration and classified behavior
Laravel/Sanctum/Collision/Ignition major constraints and PHP platform requirement migrated; no app/test logic edits.
HTTP classification: None; HTTP snapshots identical.

## Limits and baseline repairs
See PREREG.md in the harness for fixed surfaces, immutable faults and exact baseline dependency/inventory evidence.
Unauthenticated HTTP characterization only; authenticated CRUD is covered by existing Laravel/Express tests, not a frozen differential replay. No broad route/line-coverage claim. Deliberately measured seeded sample, not production certification.
Laravel 10 destination is historical/EOL; not a supported production recommendation. Petclinic is the app used in p2-08 but a different historical major migration; its J4 source fork is detached from the GitHub network, with full source ancestry preserved.
Express baseline required inert OAuth constructor values and explicit test-mode listener. Laravel baseline required PHP 8.1 for old Carbon and removal of dev-latest advisory meta-package, not runtime/test removal; one unavailable Composer version caused an infrastructure failure. Petclinic's milestone/snapshot repositories removed; style/alternate build/database variants not part of default Maven acceptance.

## Seed outcomes
- 0: article creation status wrong — project=True, HTTP=False, combined=True, infrastructure=False; 
- 1: article body lost — project=True, HTTP=False, combined=True, infrastructure=False; 
- 2: article title lost — project=True, HTTP=False, combined=True, infrastructure=False; 
- 3: user email lost — project=True, HTTP=False, combined=True, infrastructure=False; 
- 4: favorites count off by one — project=True, HTTP=False, combined=True, infrastructure=False; 

## All CI runs
- https://github.com/j4groupfounders/j4-p2f-laravelreal/actions/runs/37662690379 — j4/p2f-baseline, failure, 1.83 job-min, SHA a1d50fff5df76d4a354d94da15a5916395a35bac.
- https://github.com/j4groupfounders/j4-p2f-laravelreal/actions/runs/37663129723 — j4/p2f-baseline, failure, 0.18 job-min, SHA 479734ebd3065798a4b3ccd4f26bd0262f40004e.
- https://github.com/j4groupfounders/j4-p2f-laravelreal/actions/runs/37663430267 — j4/p2f-baseline, success, 0.35 job-min, SHA 149e4115c12bd9063269e2bf42771ac3cae8ae5a.
- https://github.com/j4groupfounders/j4-p2f-laravelreal/actions/runs/37663889755 — j4/p2f-baseline, success, 0.30 job-min, SHA 02e1e3a6123ccebec412324cc971e1f2bc14b6f1.
- https://github.com/j4groupfounders/j4-p2f-laravelreal/actions/runs/37664113235 — j4/p2f-upgrade, success, 0.38 job-min, SHA a066bf8de3375f7ce6cd930540cc8b1895da59ef.
- https://github.com/j4groupfounders/j4-p2f-laravelreal/actions/runs/37664227079 — j4/p2f-upgrade, success, 0.42 job-min, SHA b31859e2c8a9aabb4aa7b82ea886f38cfa4da1bc.
- https://github.com/j4groupfounders/j4-p2f-laravelreal/actions/runs/37664442750 — j4/p2f-seeds, success, 1.70 job-min, SHA c751167d088a731df260a516fa9d10275fb0e028.

## Upgrade diff scope

.github/workflows/j4-p2f.yml |    6 +
 composer.json                |   12 +-
 composer.lock                | 4492 ++++++++++++++++++++++++------------------
 3 files changed, 2600 insertions(+), 1910 deletions(-)

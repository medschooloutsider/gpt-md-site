# Workspace Start Here

Read these files in order before starting meaningful work:

1. `WORKSPACE_HANDOFF.md`
2. `APP_DEVELOPMENT_LOG.md`
3. `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/docs/coordination/MASTER_PLAN.md`
4. `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/WORKSPACE_HANDOFF.md`
5. `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/docs/coordination/MASTER_PLAN.md`
6. `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/WORKSPACE_HANDOFF.md`
7. `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/docs/coordination/APP_WIDE_CONCERN_ROUTING.md`
8. `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/APP_DEVELOPMENT_LOG.md`
9. `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/APP_DEV_PORTFOLIO_LEDGER.md`
10. `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/docs/app_dev_logging_contract.md`
11. `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/docs/app_dev_scope_contract.md`
12. `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/docs/app_dev_master_plan_contract.md`

## Startup Gate

- run `python3 "/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/scripts/check_appdev_coordination_readiness.py" --surface-root "." --surface-kind lane` from this directory before meaningful work
- if the check fails, restore or re-scaffold the missing coordination files before continuing
- run `python3 "/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/scripts/check_appdev_master_plan.py" --surface-root "." --surface-kind lane` before meaningful work
- run `python3 "/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/scripts/check_appdev_scope.py" --surface-root "." --surface-kind lane` before meaningful work

## Operating Rule

- keep this lane site-only: static homepage copy, legal pages, commerce copy, site assets, and published CSS
- do not mix product-code, extraction behavior, browser-recognition work, packaged QA, or App Store signing work into this publish lane by habit
- stay here when the work is site-only or publish-only
- move back to the GPT-MD app or QA-signoff surface when the work is extraction behavior, managed-browser behavior, packaged QA, or release-signoff proof

## Update Rule

- append `APP_DEVELOPMENT_LOG.md` for meaningful site-publish events
- mirror durable commercialisation milestones into `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/APP_DEVELOPMENT_LOG.md`
- update `WORKSPACE_HANDOFF.md` when current site truth, proof state, blockers, or next slices change
- reread `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/docs/coordination/MASTER_PLAN.md` after the outcome is known and before user-facing closeout
- update `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/APP_DEV_PORTFOLIO_LEDGER.md` if lane status, proof truth, or next-slice truth changed

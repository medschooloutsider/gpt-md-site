# Workspace Handoff

Updated: 2026-04-24 18:00 CEST

## Lane

- Branch: `main`
- Worktree: `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/publishing/gpt-md-site`
- Responsibility: GPT-MD public marketing site and legal pages
- Merge target: `none; shared public site repo`

## Current Objective

- keep the GPT-MD public site aligned with the current marketing diagnosis, the live Lemon Squeezy checkout, the `HK$88` price, and the source launch copy while avoiding internal QA/process language in buyer-facing sections

## What Is Already Done

- the public site repo now exists locally as a separate GPT-MD surface
- landing page copy reflects the launch-ready GPT-MD message from the commercial docs
- the page structure now uses dedicated What, Why, Advantage, Workflow, Proof, Technical Specifications, Buy, and Legal sections
- the prior Advantage/QA-heavy material has been folded into buyer-facing workflow and proof copy
- the homepage hero is now rewritten around the diagnosis-approved workflow promise: ChatGPT project tabs to selected responses to previewed Markdown output
- the top-of-page badges now emphasize buyer-facing workflow claims instead of support or release-lane details
- primary homepage copy now avoids leading with QA lanes, fixtures, and release machinery
- `WORKSPACE_START_HERE.md` now carries the required AppDev startup, master-plan, scope, ledger, logging-contract, and handoff anchors
- privacy, terms, and proof pages are present
- the site uses the GPT-MD app icon as the visual anchor
- the homepage hero now uses a real GPT-MD app-window capture from the commercial QA app-surface harness instead of the icon-only visual; the site copy is stored at `site-assets/generated/gpt-md-app-workflow-window.png` with its capture sidecar JSON
- the homepage now matches the PDF-MD page depth more closely with a Why section, Advantage comparison, screenshot grid, six-card Technical Specifications section, proof modal action, and EULA legal card
- the generated workflow image is constrained as a bounded 16:9 figure beside the workflow steps instead of a full-width vertically dominant block
- site commit `d208627` was pushed to `medschooloutsider/gpt-md-site`, GitHub Pages finished building, and the live HTML includes `#why`, `#advantage`, `#specs`, and the proof modal trigger

## Left To Do

- keep the live GPT-MD checkout URL, `HK$88` price, and support email synchronized with site copy and app metadata
- no required homepage deployment work remains from the scope-parity layout update

## Waiting On

- none for the current homepage scope-parity update

## Latest Proof Or Test Evidence

- source-copy alignment with GPT-MD commercial docs
- checkout URL now wired to the live Lemon product
- site price copy updated to `HK$88`
- public site structure expanded to include a dedicated pricing card and fuller commercial narrative
- public site now includes an Advantage section and proof panels for a closer PDF-MD-style layout
- 2026-04-24 marketing rewrite aligns the hero, workflow, proof, and pricing copy with the diagnosis from `2026-04-24_gptmd_pdfmd_marketing_diagnosis_from_chatgpt_pro_extended.md`
- startup, master-plan, and scope gates passed after repairing the site lane startup anchors
- static site structure review
- `git diff --check` passed after the 2026-04-24 landing-page edit
- 2026-04-24 grounded hero wiring used QA run `QA/runs/app-surface-qa/20260424_141602_surface-default` from the commercial QA lane; the harness passed 39/39 steps and produced a real app-window PNG capture at `site-assets/generated/gpt-md-app-workflow-window.png`.
- Local browser review served the site on `127.0.0.1:8766` and captured `site_visual_review/gpt-md-grounded-hero-wiring-1440.png`.
- 2026-04-24 scope-parity update passed `git diff --check`; local index asset reference check returned `missing []`; local browser review served the site on `127.0.0.1:8088` and captured desktop/mobile evidence at `site_visual_review/gpt-md-scope-parity-layout-1440.png` and `site_visual_review/gpt-md-scope-parity-layout-390.png`.
- GitHub Pages status returned `built`, and live HTML at `https://medschooloutsider.github.io/gpt-md-site/` contains the new `#why`, `#advantage`, `#specs`, and `data-proof-open` markers.

## Relevant Handoff Or Contract Files

- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/WORKSPACE_HANDOFF.md`
- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/docs/coordination/MASTER_PLAN.md`
- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/docs/commercialization/launch-readiness.md`
- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/docs/commercialization/site-copy.md`
- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/WORKSPACE_HANDOFF.md`
- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/APP_DEV_PORTFOLIO_LEDGER.md`

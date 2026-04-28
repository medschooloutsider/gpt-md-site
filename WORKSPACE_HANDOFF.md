# Workspace Handoff

Updated: 2026-04-28 21:29 CEST

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
- site commit `bea0aa6` tracks the eight showcase/spec PNGs that the expanded homepage references; GitHub Pages finished rebuilding and all 11 homepage image URLs now return HTTP 200
- correction commit `57a4a7a` removes the PDF-MD-derived `thymus`/spec/showcase assets from the GPT-MD homepage and untracks them from the public repo while leaving local files untouched
- copy/image alignment commit `75a655c` makes Specs text-only, limits homepage images to five GPT-MD generated/real app assets, and rewrites captions so they describe exactly what the image is: real app capture, generated workflow visual, or generated App Store composition
- `export-benchmarking.html` is now a buyer-facing proof page instead of an internal QA memo: it states the current checks, scope, weak-fit cases, live store state, and App Store Connect as the next proof slice
- the homepage proof popup is now a compact summary modal with four proof facts and scope boundaries; it no longer embeds the full proof page in an iframe

## Left To Do

- keep the live GPT-MD checkout URL, `HK$88` price, and support email synchronized with site copy and app metadata
- deploy the proof-page and proof-modal refresh to GitHub Pages, then verify the live `export-benchmarking.html` URL after Pages rebuilds

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
- 2026-04-24 broken image fix: direct live URL checks returned HTTP 200 for all 11 homepage images after commit `bea0aa6` and GitHub Pages rebuild.
- 2026-04-24 asset correction: direct live HTML/URL checks after commit `57a4a7a` confirmed no `specs/`, `showcase/routing`, `showcase/markdown`, or `thymus` image references remain; all 11 remaining homepage image URLs return HTTP 200. Fresh browser screenshot was not captured because the previous CDP lane on `127.0.0.1:59947` was no longer open.
- 2026-04-24 copy/image alignment: subagent audits classified safe assets and image-copy fit; after commit `75a655c`, GitHub Pages rebuilt and live parser checks confirmed 5 homepage images, all under `site-assets/generated/`, no PDF/thymus/spec/showcase bad refs, all image URLs HTTP 200, and zero `MarkEdit`/`PDF` text mentions on the homepage.
- 2026-04-28 proof refresh: `git diff --check` passed; local HTML asset-reference check returned `missing []` for `index.html` and `export-benchmarking.html`; local browser screenshots were captured at `site_visual_review/gpt-md-proof-page-redesign-1440.png`, `gpt-md-proof-page-redesign-390.png`, `gpt-md-proof-modal-redesign-1440.png`, and `gpt-md-proof-modal-redesign-390.png`; modal verification confirmed it opens and contains no iframe.

## Relevant Handoff Or Contract Files

- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/WORKSPACE_HANDOFF.md`
- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/docs/coordination/MASTER_PLAN.md`
- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/docs/commercialization/launch-readiness.md`
- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/apps/GPT-MD/qa-signoff/GPT-MD-commercial-qa/docs/commercialization/site-copy.md`
- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/Commercialisation_Hub/WORKSPACE_HANDOFF.md`
- `/Volumes/DATA_ARCHIVE/Hub_Network/20_App_And_Tool_Hubs/AppDev_Hub/APP_DEV_PORTFOLIO_LEDGER.md`

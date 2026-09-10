# GitHub Portfolio README Refresh Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Rebuild Ali Raza Memon's GitHub presence into a cohesive founder + full-stack developer + AI product builder portfolio by refreshing selected repository READMEs and then rebuilding the public profile README.

**Architecture:** Documentation-only changes across multiple repositories. Each repository README is treated as an independent portfolio artifact, grounded only in code/docs already present in that repository. The profile README is updated last so its project summaries stay consistent with the final project READMEs.

**Tech Stack:** GitHub Markdown, repository metadata, existing project stacks, Shields.io badges, one profile-only animated typing SVG service.

**Spec:** `docs/superpowers/specs/2026-09-11-github-portfolio-readme-design.md`

## Global Constraints

- Position the profile as **Founder • Full-Stack Developer • AI Product Builder**.
- Do not invent metrics, customers, revenue, partnerships, deployments, awards, certifications, or implemented features.
- Distinguish clearly between built, in progress, planned, and concept-stage work.
- Keep private/commercial repositories private; this plan changes documentation only.
- Never copy secrets, credentials, environment values, private customer data, or sensitive commercial strategy into README copy.
- Project READMEs remain static and professional.
- The public profile README may use exactly one tasteful animated typing element near the hero.
- Do not use cluttered GitHub-stat widget walls or excessive emoji/badges.
- CodeEq remains deferred until its repository is accessible through the connected GitHub account.

---

### Task 1: Refresh PakkOrder README

**Files:**
- Modify: `alixraza1001/pakkorder-backend/README.md`

**Interfaces:**
- Consumes: existing backend code, current README, package metadata, and routes/services already present.
- Produces: the canonical public-facing description of PakkOrder used later by the profile README.

- [ ] **Step 1: Re-fetch the current README and inspect package/code evidence**

Read `README.md`, `package.json`, `server.js`, and representative files under `src/routes` / `src/services` as needed. Confirm the implemented COD verification flow, WhatsApp integration, email confirmation, client dashboard, Firebase usage, and any seller/platform integration claims.

- [ ] **Step 2: Rewrite README with this exact section order**

1. `# PakkOrder`
2. One-line value proposition: COD order verification and ecommerce automation for Pakistani sellers.
3. `## Why PakkOrder` — explain the fake/unconfirmed COD order problem without unsupported market statistics.
4. `## What it does` — WhatsApp + email confirmation, confirm/cancel workflow, automated order handling, dashboard/integration capabilities only where code confirms them.
5. `## How the workflow works` — order received → confirmation request → customer response → order status update / timeout handling.
6. `## Core capabilities`
7. `## Architecture & tech stack`
8. `## Development setup`
9. `## Configuration` — retain environment-variable documentation but remove real-looking example secrets or anything that could be mistaken for a live credential.
10. `## Project status`
11. `## Background` — state that the initial product was developed with Claude as an AI-assisted development partner only if phrased as development history, not as a runtime dependency.

- [ ] **Step 3: Preserve useful operational setup below the portfolio sections**

Keep existing install, Meta webhook, Firebase, Railway, and troubleshooting guidance where still accurate, but place it after the product/architecture story so visitors understand the project before operational detail.

- [ ] **Step 4: Write the README and verify**

Update `README.md`, then immediately re-fetch it and confirm the top sections render in a coherent product-first order and contain no unsupported adoption/scale claims.

- [ ] **Step 5: Commit**

Use commit message: `docs: refresh PakkOrder README for portfolio presentation`.

---

### Task 2: Refresh Business AI Platform README

**Files:**
- Modify: `alixraza1001/business-ai-platform/README.md`

**Interfaces:**
- Consumes: current README plus existing product/architecture/implementation docs.
- Produces: a clearer internal-facing README and a high-level summary that can be referenced from the public profile without exposing source.

- [ ] **Step 1: Inspect current state and milestone evidence**

Read the existing README and current implementation/roadmap docs linked from it. Keep milestone wording aligned to what is actually merged on `main`.

- [ ] **Step 2: Rewrite README with this exact section order**

1. `# Business AI Platform`
2. One-line description: multi-tenant AI commerce/operations platform beginning with restaurants and WhatsApp.
3. `## Product vision`
4. `## Launch use case` — WhatsApp ordering, Q&A/support, sales assistance, human handoff, branch/restaurant operations only where current docs support the claim.
5. `## Platform foundations` — multi-tenancy, security, auth/RLS/audit foundations, modular provider integrations.
6. `## Architecture & technology direction`
7. `## Current implementation status`
8. `## Documentation map`
9. `## Development`
10. `## Confidentiality`

- [ ] **Step 3: Remove outdated milestone narration from the hero area**

Move task-by-task historical status deeper into `Current implementation status`; do not let old M0/M1 wording dominate the first screen.

- [ ] **Step 4: Preserve confidentiality intent**

Keep an explicit confidentiality section because the repository itself marks the project private/commercial. Do not surface private strategy in the public profile later.

- [ ] **Step 5: Write, re-fetch, and commit**

Commit message: `docs: make Business AI Platform README product-first`.

---

### Task 3: Refresh Jasarat Property Intelligence README

**Files:**
- Modify: `alixraza1001/jasarat-property-intelligence/README.md`

**Interfaces:**
- Consumes: existing source-acquisition implementation and tests.
- Produces: the canonical high-level project summary used by the profile README.

- [ ] **Step 1: Re-check implementation state**

Read the current README and current source-acquisition modules/tests. Confirm that acquisition/discovery exists and AI extraction/persistence/reviewer UI are not claimed as complete unless code now proves otherwise.

- [ ] **Step 2: Rewrite README with this exact section order**

1. `# Jasarat Property Intelligence`
2. One-line value proposition: turn Urdu newspaper property transaction notices into structured, searchable real-estate intelligence.
3. `## The problem`
4. `## What is implemented today`
5. `## Source acquisition pipeline`
6. `## Data extraction direction` — explicitly label AI extraction/review/search as in progress or planned according to repository evidence.
7. `## Reliability & validation`
8. `## Architecture & project structure`
9. `## Development commands`
10. `## Project status`

- [ ] **Step 3: Keep the high-resolution URL discovery detail, but move it below the product explanation**

Retain the `/mm/PAGE.jpg` vs `/sliderpics/` distinction because it demonstrates real source forensics, but do not let URL mechanics become the project's opening story.

- [ ] **Step 4: Write, re-fetch, and commit**

Commit message: `docs: refresh Jasarat Property Intelligence README`.

---

### Task 4: Create MakaanMetrics README

**Files:**
- Create: `alixraza1001/MakaanMetrics/README.md`

**Interfaces:**
- Consumes: `frontend` and `backend` code, package/requirements files, FastAPI metadata, Celery configuration, and existing app copy.
- Produces: the first proper project README and a concise profile summary.

- [ ] **Step 1: Inspect the real stack**

Confirm frontend framework, backend framework, database/auth approach, Redis/Celery usage, scraping/comparable-property flows, report generation, and deployment configuration from code before writing.

- [ ] **Step 2: Create README with this exact section order**

1. `# MakaanMetrics`
2. One-line description: property investment intelligence for the Pakistani real-estate market.
3. `## What it solves`
4. `## Product capabilities` — live/comparable listing analysis, reports, portfolio/watchlist/alerts only where repository code supports them.
5. `## How it works`
6. `## Architecture`
7. `## Tech stack`
8. `## Repository structure`
9. `## Local development`
10. `## Project status`

- [ ] **Step 3: Avoid overstating scraper coverage or data accuracy**

Describe integrations as implemented code paths, not guaranteed live coverage of every third-party site.

- [ ] **Step 4: Create, re-fetch, and commit**

Commit message: `docs: add MakaanMetrics project README`.

---

### Task 5: Create Waqtoro README

**Files:**
- Create: `alixraza1001/Waqtoro/README.md`

**Interfaces:**
- Consumes: storefront HTML/CSS/JS, Firebase modules/configuration, cart/account/review/checkout/order-tracking code.
- Produces: an ecommerce engineering case-study README.

- [ ] **Step 1: Inspect implemented storefront flows**

Confirm pages and modules for catalog, cart, wishlist, authentication/account, reviews, checkout, order tracking, and Firebase synchronization.

- [ ] **Step 2: Create README with this exact section order**

1. `# Waqtoro`
2. One-line description: responsive ecommerce storefront and customer-account experience for a watch retail concept.
3. `## Project overview`
4. `## Implemented experience`
5. `## Frontend architecture`
6. `## Firebase-backed features`
7. `## Tech stack`
8. `## Run locally`
9. `## Project status`

- [ ] **Step 3: Use neutral product wording**

Do not foreground or celebrate replica/counterfeit product positioning; the README should focus on the ecommerce software implementation.

- [ ] **Step 4: Create, re-fetch, and commit**

Commit message: `docs: add Waqtoro ecommerce project README`.

---

### Task 6: Refresh Asif Real Estate V2 README

**Files:**
- Modify: `alixraza1001/Asif-Real-EstateV2/README.md`

**Interfaces:**
- Consumes: Next.js/Supabase code and existing package metadata.
- Produces: a real project README replacing the default create-next-app text.

- [ ] **Step 1: Inspect implemented routes and data flows**

Confirm current property pages, contact/customer workflows, localization, Supabase usage, and any admin/content features before naming them.

- [ ] **Step 2: Replace README with this exact section order**

1. `# Asif Real Estate V2`
2. One-line description: digital real-estate platform for a Karachi property business.
3. `## Project goal`
4. `## Implemented features`
5. `## Tech stack`
6. `## Architecture / data layer`
7. `## Local development`
8. `## Project status`

- [ ] **Step 3: Write, re-fetch, and commit**

Commit message: `docs: replace default Asif Real Estate README`.

---

### Task 7: Create Verified Property README

**Files:**
- Create: `alixraza1001/Verified-Property/README.md`

**Interfaces:**
- Consumes: product vision, product principles, scope, route contracts, and architecture docs.
- Produces: a concise concept/architecture README that does not pretend planned verification features are already implemented.

- [ ] **Step 1: Determine current code-vs-doc status**

Read the root project metadata/code plus `docs/product/MASTER_PRODUCT_VISION.md`, `docs/product/V2_MVP_SCOPE.md`, `docs/product/PRODUCT_PRINCIPLES.md`, and `docs/architecture/SYSTEM_ARCHITECTURE.md`.

- [ ] **Step 2: Create README with this exact section order**

1. `# Verified Property`
2. One-line description: trust-focused Karachi property platform separating verified exact listings from agency-reported inventory.
3. `## Product thesis`
4. `## Core trust model`
5. `## Planned / implemented scope` — separate these explicitly.
6. `## Architecture direction`
7. `## Product principles`
8. `## Documentation`
9. `## Project status`

- [ ] **Step 3: Create, re-fetch, and commit**

Commit message: `docs: add Verified Property project README`.

---

### Task 8: Refresh Personalized Tracker README

**Files:**
- Modify: `alixraza1001/Personalized-tracker/README.md`

**Interfaces:**
- Consumes: actual app pages/components and package metadata.
- Produces: a README describing the tracker itself instead of the AI Studio scaffold.

- [ ] **Step 1: Inspect the actual application behavior**

Read package metadata, app entry points, and user-facing components. Identify the tracker domain, main flows, persistence model, and any AI behavior actually present.

- [ ] **Step 2: Replace scaffold README with this exact section order**

1. Project name from the actual product UI
2. One-line description of what the tracker does
3. `## Overview`
4. `## Features`
5. `## Tech stack`
6. `## Run locally`
7. `## Project status`

Do not preserve generic "Run and deploy your AI Studio app" copy unless it remains directly useful as a development note.

- [ ] **Step 3: Write, re-fetch, and commit**

Commit message: `docs: replace AI Studio scaffold README`.

---

### Task 9: Clean Academic README Presentation

**Files:**
- Modify: `alixraza1001/24K-0747/README.md`
- Modify: `alixraza1001/DBS_Project/README.md`
- Modify if useful and meaningfully distinct: `alixraza1001/DBS_Project_v2/README.md`

**Interfaces:**
- Consumes: existing coursework contents.
- Produces: concise, accurate academic README pages that no longer distract from the professional portfolio.

- [ ] **Step 1: Inspect each academic repository's real purpose**

Identify course/project context from code and files. Do not infer course names that are not present.

- [ ] **Step 2: Replace personal-introduction / placeholder copy**

Use a compact structure: project title, course/context if known, what the repository contains, technologies/concepts demonstrated, and how to run where relevant.

- [ ] **Step 3: Keep these READMEs intentionally shorter than flagship projects**

Do not add startup-style marketing language, animations, or large badge sections.

- [ ] **Step 4: Write, re-fetch, and commit each repository independently**

Use repository-specific `docs:` commit messages.

---

### Task 10: Rebuild Public Profile README

**Files:**
- Modify: `alixraza1001/alixraza1001/README.md`

**Interfaces:**
- Consumes: final canonical summaries from Tasks 1–9 plus confirmed personal details.
- Produces: the public GitHub profile landing page.

- [ ] **Step 1: Replace the PakkOrder-only positioning**

Use the hero identity:

`Ali Raza Memon — Founder • Full-Stack Developer • AI Product Builder`

Follow with a short line about building software at the intersection of AI, commerce, property technology, and business operations.

- [ ] **Step 2: Add exactly one animated typing element**

Use a GitHub-compatible SVG typing banner with short phrases such as:
- `Building products that solve real business problems`
- `Full-stack software • AI systems • automation`
- `From idea to shipped product`

Keep animation only in the hero area. No other animated widgets.

- [ ] **Step 3: Add concise About section**

Include:
- Founder/CEO of Hexium Global
- BS Computer Science at FAST-NUCES Karachi (2024–2028)
- Product-building interests across AI SaaS, ecommerce, real estate/property intelligence, and automation
- No GPA and no fake certifications

- [ ] **Step 4: Add Featured Projects section**

Use a clean Markdown table/cards-style layout with these entries in this order unless final repository evidence suggests a better sequence:
1. PakkOrder — link if public at implementation time; otherwise present as private project text.
2. Business AI Platform — private project, description only.
3. Jasarat Property Intelligence — private project, description only.
4. MakaanMetrics — private project, description only.
5. Waqtoro — link if public at implementation time; otherwise description only.
6. Asif Real Estate V2 — private project, description only.
7. Verified Property — private project, description only.

Add CodeEq near the top only after its repository becomes accessible.

- [ ] **Step 5: Add grouped Tech Stack**

Only include technologies confirmed by project/user evidence. Organize into:
- Languages
- Frontend
- Backend & APIs
- Data & Auth
- AI & Automation
- Product / Dev Tools

Use restrained Shields.io badges or compact inline icons. Avoid one giant unstructured badge wall.

- [ ] **Step 6: Add Founder / Product Work, Education, and Contact**

Education copy:
- FAST-NUCES Karachi — BS Computer Science, 2024–2028
- The City School — O Levels & A Levels, A Levels completed 2024

Contact:
- LinkedIn: `https://www.linkedin.com/in/ali-raza-b25b19371/`
- Email: `ali.xraza.1001@gmail.com`
- GitHub: `@alixraza1001`

- [ ] **Step 7: Remove old narrow claims**

Delete outdated copy that frames the account only around scaling PakkOrder or only around Node/Firebase/Shopify.

- [ ] **Step 8: Write, re-fetch, visually sanity-check Markdown structure, and commit**

Commit message: `docs: rebuild GitHub profile as founder developer portfolio`.

---

### Task 11: Final Cross-Repository Verification

**Files:**
- Verify all READMEs changed in Tasks 1–10.

**Interfaces:**
- Consumes: final GitHub-renderable Markdown from all edited repositories.
- Produces: verified portfolio documentation with consistent positioning.

- [ ] **Step 1: Re-fetch every changed README**

Confirm each file exists on the default branch and contains the intended top-level sections.

- [ ] **Step 2: Run an accuracy consistency pass**

Check that the profile README does not claim anything stronger than the project README or repository evidence.

- [ ] **Step 3: Run a privacy pass**

Search edited copy for credentials, token-like values, internal customer data, or confidential implementation/business details. Remove anything questionable.

- [ ] **Step 4: Run a presentation pass**

Confirm:
- exactly one animation exists, only on the profile README;
- project READMEs are static;
- no fake certification section exists;
- private repos are not accidentally exposed through source links;
- public links resolve only to repos that are public at verification time;
- old placeholder/default framework README text is gone where replaced.

- [ ] **Step 5: Report completion with repository-by-repository commit SHAs and any deferred items**

Explicitly list CodeEq as deferred if it remains inaccessible.

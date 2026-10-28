# Research Repro — Computational Observatory

Local interactive concept website based on selected visual direction 2.

Preview: http://127.0.0.1:4173/

## Included

- Custom brand mark, favicon and generated evidence artwork.
- Dark observatory hero, light figure comparison, evidence map, failure taxonomy and reviewer workbench.
- Lenis smooth scrolling, GSAP reveals/parallax and a pinned horizontal product gallery on suitable desktop viewports.
- Reduced-motion support and a motion toggle; ordinary grid fallback on mobile and with motion disabled.
- Five separate product pages: Research Desk, Research Review, Research Proof, Research Signal and Research Report.
- Platform, capabilities, problem, solutions/personas, pricing, pilot, resources, company, trust, ecosystem, evaluation, contact, privacy, terms, accessibility and sign-in preview pages.
- Ten fictional study records, search/filter queue, evidence source pane, editable local reviewer notes and downloadable illustrative JSON reports.

## Truth boundary

This is a frontend concept preview, not an operating research platform. No research code runs. There is no real authentication, payment, analytics collection, manuscript upload, external communication or form delivery. Notes last only in the current record view. Forms validate locally and explicitly say nothing was sent. All data and images are illustrative. The proposed $1,000 ten-submission pilot is a pricing hypothesis. It is not an accepted rate or checkout.

The current first-pilot scope is a non-executing artifact completeness audit. Environment execution, comparison and preservation are proposed directions with separate gates. Same-data computational reproducibility is distinguished from independent scientific replication. Failed or missing artifacts do not imply misconduct.

## Project

React + Vite, React Router, GSAP/ScrollTrigger, Lenis, Recharts and Phosphor icons. Self-hosted Manrope Variable and IBM Plex Mono. Font license copies are in `licenses/`.

Run locally: `npm install`, then `npm run dev -- --host 127.0.0.1 --port 4173`.
Build: `npm run build`. Hosting-package checks: `npm run test:sites`.

The running preview has already been started. The prepared build is in `dist/`; nothing has been deployed or connected to researchrepro.com.

## Review artifacts

- `desktop-home.jpg`: 1440×900 homepage.
- `desktop-audit.jpg`: 1440×900 RA-009 workbench.
- `mobile-home.jpg` and `mobile-audit.jpg`: 390×844 captures.
- `desktop-full.jpg`: full homepage with motion disabled.
- `visual-target.jpg`: selected visual direction.
- `qa-hero-comparison.jpg` and `qa-detail-comparison.jpg`: side-by-side visual comparisons.
- `design-qa.md`: QA evidence and limitations.
- `synthetic-fixtures.json`: fictional records, manifest, taxonomy and graph values.

## Before a public launch

Connect an approved form destination and consent-aware analytics; implement real identity only if needed; verify company/domain ownership and approved legal copy; measure production performance and accessibility; configure hosting and DNS. No public launch, live service, customer commitment or security certification is claimed here.

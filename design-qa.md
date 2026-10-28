# Research Repro design QA

final result: passed

Scope: frontend concept-preview handoff. This result does not certify a production research execution system or deployed website.

## Source and evidence

- Source visual truth: `visual-target.jpg`, copied from the selected Computational Observatory generated direction. Source pixels: 941×1672.
- Implementation: http://127.0.0.1:4173/ and /demo/studies/ra-009.
- Desktop viewport: 1440×900 CSS px, device scale factor 1. Captures: `desktop-home.jpg`, `desktop-audit.jpg`.
- Mobile viewport: 390×844 CSS px, device scale factor 1. Captures: `mobile-home.jpg`, `mobile-audit.jpg`.
- Full homepage: `desktop-full.jpg`, motion disabled so all explanatory sections are visible.
- Full hero comparison: `qa-hero-comparison.jpg`, source and implementation normalized to equal widths in one image.
- Focused comparison: `qa-detail-comparison.jpg`, figure-comparison and four-column workbench regions normalized to 850px widths. The record-view title differs from the homepage source; only the shared workbench component is compared.

## Intentional adaptations

The reference is an art-direction board, not a fully specified product. Its gene-expression/dose-response labels and inconsistent module descriptions were corrected to the user's computational social science brief. The final fictional example is participation versus commute duration. The native editable workbench replaces a static screenshot. Native chart/table content supports meaningful evidence inspection. The site adds the full page architecture and explanatory sections absent from the short board.

The visual identity retains the dark green observatory, mint connections, amber missing-lockfile cue, translucent evidence planes, square fine-bordered panels, light comparison surface, dense dark four-column workbench and large restrained typography. Desktop whitespace is more generous than the compressed reference board. A permanent disclosure strip and expanded navigation are intentional additions. Small module symbols use the Phosphor icon library; custom hero/support illustrations remain generated raster assets.

## Findings and iteration history

- [P1 — fixed] Navigating away from a GSAP-pinned gallery could conflict with React removing the pinned node. A stable parent now owns the section. Retested homepage → demo → queue → record → report → pilot and return navigation without new console errors.
- [P2 — fixed] Initial desktop hero was too tall and imagery competed with type. Reduced artwork height and adjusted grid/spacing. `desktop-before.jpg` records the earlier state; `desktop-home.jpg` and the combined hero comparison show the revised composition.
- [P2 — fixed] Mobile hero word overflow and horizontal reveal offsets exceeded the 390px viewport. Responsive display size and vertical-only mobile reveals fix this. DOM checks report 390px document width at 390px viewport on homepage and audit.
- [P2 — fixed] Motion-disabled desktop gallery retained a horizontal strip. It now shows all five modules in a three-column grid; mobile becomes one column. Browser geometry confirmed every card within the desktop content width.
- [P2 — fixed] Trailing slash on the company route caused content lookup failure. Normalized editorial content lookup and verified the Company heading.
- [P2 — fixed] Disclosures scrolled out of view. The concept/synthetic/non-executed strip now remains sticky below navigation, including mobile.
- Font import resolution failure was corrected before final build; this was implementation troubleshooting, not a visual comparison pass.

## Required fidelity surfaces

- Typography: self-hosted Manrope Variable provides the geometric display style; IBM Plex Mono differentiates artifact/status metadata. Hero wraps correctly on desktop and mobile. Native workbench text is sharp and editable. Source board's compressed text density is deliberately relaxed.
- Spacing/layout: hero two-column balance, light figure comparison and dark workbench hierarchy checked in combined images. Four workbench panes align at desktop; mobile stacks source and reviewer content. Tables scroll within their own containers.
- Colors/tokens: deep green #101713, pearl #eef1ec, mint #b5d6c2, amber #d6aa64. Amber denotes blockers; status text accompanies color. Light/dark alternation matches the chosen direction.
- Images: generated glass evidence panels, matching supporting artwork and custom raster brand mark are crisp at target viewports. No screenshot is used in place of interactive product UI. Social-science content intentionally differs from the initial reference.
- Copy/content: five offers and hypothesis pricing retained. NOT EXECUTED, license blocker, simulated execution error and simulated mismatch are distinguished. No customer logos, acceptance, live integrations or measured ROI are invented.

## Functional checks

Passed desktop navigation and Escape dismissal, mobile navigation, all five product routes, platform, solutions, pricing, resources, pilot protocol, company, trust and sign-in preview. Checked horizontal-gallery navigation and motion-off grid. Queue search for RA-009 returned exactly one matching record. Saved a synthetic reviewer note and observed local confirmation. Illustrative JSON report download was prepared. Pilot form accepted fictional valid inputs and displayed explicit no-transmission confirmation. Desktop and mobile workbench screenshots captured. New console errors after the fixes: none observed during the smoke-test flow.

`npm run build` passes. `npm run test:sites` passes 4 tests. Ten fixture counts agree with the queue: 3 audit-complete, 3 pending, 2 blocked, 2 rejected. Actual research executions: zero.

## Residual follow-up / test gaps

- [P3] Split the 865kB uncompressed JS bundle and measure production performance before deployment. Build currently reports a chunk-size advisory.
- Formal screen-reader, cross-browser, text-zoom and automated contrast audits remain for production readiness. Keyboardable controls, labels, chart data table, visible focus and reduced-motion fallbacks are present, but this is not a WCAG certification.
- Forms/authentication are deliberately disconnected. No end-to-end backend, security-isolation or research execution tests apply to this frontend concept.

No remaining actionable P0/P1/P2 issues were found in the scoped visual and primary-flow review.

## Hover refinement — 28 October 2026
Added pointer-gated tonal button states, directional action arrows, card border/elevation feedback, navigation underlines, evidence-node highlights, tab/filter feedback, row tracking, input borders and disclosure header feedback. Cards stay straight and stationary. Disabled buttons do not animate. OS reduced-motion and the existing motion toggle suppress transitions. Keyboard card focus was verified in the browser: amber 2px outline and green inset edge. Screenshot: interaction-focus.jpg. Desktop document width remained 1440px. Build passed. Pointer hover styles were reviewed in CSS; automated pointer-hover simulation was unavailable in this browser API.

Research references: [Carbon motion](https://www.carbondesignsystem.com/building-blocks/foundations/motion/overview), [Material states](https://m3.material.io/foundations/interaction/states/applying-states), [MDN hover](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media/hover), [MDN focus-visible](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:focus-visible), [WCAG](https://www.w3.org/TR/WCAG22/). These informed the interaction approach; the exact palette and 160–220ms timings are project design choices.

## Continuity identity update
Selected option 01 rebuilt as editable vector paths, with outlined Manrope lettering. 21 SVG files parsed successfully and contain no image or text elements. Favicon PNG family rendered with resvg at 16–512px; ICO includes 16/32/48px. Header/footer now use the pearl horizontal SVG. Original angled homepage hero restored from hero-evidence.png; supporting illustrations remain straight. Browser capture: continuity-home.jpg at 1440×900. Fresh mobile load reports 390px document width at 390px viewport. Build passed. The vector reconstruction preserves the mirrored RR and curved seam while regularizing geometry; it is not a pixel-exact bitmap trace.

## Atmospheric backgrounds and shutter interactions
User-requested change from flat surfaces: generated organic forest/bronze and pearl/sage textures applied across marketing and demo sections, with overlays for readability. No new striped, grid or checked background treatments. Original angled hero artwork remains and is blended into the texture.

Button label flip uses two visual layers; duplicate is aria-hidden. Shutters are pseudo-element paint layers, preserving card geometry and hit targets. Different card directions reveal jade or champagne. Focus receives the same color fill, and OS reduced-motion / motion toggle removes transition motion.

Browser verification: hovered report-export button had front label opacity 0, back label opacity 1, shutter identity transform; export confirmation still worked. Focused product card had champagne fill, shutter identity transform and card transform none. Desktop capture atmosphere-home.jpg and card-state capture shutter-card.jpg. Fresh mobile homepage had document width 390 at viewport 390. Production build passes (existing JS chunk advisory remains).

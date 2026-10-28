# Prototype Instructions

Run the local server yourself and open the preview in the browser available to this environment. Do not give the user server-start instructions when you can run it.

Before making substantial visual changes, use the Product Design plugin's `get-context` skill when the visual source is unclear or no longer matches the current goal. When the user gives durable prototype-specific design feedback, preferences, or decisions, record them in `AGENTS.md`.

When implementing from a selected generated mock, treat that image as the source of truth for layout, component anatomy, density, spacing, color, typography, visible content, and hierarchy.

Build app UI in `src/`. Keep `.openai/hosting.json`, `worker/index.js`, `scripts/prepare-sites-build.mjs`, and `tests/sites-worker.test.mjs` intact so the same local prototype can be handed to Sites. Before a Sites handoff, run `npm run build` and `npm run test:sites`; the build must leave `dist/client/index.html`, `dist/server/index.js`, and `dist/.openai/hosting.json`.

User design preference: keep UI cards and supporting illustration panels straight. Explicit exception: homepage hero must retain the original angled glass panels (hero-evidence.png). Selected logo: Continuity option 01; use vector masters in assets/continuity.

Visual refinement: use expressive shutter color reveals on interactive cards/buttons and flip-label motion on primary actions. Keep card geometry straight. Backgrounds should use organic grain, atmospheric ink/light and paper texture; never add stripes, grids or checked patterns. Preserve original angled hero artwork.

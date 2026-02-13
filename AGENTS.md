# Agent Guide (Docusaurus Template)

## Project snapshot
- Framework: Docusaurus 3 (classic preset), React 19, TypeScript.
- Structure: docs + static assets + src pages/components.
- Theme: Infima defaults with green primary palette.
- Homepage: hero banner + three feature cards with SVGs.

## Key files
- `docusaurus.config.ts`: site metadata, navbar/footer, theme, presets.
- `src/pages/index.tsx`: homepage layout and hero CTA.
- `src/components/HomepageFeatures/index.tsx`: feature cards content.
- `src/css/custom.css`: global theme variables.
- `docs/`: documentation content.
- `static/`: images and public assets.

## Content feel
- Friendly, starter-template tone ("My Site", "Dinosaurs are cool").
- Clean, content-first layout; simple hero + feature grid.
- Green accent color; light theme by default with dark mode palette.

## Common commands
- `yarn start`: local dev server.
- `yarn build`: production build to `build/`.
- `yarn serve`: serve the build output.
- `yarn typecheck`: TypeScript checks.

## Notes for agents
- Prefer editing content in `docs/` for copy changes.
- Homepage visuals are driven by `src/pages/index.tsx` and
  `src/components/HomepageFeatures/index.tsx`.
- Global theming tweaks go in `src/css/custom.css`.

## Patch path safety (Windows)
- For `apply_patch`, always use workspace-relative paths (for example `package.json`), never absolute Windows paths like `D:\thegioitienhiep\package.json`.
- Do not include drive letters (`D:`) in `*** Update File:`, `*** Add File:`, or `*** Delete File:` headers.
- If a tool returns an absolute path, convert it to a repo-relative path before building the patch header.

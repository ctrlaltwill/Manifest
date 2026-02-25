# Manifest (Fork)

Personal fork of the original Manifest/Baseline Obsidian theme, maintained for custom UI refinements.

## Purpose of this fork

This repository is focused on a stable, opinionated visual variant of the original theme.

- Keep behavior and features intact
- Preserve compatibility with upstream theme structure
- Maintain a single canonical CSS output for personal use

## Source of truth

The guiding stylesheet for this fork is:

- `src/theme.scss` (contains full canonical CSS text)

Build output is written to:

- `theme.css`

In this fork, the build process intentionally performs a direct copy from `src/theme.scss` to `theme.css` to avoid parser-driven transformations and preserve exact styling.

## Build docs

### Requirements

- Node.js 18+ (recommended)
- npm

### Install

```bash
npm install
```

### Build

```bash
npm run build
```

This updates `theme.css` from `src/theme.scss` with no style/functionality changes.

## Visual changes in this fork

Primary visual differences from upstream are concentrated in:

- **Typography**
  - Font sizing/weight/spacing refinements for better readability and hierarchy
- **Button styling**
  - More consistent corner radii, hover fills, and interaction states
- **Navigation layout**
  - Sidebar/tab layout refinements for spacing, active-state clarity, and alignment
- **Image styling**
  - Visual adjustments around image presentation to better match the fork’s design language

## Repository structure (relevant files)

- `src/theme.scss` — canonical style source used by this fork
- `theme.css` — distributed Obsidian theme stylesheet
- `manifest.json` — Obsidian theme metadata
- `snippets/` — optional CSS snippets

## Updating from upstream

When syncing upstream changes:

1. Merge/rebase upstream changes into this fork.
2. Re-apply any intentional customizations in `src/theme.scss`.
3. Run `npm run build`.
4. Validate visual parity in Obsidian.

## License

This fork follows the original project license: see `LICENSE.txt`.

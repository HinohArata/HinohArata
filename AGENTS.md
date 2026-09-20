# AGENTS.md

## What this repo is

GitHub profile repository (`github.com/HinohArata/HinohArata`). There is no code: `README.md` renders directly on the public profile page, and `banner.svg` is a local asset referenced at the top of it. Any push to `main` instantly changes the live profile.

## Facts an agent will otherwise miss

- No package manager, build, test, lint, or CI tooling exists anywhere in the repo. There is nothing to run to verify changes — review the rendered HTML/markdown manually.
- `README.md` mixes HTML and markdown — `<table>` rows are used to lay out card grids and `<div align="center">` to stack inline badges. When editing, keep the two-column card layouts intact or badge rows overflow on mobile.
- `banner.svg` is a rendered `README.md` asset with SMIL animations (pulsing orbs, blinking cursor, self-drawing line). When editing it, keep animations valid — a broken SVG breaks the whole header.
- `arata.png` (profile asset) sits in the repo but is **not referenced** by `README.md`; do not assume it is used or delete it.
- Opening a PR is not possible for this repo (single user, profile repo). Work is committed directly on `main` and pushed.
- Commit message style in history is terse, e.g. `update profile`, `Update README.md` — follow that.
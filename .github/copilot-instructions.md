## Purpose
Provide concise, actionable guidance for AI coding agents working in this repository.

## Repo Snapshot
- Single-page static website: primary file is `index.html` at the repository root.
- `index.html` links to `styles.css` (not present in the repo snapshot) and uses simple anchor navigation (`#section1`, `#section2`, `#section3`).

## Big Picture
- This is a minimal static site: no build system, package manager, or backend services detected.
- Changes are typically small edits to HTML/CSS/JS. Agents should not add heavy dependencies without explicit instruction.

## Key Files and Patterns
- `index.html`: main entry — update content, navigation, and metadata here.
- `styles.css` (referenced from `index.html`): style file expected at repo root — check for it before creating duplicates.

## Developer Workflows (discovered / recommended)
- Serve locally with Python (works cross-platform):

  ```powershell
  python -m http.server 8000
  ```

- Alternatively use `npx http-server . -p 8000` if Node.js is available.
- There are no tests or build steps to run in this snapshot. If you add a toolchain, update this file with exact commands.

## Project-specific Conventions
- Keep the site static and dependency-free unless the repo owner requests a frontend framework.
- When adding files, prefer small, focused changes (e.g., a new `styles.css` or a `scripts/` folder) and include a short README describing the new workflow.

## Integration Points & External Dependencies
- No external services, APIs, or CI workflows detected. If you add integrations (APIs, CDNs, CI), document configuration and secrets handling here.

## How to Edit / PR Guidance
- Make minimal changes per PR. For content edits to `index.html`, update only the relevant section and add a short PR description: what changed and why.
- If adding a build system or tests, include a migration note and `README.md` updates describing commands and expected environment.

## When to Ask for Clarification
- If a requested change implies adding dependencies, a runtime, or CI, ask the repo owner before implementing.
- If multiple pages or components are needed, confirm desired directory structure and deploy target.

## Example Tasks (how an agent should proceed)
- Small content update: edit `index.html`, run `python -m http.server 8000`, verify navigation anchors work.
- Add stylesheet: create `styles.css` at root, update `index.html` link, and include a one-paragraph `README.md` describing usage.

If anything here is unclear or you want this expanded (e.g., add CI, tests, or a scaffold), tell me which direction and I will update this file.

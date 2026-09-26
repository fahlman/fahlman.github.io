# fahlman.github.io — Repository Instructions

Read with the shared `AGENTS.md`. No previous repository agent guide was present.

## Site and source

- Static project website in `fahlman/fahlman.github.io`, served at
  `code.fahlsing.com` as recorded in `CNAME`.
- `index.html` contains the page and its inline CSS; `assets/`, `favicon.ico`,
  `CNAME`, and `.nojekyll` are the published supporting files.
- This is an HTML/CSS website, not a Swift/macOS application. Preserve its
  existing static architecture; the shared SwiftUI/toolchain defaults do not
  call for adding an application framework or build dependency.

## Verification and publication

- Inspect changed content, links, asset paths, and responsive browser rendering.
  No local package-based build or automated test command is declared.
- Read `.github/workflows/` before publishing. The Pages workflow copies the
  site files into `_site`, uploads them, and deploys to GitHub Pages.
- A push to `main` or a manual workflow dispatch deploys the website. Treat that
  as publication, not an ordinary branch update; follow the shared authorization
  rules before taking either action.

## Toolchain applicability

This is a static HTML/CSS site. A Swift compiler, Swift language mode,
Apple SDK, and macOS deployment target do not apply. Preserve the existing
static-site and GitHub Pages workflow.

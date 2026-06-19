# Changelog

All notable changes to Idexal Code are documented here.
This project follows [Semantic Versioning](https://semver.org).

## [1.0.1] — 2026-06-19

The first public distribution build — installers are now published to the public
[idexal/idexal-code](https://github.com/idexal/idexal-code) repository for download.

### Changed

- **Two-repo distribution** — the private repo builds; the public
  `idexal/idexal-code` repo distributes the downloadable installers and receives
  auto-updates. Documented in `DISTRIBUTION.md`.

### Fixed

- **Agents overview now shows each agent's model** (it previously always showed
  "default model" due to a value-shape mismatch).
- Type-soundness fixes across the per-agent models, agents panel, and multi-agent
  tasks views.

## [1.0.0] — 2026-06-18

The first production release of **Idexal Code** — a professional desktop
coding-agent experience by Idexal.

### Added

- **Multi-model support with automatic fallback** — pick any model from any
  connected provider, and configure a fallback that engages automatically when a
  model fails or runs out of credits, with no interruption.
- **Per-agent models** — assign any model (and its own fallback) to any agent,
  from Settings → General → Agent models.
- **Multi-agent tasks** — launch one goal across several agents at once; each runs
  in its own session, in parallel, with live status (starting → running → done)
  tracked from a single panel. Opened via the "Tasks" button.
- **Inline autocomplete** — Copilot-style ghost text drawn from your prompt
  history; `Tab` to accept, `Esc` to dismiss. Toggle in Settings.
- **Aurora design system** — a cohesive Idexal dark theme: glass surfaces, an
  animated composer border, gradient accents, branded scrollbars, and a living
  backdrop.
- **About Idexal Code** dialog with version, company, founder, and support links.
- **Branded Windows installer** — an advanced NSIS setup wizard (welcome →
  license → install location → finish) with the Idexal logo and license.
- **Release pipeline** — a GitHub Actions workflow that builds and publishes the
  installer on a version tag.

### Notes

- Idexal Code builds on the open-source [OpenCode](https://github.com/anomalyco/opencode)
  engine (MIT) and extends it with the features above and the Idexal experience.

[1.0.1]: https://github.com/idexal/idexal-code/releases/tag/v1.0.1
[1.0.0]: https://github.com/idexal/idexal-code/releases/tag/v1.0.0

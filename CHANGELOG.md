# Changelog

All notable changes to this project are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.3.2] - 2026-11-03

### Fixed

- `.badge` sizes to its label (`width: fit-content`), including inside the preview type grid.
- Radius swatches in `preview.html` are boxes, so each corner radius is visible. The space scale is unchanged.

## [0.3.1] - 2026-11-03

### Changed

- `preview.html` sample client and person labels are placeholders. No token or component changes.

## [0.3.0] - 2026-11-02

### Added

- Optional controls in `components.css`: `.toast`, `.dialog`, `.menu` (with `.menu-head`, `.menu-sep`, `.menu-label`, `.menu-item`), `.picker`, `.stepper`, `.segmented`, `.chip`, `.icon-btn`, `.search`, `.filter-bar`, `.link-btn`, `.count`, `kbd`, `.btn.sm`, `.btn.lg`, and field help, error, and focus states. Tokens are unchanged. Shell, tables, navigation, and the account cluster are not included.

## [0.2.0] - 2026-11-02

### Added

- `components.css`: optional classes `.btn.primary`, `.btn.secondary`, `.btn.ghost`, `.btn.danger`, `.btn.danger-ghost`, `.input`, `.badge` (status and identity variants), and `.banner` (info, warning, danger). Primary is brand black. Focus stays the charcoal ring. Tokens are unchanged.

## [0.1.1] - 2026-11-02

### Added

- `preview.html`: a static gallery of the tokens. It is a preview, not a published component API. No token changes.

## [0.1.0] - 2026-11-02

### Added

- `tokens.css`: brand peach `#e18972`, brand black `#1e1e1e` for text and action, Vivid Blue `#186aea` for links and info, and a charcoal (brand black) focus ring.
- Role tokens for background, text, border, action, focus, type, space, radius, control heights, and row heights.
- Product-extension tokens, named as extensions: warm gray ramp, success / warning / danger, peach washes, and the four-step heat ramp.
- `tokens.md` describing each token and which values are brand versus product extension.
- `brand/README.md` with the guidelines colors, the Poppins decision, and the logo clear-space rule. No logo files.

Peach is identity only. It is not a button fill.

This version does not include components, font files, PDF styles, share-page styles, or email styles.

[0.3.2]: https://github.com/Martech-Mission/martech-design-system/releases/tag/v0.3.2
[0.3.1]: https://github.com/Martech-Mission/martech-design-system/releases/tag/v0.3.1
[0.3.0]: https://github.com/Martech-Mission/martech-design-system/releases/tag/v0.3.0
[0.2.0]: https://github.com/Martech-Mission/martech-design-system/releases/tag/v0.2.0
[0.1.1]: https://github.com/Martech-Mission/martech-design-system/releases/tag/v0.1.1
[0.1.0]: https://github.com/Martech-Mission/martech-design-system/releases/tag/v0.1.0

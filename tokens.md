# Tokens

`tokens.css` is the only runtime file in v0.1.0. There is no build step. Apps copy that file from a git tag. See the README for the copy path.

Components use the role tokens (`--text`, `--border`, `--action`, `--bg-app`, and the rest of that group). They do not read raw `--gray-*` values. A brand change then stays in this file.

Peach (`--brand`) is identity only: the logo, an active-nav mark, an avatar wash. It is not a button fill and not a status color. Primary actions use `--action`, which is brand black.

## Brand

These four values are Brand Guidelines V1.0. CMYK is recorded in `brand/README.md`.

| Token | Hex | Use |
| --- | --- | --- |
| `--brand`, `--brand-500` | `#e18972` | Martech Peach. Identity only. |
| `--text`, `--action` | `#1e1e1e` | Brand black. Body text and the primary button. |
| `--info`, `--link`, `--info-700` | `#186aea` | Vivid Blue. Links and info. |
| `--gray-0`, `--bg-surface` | `#ffffff` | White. Page surfaces. |

`--focus-ring` is 2px white plus 2px brand black, so a focused control does not look like an error and does not use Vivid Blue.

`--brand-50` (`#fdf1ed`), `--brand-100` (`#f9ddd3`), and `--brand-700` (`#a84a32`) are product-extension washes and ink from the timesheets proposal. They sit next to peach for tints. They are not extra brand colors.

`--action-hover` (`#161616`) is a product-extension press state, darker than brand black.

## Product extensions

Not brand colors. They exist so app UI can show state and density without spending peach or Vivid Blue on status.

### Warm gray ramp

| Token | Hex | Typical role |
| --- | --- | --- |
| `--gray-0` | `#ffffff` | `--bg-surface` |
| `--gray-25` | `#fbfaf9` | `--bg-app` |
| `--gray-50` | `#f6f4f2` | `--bg-subtle` |
| `--gray-100` | `#eeebe8` | `--bg-hover` |
| `--gray-200` | `#e3dfdb` | `--border` |
| `--gray-300` | `#cfcac4` | `--border-strong` |
| `--gray-500` | `#8a847e` | `--text-faint` |
| `--gray-600` | `#6b6560` | `--text-muted` |
| `--gray-800` | `#3a3632` | Ramp only. No role token points here in v0.1. |
| `--gray-900` | `#2b2b2b` | Ramp only. This is not brand black and not `--text`. |

### Status

| Token | Hex | Meaning |
| --- | --- | --- |
| `--success-50` | `#e8f4ec` | Success wash |
| `--success-700` | `#1f7a4a` | Success ink |
| `--warning-50` | `#fff6e0` | Edited / warning wash |
| `--warning-300` | `#ecc66a` | Edited border |
| `--warning-700` | `#8a5a00` | Warning ink |
| `--danger-50` | `#fdecea` | Danger wash |
| `--danger-700` | `#b42318` | Danger ink |
| `--info-50` | `#eaf1fc` | Info wash behind Vivid Blue |

### Heat ramp

One blue hue, four steps, for density shading such as a pivot cell. More ink means more of the measured thing.

| Token | Hex |
| --- | --- |
| `--data-1` | `#eef2f9` |
| `--data-2` | `#dbe4f3` |
| `--data-3` | `#c3d2ec` |
| `--data-4` | `#a6bce2` |

## Type

`--font-ui` and `--font-brand` both name Poppins, with a system sans-serif fallback. This repo does not ship font files. WS Paradose and Inter are not tokens. See `brand/README.md` for why Paradose is absent.

| Token | Value | Use |
| --- | --- | --- |
| `--text-xl` / `--lh-xl` | 20px / 28px | Page titles. Weight 600. |
| `--text-lg` / `--lh-lg` | 16px / 24px | Section titles. Weight 600. |
| `--text-base` / `--lh-base` | 14px / 22px | Body, menus. |
| `--text-md` / `--lh-md` | 13px / 20px | Tables and controls. Tabular numerals. |
| `--text-sm` / `--lh-sm` | 12px / 16px | Labels, column headers, help. |
| `--text-xs` / `--lh-xs` | 11px / 16px | Badges, keyboard hints. |
| `--font-mono` | ui-monospace, SF Mono, Consolas | Code only. |

## Space, shape, size

| Token | Value | Use |
| --- | --- | --- |
| `--space-1` … `--space-8` | 4, 8, 12, 16, 20, 24, 32px | Gaps and padding. No step named `--space-7`. |
| `--control-sm` / `--control-md` / `--control-lg` | 28 / 32 / 40px | In-table controls, every input and button, large targets. |
| `--row-comfortable` / `--row-compact` | 36 / 30px | Data-table row height. |
| `--radius-sm` / `--radius-md` / `--radius-lg` / `--radius-full` | 4 / 6 / 10 / 999px | Keys, controls, cards and menus, pills and avatars. |
| `--shadow-popover` | one shadow, brand-black alpha | Floating layers only. Surfaces stay flat. |
| `--focus-ring` | 2px white + 2px brand black | Every focusable control, via `:focus-visible`. |

## Not in this version

No component classes, no logo files, no PDF, share-page, or email styles. Those stay in each app. Timesheets is the first consumer and is not pinned yet.

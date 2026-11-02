# Brand rules for these tokens

Source: MarTech Mission Brand Guidelines V1.0. This file records the rules v0.1.0 follows. It does not redraw the identity. Logo files are not in this repository.

Deviations from the guidelines need approval from Priscilla (`priscilla@martechmission.com`).

## Color

| Name | Hex | CMYK | Token |
| --- | --- | --- | --- |
| Martech Peach | `#e18972` | 0 39 49 12 | `--brand` |
| Vivid Blue | `#186aea` | 90 55 0 8 | `--info`, `--link` |
| White | `#ffffff` | 0 0 0 0 | `--bg-surface` |
| Black | `#1e1e1e` | 0 0 0 88 | `--text`, `--action` |

Peach is identity only: the logo, an active-navigation mark, an avatar wash. It is not a button fill and not a success, warning, or danger color. Primary buttons are brand black (`--action`). White text on peach is not a control style.

Vivid Blue is the link color and the info color. The focus ring stays black: 2px white plus 2px brand black (`--focus-ring`). Focus does not use Vivid Blue.

The warm gray ramp, success, warning, danger, peach washes (`--brand-50`, `--brand-100`, `--brand-700`), and the heat ramp (`--data-1` … `--data-4`) are product extensions for app UI. They are not brand colors. They are listed in `tokens.md`.

## Type

In this design system, `--font-ui` and `--font-brand` both name **Poppins**. Poppins is the guidelines' secondary face (body, paragraphs, and longer passages). Apps load it themselves. This repository contains no font binaries.

WS Paradose is the guidelines' headline face (headlines, titles, and other prominent text). It stays out of this system until a webfont license is confirmed. Do not add the files, and do not set either font token to Paradose, before that.

Inter is not a brand face and is not a token.

## Logo

Use the primary logo in most situations. The guidelines also define color, black, white, horizontal, and vertical versions. On a light surface, use the color logo. Use the white or black version when the background calls for it.

Clear space: **x is the height of the word MISSION** in the logo. Keep at least that margin around the mark. The guidelines' diagrams also show tighter measures of x/2 and x/4 on parts of the lockup; x is the rule this system states, and the diagram's smaller measures are not a license to crop the wordmark.

The symbol plus the letter M is for social-profile images. It is not a substitute for the primary logo in an app header. The symbol may sit over photography or as a large background shape.

No logo files are stored here. Take artwork from the source linked in the guidelines, and do not redraw it.

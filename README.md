# MarTech Mission design system

Shared design tokens for MarTech Mission internal apps. The published surface is `tokens.css`, optional `components.css`, and these docs. There is no build, no npm package, and no React or Storybook.

`preview.html` is a static gallery you open in a browser next to `tokens.css`. It is a preview, not a published component API. Apps do not copy it.

David owns releases. Apps adopt a tag when they choose. Nothing here tracks `main`.

## What is published

| File | Purpose |
| --- | --- |
| `tokens.css` | CSS custom properties. Copy this from a tag. |
| `components.css` | Optional button, field, badge, and banner classes. Copy it the same way. |
| `tokens.md` | What each token means, and which ones are product extensions. |
| `brand/README.md` | Brand color, type, and logo rules this file is allowed to follow. |
| `CHANGELOG.md` | What changed in each tag. |
| `README.md` | How to pin a tag, and which apps have pinned one. |

## How an app depends on it

Copy `tokens.css` from a git tag. Record that tag next to the copy. Do not add this repository as an npm dependency.

Timesheets, when it pins a version, uses these paths:

- `public/css/tokens.css` — the copied file
- `public/css/TOKENS_VERSION` — one line, the tag, for example `v0.1.0`

```bash
git clone --depth 1 --branch v0.1.0 git@github.com:Martech-Mission/martech-design-system.git
cp martech-design-system/tokens.css public/css/tokens.css
printf '%s\n' v0.1.0 > public/css/TOKENS_VERSION
```

A later tag is adopted the same way, in that app's own change, after reading `CHANGELOG.md`.

Copy `components.css` from that same tag if the app wants the classes. They are optional, and they do not change the tokens. Timesheets would put the file at `public/css/components.css` and still record the one tag in `public/css/TOKENS_VERSION`. Link `tokens.css` before `components.css`.

## Consumers

| App | Pinned | Copy path |
| --- | --- | --- |
| timesheets | not yet pinned | `public/css/tokens.css` |

PDF reports, public share pages, and email are outside v0.1. They do not use this file yet.

## Versions

Tags are [semver](https://semver.org/spec/v2.0.0.html). `CHANGELOG.md` follows Keep a Changelog.

- **Patch:** comments, docs, or a fix that does not change a painted value.
- **Minor:** a new token or an optional component class. Existing tokens still mean the same thing.
- **Major:** a renamed or removed token, or a role that changes meaning (for example `--action` no longer being brand black).

The changelog entry, the tag, and a row in the table above are the announcement. There is no automatic upgrade.

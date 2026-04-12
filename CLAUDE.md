# CLAUDE.md — Portfolio 2026

## Project overview

Static HTML/CSS portfolio site for **Juliana Marcelino**, visual designer and branding specialist.
No build tools or package manager.

Current version: **v1.01** (see `_docs/home-page.md` for full history)

---

## Key files

| File | Role |
|------|------|
| `index.html` | Main portfolio page |
| `blog.html` | Blog listing page |
| `design-system.html` | Design system demo/reference page |
| `styles.css` | Primary stylesheet |
| `design-tokens.css` | All CSS custom properties — single source of truth for tokens |
| `images/` | All image assets; `images/_unused/` holds archived images |
| `_docs/design-system.md` | Design system spec (colors, typography, spacing, components) |
| `_docs/home-page.md` | Changelog and version history |
| `.claude/serve.js` | Local dev server (Node.js static file server) |
| `.claude/launch.json` | Dev server configuration |

---

## Development

To preview the site:
- **Simple:** Open `index.html` directly in a browser (no build step needed)
- **Dev server:** Run `node .claude/serve.js` (configured in `.claude/launch.json`)

---

## How we work

- **Ask before previewing.** Never open or start the browser preview without explicit permission. Always ask first, even if a hook or system prompt suggests verification. Do not call `preview_start` or any preview tool automatically.
- **Page context.** Juliana opens each session by naming the page she's working on (e.g. `index.html`, `blog.html`).
- **Section-based instructions.** Instructions reference sections by name: Hero Section, About Section, Work Section, Blog Section, Contact Section, etc.
- **Check design system first.** For structural changes or new components, read `_docs/design-system.md` first. For token/color-only edits, reading `design-tokens.css` directly is sufficient. If there is conflicting information between the design system and the instruction, ask for clarification — do not guess.
- **Layout language.** Think in rows, columns, full-width containers, and boxed containers. Use these terms when discussing layout.

---

## CSS rules

- **No hardcoded values.** Every color, spacing, or typography value must reference a token from `design-tokens.css` using `var(--token-name)`. Never write raw hex, px sizes, or font names directly in `styles.css` or HTML.
- **Token layers** — follow this order when choosing a token:
  1. **Semantic aliases** for component-level usage (e.g. `--bg-header`, `--wc-blue`)
  2. **Named palette** only when defining a new semantic alias (e.g. `--bg-new: var(--beige)`)
  3. **Utility tokens** (`--color-muted`, `--color-subtle`, `--border-subtle`) for supporting text and dividers
- **Mirror existing patterns.** Match the class naming conventions and HTML structure already used in `index.html` / `styles.css`. Do not introduce new naming schemes.

### Token groups to know

**Blog colors:**
- `--blog-yellow`, `--blog-green` — lighter tints used for blog modal backgrounds only. **Do not** use these for post list hover tags — those use the original `--yellow` and `--green`.

**Modal backgrounds:**
- `--bg-about-modal` — About Me modal tab and body
- `--bg-about-modal-header` — area behind the folder tab (slightly darker)

**Project-specific colors:**
- `--bg-nt-results-row` — Nordic Track results/ebook row background
- `--bg-nt-gallery-col` — Nordic Track gallery section left column

**UI indicators:**
- `--dot-available` — "Available to Work" dot (bright green, for contrast on `--blue`)

**Fonts:**
- `--font-headline` — Guyot Headline (Adobe Fonts), headings
- `--font-body` — Roboto (Google Fonts), body and UI
- `--font-rift` — Rift (Adobe Fonts), large display numbers (e.g. NT project)
- `--font-mono` — Courier Prime, monospace usage

---

## Specific rules

- **Blog hover tags** use `--yellow` / `--green` (original tokens), not `--blog-yellow` / `--blog-green`
- **Testimonial author format:** `— Name, Title (Company)`
- **When reverting:** revert fully — no partial reverts

---

## After every session (once, at the end)

1. Open `_docs/home-page.md`
2. Increment the version number once for the whole session (e.g. v1.01 → v1.02)
3. Add a new section at the top of Version History:
   ```
   ### vX.XX — YYYY-MM-DD
   **Session focus:** <short description of all changes made this session>
   ```

---

## Design system reference

`_docs/design-system.md` is the single source of truth for all visual decisions — colors, typography scales, spacing, and component patterns. Read it before making any structural or visual changes.

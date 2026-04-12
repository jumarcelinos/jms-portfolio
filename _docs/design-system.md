# Design System — Portfolio 2026

Single source of truth for all visual design decisions.
CSS tokens live in `/design-tokens.css`.

---

## Colors

### Named palette — Primary

These are the raw color values that define the brand. Always reference these when defining semantic tokens.

| Token | Hex | Usage |
|-------|-----|-------|
| `--maroon` | `#672527` | Primary highlight / accent, social circles, footer bg |
| `--black` | `#393939` | Body text, nav links, buttons (alias: `--dark`) |
| `--white` | `#ffffff` | White backgrounds and text |
| `--beige` | `#E2DFCB` | Header background, modal background |
| `--egg-white` | `#F4F5E8` | Page background, hero, sections |

### Named palette — Complementary

| Token | Hex | Usage |
|-------|-----|-------|
| `--yellow` | `#D8B76A` | Contact section background |
| `--green` | `#548B4D` | About modal name / title accent |
| `--blue` | `#2F53A1` | Hero card, work cards 1 & 6 |
| `--red` | `#ED5D29` | Work cards 3 & 5 |
| `--pale-purple` | `#CFAEBC` | Reserved |
| `--darker-beige` | `#CEBFA2` | Reserved |
| `--light-blue` | `#C1E1DC` | Reserved |
| `--sand` | `#DADCC2` | Blog section background |

### Semantic aliases

These tokens describe *usage*, not raw color. They always point to a named palette token above.

| Token | Points to | Hex | Used in |
|-------|-----------|-----|---------|
| `--dark` | `--black` | `#393939` | Backward-compat alias |
| `--cream` | `--beige` | `#E2DFCB` | About modal background |
| `--bg-page` | `--egg-white` | `#F4F5E8` | `<body>` |
| `--bg-hero` | `--egg-white` | `#F4F5E8` | Hero, Latest Work, About sections |
| `--bg-header` | `--beige` | `#E2DFCB` | Sticky header, testimonial carousel |
| `--bg-contact` | `--yellow` | `#D8B76A` | Contact section |
| `--bg-social` | `--maroon` | `#672527` | Social icon circles (header & footer) + footer bg |
| `--bg-blog` | `--sand` | `#DADCC2` | Blog section background |
| `--wc-blue` | `--blue` | `#2F53A1` | Work cards 1 & 6, hero card, blog rect |
| `--wc-cream` | `--egg-white` | `#F4F5E8` | Work cards 2 & 4 |
| `--wc-red` | `--red` | `#ED5D29` | Work cards 3 & 5 |

### Utility

| Token | Hex | Usage |
|-------|-----|-------|
| `--color-muted` | `#555` | Secondary / supporting body text |
| `--color-subtle` | `#999` | Nav number labels |
| `--border-subtle` | `rgba(57,57,57,0.12)` | Header bottom divider |

> **GoZeek modal only** (project-specific, not tokenized):
> Navy `#1d2a9f`, teal `#A0D6CD`, pink `#EC68A7`, yellow `#FEC909`

---

## Typography

### Font families

| Token | Value | Role |
|-------|-------|------|
| `--font-headline` | `'guyot-headline', Georgia, serif` | Headings H1–H3 |
| `--font-body` | `'Roboto', Helvetica, Arial, sans-serif` | Everything else |

**Loading:**
- Guyot Headline → Adobe Fonts (typekit.net)
- Roboto → Google Fonts

### Type scale

| Token | Size | Family | Weight | Line-height | Usage |
|-------|------|--------|--------|-------------|-------|
| `--text-h1` | 50px | Guyot Headline | 700 | 1.1 | Hero title |
| `--text-h2` | 40px | Guyot Headline | 700 | 1.15 | Section titles (Work, Blog, Contact) |
| `--text-h3` | 32px | Guyot Headline | 400 | 1.2 | About title, subsection titles |
| `--text-h4` | 30px | Roboto | 700 | 1.25 | Card titles |
| `--text-h5` | 20px | Roboto | 400 | 1.3 | Labels, subtitles |
| `--text-body` | 18px | Roboto | 400 | 1.65 | Body copy |
| `--text-btn` | 16px | Roboto | 700 | — | Buttons, nav numbers |
| `--text-logo` | 32px | Roboto | 700 | 1.1 | Wordmark ("Jumar") |
| `--text-sm` | 14px | Roboto | 700 | — | Tags, author labels |

**Special treatments:**
- `em` inside H1/H2/H3 → italic, weight 400 (no bold)
- Nav labels → underline, underline-offset 4px, letter-spacing 0.03em
- Hero subtitle → uppercase, letter-spacing 0.06em
- Testimonial author → uppercase, letter-spacing 0.06em

---

## Spacing

One scale covers padding, margin, and gap values across all sections.

| Token | Value | Key usages |
|-------|-------|------------|
| `--space-xs` | 8px | Social icon gap, brand-icon gap |
| `--space-sm` | 14px | Button vertical padding, small gaps |
| `--space-md` | 28px | About gutter, testimonial author gap |
| `--space-lg` | 48px | Header padding, nav gap, testimonial sides |
| `--space-xl` | 80px | Hero & section vertical padding, hero card padding |
| `--space-2xl` | 100px | About section vertical padding |

---

## Buttons

### `.btn-outline` (only button style)

| Property | Value |
|----------|-------|
| Padding | `14px 40px` |
| Font | Roboto 16px / Bold |
| Letter spacing | `0.12em` |
| Text transform | uppercase |
| Background | `#393939` (solid dark) |
| Border | `1.5px solid #393939` |
| Color | `#fff` |
| Border radius | 0 (sharp corners) |
| Transition | `0.25s` |

**Hover state:**
- Background → transparent
- Color → `#393939`
- Border stays `#393939`

---

## Icons

All icons are SVG files in `/images/`.

| Icon | File | Container | Image size | Usage |
|------|------|-----------|------------|-------|
| LinkedIn | `linkedIn.svg` | 36×36px circle | 16×16px | Header & Footer |
| Instagram | `instagram.svg` | 36×36px circle | 16×16px | Header & Footer |
| Mail | `mail.svg` | 36×36px circle | 16×16px | Header & Footer |
| Arrow | `arrow.svg` | — | 36px wide | Carousel nav, page links |
| Close | `close_window.svg` | — | auto | Modal close button |
| JMS Logo | `jms_logo.svg` | 80px height | auto width | Header right, Footer |

**Social icon treatment:**
- Container: 36×36px, `border-radius: 50%`, background `#672527`
- Hover: background changes to `#393939`
- Icon: 16×16px, filter `brightness(0) invert(1)` (white)

---

## Grid System

4-column named grid defined on `<body>`:

```
[full-start] minmax(40px,1fr) [content-start] 1fr [col3-start] 1fr [content-end] minmax(40px,1fr) [full-end]
```

| Column span | Used by |
|-------------|---------|
| `full-start / full-end` | `header`, `.hero`, `.contact-section`, `footer` |
| `content-start / content-end` | `.about`, `.latest-work`, `.blog-section` |
| `content-start / col3-start` | About left column |
| `col3-start / content-end` | About right column |

Children inherit columns via `display: grid; grid-template-columns: subgrid`.

---

## Transitions

| Token | Value | Usage |
|-------|-------|-------|
| `--transition-fast` | `0.2s` | Link/icon hover (opacity, color, transform) |
| `--transition-std` | `0.25s` | Button hover (background, border, color) |

---

## Border Radius

The design is intentionally sharp (rectangular). Most elements use `0`.

| Token | Value | Applied to |
|-------|-------|------------|
| `--radius-none` | `0px` | Buttons, form inputs, work card tags (Latest Work section) |
| *(no token — 20px)* | `20px` | Outline tag chips: `.proj-meta-tag` (GoZeek modal), `.bpp-tag` (blog preview), `.blog-modal-tag` (blog modal) |
| `--radius-circle` | `50%` | All social icon containers (header, footer, about modal) |

> **Note:** Work card tags (`.work-card .tag`) are flush with the top-left card corner and clipped by the parent's `overflow: hidden` — they use `0` radius to stay sharp.

---

## Component Quick Reference

| Component | Background | Typography | Notes |
|-----------|------------|------------|-------|
| Header | `--bg-header` | Roboto 18px bold nav | Sticky, z-index 100 |
| Hero card | `--wc-blue` | H1 Guyot, H5 subtitle | Max-width 520px, padding 80px |
| About section | `--bg-hero` | H2 + body copy | 2-col: text left, photo+carousel right |
| About pop-up | `--cream` → `--beige` | H1 name, H2 title, body | Width 1000px; Text 2 = looking-for, Text 3 = location |
| Work cards | 6 colour themes | H4 title, body desc | 3-col grid, aspect-ratio 640/845; tags square corners |
| Testimonial carousel | `--bg-header` | 18px italic | 5s auto-rotate, manual arrow |
| Blog cards | `--bg-hero` | H4 title, body meta | 3-col grid; outline tags, `border-radius: 20px` |
| Blog post modal | `--white` | H2 title (black), body | Width 1200px; share button bottom-right, design-system styled |
| GoZeek pop-up | `#1d2a9f` | Poppins headings | Width 1200px; meta tag chips `border-radius: 20px` |
| Contact section | `--bg-contact` | H2 + form inputs | Underline-only inputs |
| Footer | `--bg-social` | Roboto | 4-col grid matching page grid |

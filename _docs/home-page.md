# Home Page — Documentation
**Files:** `index.html` · `blog.html` · `styles.css`
**Designer:** Juliana Marcelino
**Project:** Portfolio 2026

---

## Version History

### v1.15 — 2026-04-11
**Session focus:** Detail pass across index.html — general, About section, About modal, Work section, Testimonials, and three project modals. Hover links: removed color changes on all hover states (nav sidebar, top nav, footer links, page numbers) — underline only. About section: bg changed to `about-bg-03.jpg`; copy updated ("It means I focus on the message…"); "Get to know me" gets underline on hover. About modal: Portfolio/Curriculum changed from styled buttons to `btn-text-link` text links; info box dividers moved from between items to under each title header; Curriculum download link added to Experience accordion. Work section: EcoFabrics card description updated to "Turning Transparency Into a B2B Buying Experience."; GoZeek card image `object-position: top` to avoid cropping subject's head. Testimonials: "Words" made italic in section heading. All three project modals: "Project Type" label renamed to "Work Format". GoZeek: CTA layout already correct (Work With Me centered, Next Project absolute right). EcoFabrics: hero subtitle updated; "Technology" tag color → `var(--ef-hero-bg)`; Challenge title: removed "time-pressed"; Process section title updated to "Different Personas, Same Need: Fast Access to Trusted Information"; Lars paragraph expanded. Nordic Track: website image gains `margin-bottom: 72px`; CTA divider replaced with full-width `<hr class="nt-cta-divider">` using negative margins; CTA section bottom padding aligned to match EcoFabrics (set `padding-bottom: 0` on `.nt-website`).

### v1.14 — 2026-04-09
**Session focus:** EcoFabrics modal — full case study restructure. Hero: bg → `#7B2D0D` (`--ef-hero-bg`), "Web Design" → "UI Design", location → "Odense". Intro nav: updated from 5 to 6 sections (01 About, 02 Challenge, 03 Research, 04 Process, 05 Design Decisions, 06 Results). Challenge: rows swapped (image row on top, text on bottom); two images replaced by single full-width `eco-product-list.png` (120px padding, boxed); text row bg → `var(--egg-white)` with 120px outer padding to match image boxing; label restored to normal flex flow (matching About section style); editorial image → `eco-two-woman-editorial.png`. Research: old Process section replaced entirely — new 2-column layout with `eco-lonely-boy-editorial.jpg` covering the left column and text content on the right; editorial image row later removed, collapsed to 1-column right with 72px padding; text condensed to single paragraph; bg → `#92BD91` (`--ef-research-bg`); overlap with Results fixed by removing fixed height, using `min-height` + `position: absolute` on left image + flex right column. Branding section removed. Process section added: 40/60 grid, `var(--dark)` bg, two personas copy, `eco-website-pages-composition-02.png` image vertically centered with 24px padding. Results: heading → "Every Structure Serves a User Need", new body text, left column replaced with auto-rotating infinite-loop slider (3 slides: `eco-product-page-screen.png`, `eco-category-page-screen.png`, `eco-search-screen.jpg`); seamless loop via clone technique; dots indicator. Tokens added: `--ef-hero-bg`, `--ef-research-bg`.

### v1.13 — 2026-04-08
**Session focus:** Project modal refinements and EcoFabrics modal built from scratch. Both modals (GoZeek + Nordic Track): arrow removed from "Next Project" text link, underline added, text link vertically centered with button. GoZeek: Challenge bg → `#1d2a9f`, button and text link → `#1d2a9f`. Nordic Track: logomark removed from Process section; two stacked website images replaced with `nordic-track-websites.png`; button and text link → `#175e50`; Website section bg → `#edeceb`. Brand colors tokenized as `--gz-brand`, `--nt-brand`, `--ef-brand`. Next Project chain wired: GoZeek → EcoFabrics → Nordic Track → GoZeek. EcoFabrics modal added: hero (dark forest green), Intro (3×2 collage grid, bg `#B39F7A`, nav links white), About (2-col, text left + full-cover image right, bg `#DBD7D0`), Challenge (2×2 grid, bg `#A05D41`, terracotta, text row + image row), Process, Branding, Results, and Website sections with CTA row.

### v1.12 — 2026-04-07
**Session focus:** blog.html synced with index.html — header CTA linked to PDF, footer subscribe form action updated to Formspree URL, blog card dates updated to full DD/MM/YYYY format, all 5 blog post modal contents updated to match index.html (arrow images, blog-modal-box, step tables, hr personality dividers), back button changed to close modal instead of reloading the page. Shared blog-posts.js created as single source of truth for post data; both index.html and blog.html now load blogPosts from this file.

### v1.11 — 2026-04-05
**Session focus:** blog.html updates. Footer synced with index.html (tagline, subtitle, text nav links, text social links). Contact section heading updated to match index.html ("Ready to Tell Your Brand Story?") with section label. Blog page headline changed to "Design Insights for Founders / and Brand-Builders" (two lines). Post titles weight reduced from 700 to 400. Scroll sidebar bug fixed (missing null guard on `navSidebarClose` was crashing the script). Blog post modal: content horizontal padding increased to 140px via new `--space-3xl` token. "Back to See More" now navigates to blog.html instead of just closing the modal.

### v1.10 — 2026-04-05
**Session focus:** Multi-section refinements. Accordions: period removed from badge labels; Experience relabeled B, Skills relabeled C. About right column: circled "A" badge added at bottom-right (`.about-right-badge`, absolutely positioned). Testimonials: all 9 author lines split into `.testi-author-name` (name) and `.testi-author-meta` (title + company) stacked vertically. Footer: col 2 label changed from "Menu" to "Explore"; new col 4 "Follow" added with email/LinkedIn/Instagram icons in white circles with maroon icon color; hover inverts to white icon + white outline; footer grid updated from `repeat(3, 480px)` to `repeat(4, 1fr)`; divider extended to new column.

### v1.09 — 2026-04-05
**Session focus:** Experience & Skills accordion refinements. A./B. badge circles restored before accordion titles. Solid black `border-bottom: 1px solid var(--dark)` added to both `.about-vtab--experience` and `.about-vtab--skills` accordion rows.

### v1.08 — 2026-04-05
**Session focus:** Header underline scoped to label only; About accordions moved to own section; About section padding confirmed 80px top and bottom. Header: nav link underline on hover now applies only to `.nav-label` span (not the number), both header nav and scroll sidebar. About: Experience and Skills accordions moved out of `.about` section into a new `.about-accordions` section directly below; CSS selectors re-scoped from `.about >` to `.about-accordions >`; `.about` section retains 80px top and bottom padding.

### v1.07 — 2026-04-05
**Session focus:** Header, About, Testimonials, Blog, and Footer updates across two sub-sessions. Header: hand-drawn circle removed from nav links; underline added on hover (both header nav and scroll sidebar). About: 80px bottom padding added below columns; accordion hover opacity effect removed; A./B. badge circles removed from accordion labels; both accordion backgrounds changed to `--beige`. Testimonials: Page 1 cards 2 and 3 swapped (Thomas before Carlos); Page 2 reordered to David → Anne → Camilla; Page 3 reordered to Sofia → David → Nina; auto-loop slowed to 8s; pause button removed; loop now pauses on card hover (`.testi-pages-wrap`) instead of full section hover. Blog section: page number indicators replaced with dots (`.testi-dot` style, dark color on sand bg). Footer col 2: sidebar-style nav reverted back to original plain links (02 About / 03 Work / 04 Blog).

### v1.05 — 2026-04-04
**Session focus:** Header, About section, and Footer overhaul. Header: About nav link (header + sidebar) now opens About Me modal via `.open-about` class; scroll close button JS null-guard fix; sidebar hover circle scoped to label-text width (auto width, ±8px offsets); Portfolio button hover: dark bg + white text. About: social icons replaced with "Juliana Marcelino" name (Roboto, `--text-h2`); Experience + Skills accordions moved inside the About section as full-width subgrid rows (removed standalone section wrappers); A./B. badge circles added before headings (28px circle, border, top-aligned at cap-height); 01 About label right-aligned (`justify-content: flex-end` + `flex: 0 0 auto` fix); bio text vertically centered (`height: 100%` fix); add icon 40px at `content-end`; both accordions start closed; same closed height via `min-height: 110px`; Skills overlap removed; about section bottom padding removed. Footer: three equal 480px columns; dividers changed from full-height `border-left` to 60%-height centered pseudo-elements (`top: 20%; height: 60%`); col 2 menu reduced to 02 About / 03 Work / 04 Blog (Contact removed).

### v1.04 — 2026-04-04
**Session focus:** Multi-section refinements across both pages. Scroll header: logo removed; sidebar internal close button removed (close button stays in scroll header only). About: accordion icons hidden when closed — no icon in closed state, remove icon in open state. Footer: cols 2 and 3 wrapped in `.footer-col-group` for equal sizing and closer grouping; Col 2 nav links now numbered (01–04) matching main nav style; social icons removed from footer; Col 3 gains "Odense, Denmark" location line above email. Testimonials: switched to CSS grid stacking (`grid-area: 1/1`) so all pages occupy the same space simultaneously — section height stays constant across page transitions, no layout jump. Blog post modal: reset to single flat column — `renderTwoCol` replaced by `renderContent` (title + rawHtml); `.blog-modal-row-1` 2-col grid removed; `font-style: italic` removed from `.blog-modal-title`; `.blog-modal-back-link` set to `font-weight: 700`.

### v1.03 — 2026-04-03
**Session focus:** Refinements across multiple sections. Header: Portfolio button hover now renders icon black (added `.header-cta:hover img` filter override). Scroll header: added `.scroll-header-close` button that shows when sidebar is open, hiding the hamburger; JS updated with `sidebar-open` class on scroll header and `scrollCloseBtn` listener (both pages). Sidebar: nav links changed to row layout — number and label on the same line. About: "Get to know me" button changed from `.btn-outline` to `.btn-text-link` (new class matching hero-cta style — text + arrow, transparent background); accordion icons fixed — add icon shows when closed, remove icon shows when open. Testimonials: reverted to natural height layout — `align-items: start` on `.testi-page`, scatter transforms removed. Footer: reset to 3-column layout — Col 1: headline tagline (Guyot font, large) + subscribe form; Col 2: menu label + vertical nav links + social icons; Col 3: Contact label + email link.

### v1.02 — 2026-04-03
**Session focus:** Multi-section overhaul across index.html, blog.html, and shared styles. Header: logo removed from static header (both pages); scroll-header dropdown replaced with a right-side sidebar overlay (.nav-sidebar) containing numbered nav links + Portfolio button; sidebar opens/closes on hamburger click with backdrop and Esc key support. Hero: --dot-available token updated to #22C55E for stronger green contrast. About: .about-label color changed from --yellow-dark to --dark (black, WCAG AA on yellow); accordion open state now hides the toggle icon entirely. Testimonials: scatter effect restored — per-card rotate/translateY transforms on nth-child selectors; align-self: stretch removed. Footer (both pages): Col 1 split into two inner columns — logo left, tagline + subscribe form right; subscribe form restyled as contact-form style (border-bottom only, transparent bg) with arrow icon replacing the button; Col 2 restructured as flex column — menu nav + social icons (moved here) + portfolio button; inner column divider removed; portfolio button padding updated to design system tokens. Blog post modal (both pages): tag outline removed; photo block padding added; meta row (author + date) moved to below image; divider moved below meta row; content restructured — row 1 is a 2-col grid with title (col 1) and first paragraph (col 2); renderTwoCol JS updated to accept title param; "Back to See More" link text capitalised. Blog.html intro: background-image updated to match header's exact 4-line vertical grid pattern.

### v1.01 — 2026-04-02
**Session focus:** Refinements and corrections. Scroll header: background made transparent (was --bg-header). Scroll logo enlarged to --logo-jms-height (64px). Hero h1: reverted handwriting spans — "Brand Stories" and "Connect" back to default font. About: .btn-outline button uses align-self: flex-start so it no longer stretches full width; padding reduced to proportionate 14px 28px via tokens. Work title: reverted circle-wrap / hand-drawn circle overlay. Testimonials: selective handwriting font — Page 1 card 2, Page 2 card 3, Page 3 card 1 use .testi-quote--handwriting; all other cards revert to --font-body. Cards fitted to grid: removed --a/b/c offset variants, align-self: stretch, gap reduced. Footer: full redesign on both pages — two-column row with top/bottom/divider solid lines; Col 1: logo + "Stay in Touch with Me" tagline + email subscribe form + social icons (white circle bg, black icons, left-aligned); Col 2: two inner columns — Menu nav (left) + Portfolio button (right); no gap between columns. blog.html header: replaced old identity block with same logo + nav + CTA as index. Blog contact title updated to match index. Blog post list: top padding added (--space-xl) to create space between intro and list.

### v1.00 — 2026-04-02
**Session focus:** Major multi-section overhaul. Scroll header (fixed bar) appears on scroll with logo + hamburger that opens a dropdown nav — added to both index.html and blog.html. Hero h1: "Brand Stories" and "Connect" now use Nothing You Could Do handwriting font via new `<span class="hero-handwriting">` wrappers. About: "Get to know me" changed from `<a>` to `.btn-outline` button. Testimonials: replaced 4-card pages with exactly 3 unique cards per page using `.testi-pages-wrap` + `.testi-page--1/2/3` grid variants for seamless animation; `.testi-quote` now uses handwriting font. Work: `<em>Selected Work</em>` wrapped in `.circle-wrap` + `.circle-svg` hand-drawn circle overlay. Footer: fully restructured on both pages — logo removed, centered social icons (email + LinkedIn + Instagram), bottom-right Menu nav block, bottom-right up-arrow. Blog intro: bg changed to `--bg-header` with column-line gradient + increased bottom padding. Blog post modal (both pages): tag moved to header row centre, author left / date right, portrait cover image, title below `<hr>` divider, content split into two-column sections (heading left, body right), "Back to see more" link replaces Share button. Blog contact form: added `select-wrap` + `arrow_drop_down.svg`.

### v0.99 — 2026-04-02
**Session focus:** Header logo to 64px, black (filter: brightness(0)). About: accordion fills full div height when open, slide-in animation, add.svg/remove.svg toggle icons far-right in circle, social icons bigger (40px circles), Tab 02 → beige, closed tabs push to bottom. Testimonial: auto-loop every 5s (pauses on hover), wide cards (span 2 cols) alternate with narrow for layout contrast, slide-in animation on page change. Contact: custom arrow_drop_down.svg icon on select, option border-radius removed. Blog.html: intro + list bg changed from beige to egg-white.

### v0.98 — 2026-04-02
**Session focus:** Header logo enlarged to 48px. About: social icons moved below portrait (centered); vertical tabs get +/− toggle icon in outline circle; Experience tab = pale-purple bg, Skills tab = darker-beige bg (label + content). Testimonial section: binder removed, replaced with maroon bg + quadriculado beige grid pattern, 3 scattered egg-white cards per page, 3 pages (8 testimonials), arrow + dot navigation. Contact: title centered.

### v0.97 — 2026-04-02
**Session focus:** Header logo: removed brightness filter (now shows in natural maroon), switched to --logo-jms-height token (32px), added align-self: flex-start. Hero "Available to Work" badge now has outlined pill border (new --radius-pill token). About section right column restructured as vertical accordion tabs — 01 About (bio), 02 Experience, 03 Skills & Tools — with JS tab switching.

### v0.96 — 2026-04-02
**Session focus:** Section reorder (Work now before Testimonial, Blog moved after Contact). Renamed Binder Section → Testimonial Section in HTML and CSS. Header logo resized to 32px (proportional to button). Header CTA button updated to match `.btn-outline` design system spec: correct padding, border, letter-spacing, uppercase, sharp corners, and proper hover state.

### v0.95 — 2026-04-02
**Session focus:** CLAUDE.md updated — version number corrected to v0.94, added missing key files (images/, serve.js, launch.json), documented undocumented token groups (blog colors, modal backgrounds, NT colors, dot-available, Rift and mono fonts), promoted learned feedback rules into the project file, and added "How we work" and "Development" sections.

### v0.94 — 2026-04-01
**Session focus:** Header logo height reduced to 15px. About section bg image changed to about-bg-02.JPG.

### v0.93 — 2026-04-01
**Session focus:** Header switched to subgrid — logo in left gutter, nav left-aligned at content-start, Portfolio button (black, download icon) in right gutter. About col 2: icons smaller (28px) with spacing, bio-inner vertically centered via flex column.

### v0.92 — 2026-04-01
**Session focus:** Header logo enlarged to 64px. Hero gets column-lines background-image (matching header). About: "About Me" tag replaced with social icon row (moved from header); about-label font changed from mono to Roboto.

### v0.91 — 2026-04-01
**Session focus:** Hero bg changed to beige (--bg-hero token updated). About col 2 bg changed to egg-white. about-bio-label gets tag-style outline (border 1.5px dark, radius 20px). "Get to know me" link added below bio, uses open-about class to trigger about modal.

### v0.90 — 2026-04-01
**Session focus:** About section uses subgrid to inherit body columns; left column placed at content-start/col3-start, right at col3-start/content-end — boxed within content area, no gap, bg image shows in gutters. Vertical padding only on section.

### v0.89 — 2026-04-01
**Session focus:** About section bg image extended to full-width (grid-column: full-start / full-end); columns remain visually boxed via the existing padding.

### v0.88 — 2026-04-01
**Session focus:** About section: about-bg.JPG set as background image (cover/center); padding var(--space-xl) added around the section.

### v0.87 — 2026-04-01
**Session focus:** About section changed from full-width (full-start/full-end) to boxed (content-start/content-end).

### v0.86 — 2026-04-01
**Session focus:** Header: identity text replaced with jms-logo.svg (black, 48px height); social icons enlarged to 40px circles / 18px icons. About: both inner containers set to height: 100% for equal height; about-right gets align-items: center to horizontally center about-bio-inner.

### v0.85 — 2026-04-01
**Session focus:** Hero: added footer bar below CTA with line above, name/role left and location right. About: wrapped left column content in .about-left-inner (max-width: 640px) to match .about-bio-inner width on the right.

### v0.84 — 2026-04-01
**Session focus:** Hero content container centered horizontally within the section.

### v0.83 — 2026-04-01
**Session focus:** Hero inner container capped at 1255px max-width; remaining border-bottom removed from Available to Work badge.

### v0.82 — 2026-04-01
**Session focus:** Hero section polish — inner wrapper made full-width (removed max-width: 640px); border-top removed from Available to Work badge; hero headline set to 70px via new --text-hero token.

### v0.81 — 2026-04-01
**Session focus:** Hero section simplified — SVG illustration removed, 2-column grid collapsed to single column, content (Available badge + headline + CTA) left-aligned.

### v0.80 — 2026-04-01
**Session focus:** Header layout: social icons moved to far right end; nav links centered (flex: 1 + justify-content: center). About section: removed justify-items: center so both columns fill their full 50% width edge-to-edge.

### v0.79 — 2026-03-30
**Session focus:** Nav right-aligned. Hero headline updated with extended copy. About columns horizontally centered; about-bio-inner matches hero-inner width (640px). Courier Prime added to font stack as --font-mono; applied to about-label and about-bio-label.

### v0.78 — 2026-03-30
**Session focus:** Hero right col content wrapped in hero-inner with padding. About section: bg changed to yellow, h3→h2, portrait smaller (55%), right col gets bio paragraphs with "About Me" label. Testimonial binder extracted into standalone binder-section below about.

### v0.77 — 2026-03-30
**Session focus:** Major layout restructure — Hero changed to true 2-column full-width (white grid col left / egg-white content col right); available-to-work badge gets border lines; all text/arrow dark. About changed to 2-column full-width; left col has label "01", centered title overlapping portrait, about-image-01 only; right col holds binder; image stack (02 & 03) removed.

### v0.76 — 2026-03-30
**Session focus:** Layout polish pass 2 — header grid lines more visible (0.07→0.18 opacity); squares animation changed to hover-per-row (no auto-loop); hero card text left-aligned; about-left full padding; about title split into 3 lines; binder tabs use per-tab colors (egg-white / pale-purple / darker-beige), panels equal height via CSS grid overlay; removed hand-drawn circle from Learn More; paper texture overlay on about-image-02 and about-image-03 via stack-wrap wrappers; paper clip added to binder right side.

### v0.75 — 2026-03-30
**Session focus:** Layout polish pass — hero card content centered; squares animation changed to independent row-based loops (3 rows, different speeds/phases); about-left padding added; tab labels widened; all binder panels given min-height; Experience tab/panel set to pale-purple; testimonials auto-rotate (4.5s, pause on hover), arrows moved below text left-aligned; Learn More links get hand-drawn circle on hover; contact dropdown border-radius removed.

### v0.74 — 2026-03-30
**Session focus:** Testimonial binder redesign — changed from 4 decorative tabs to 3 functional tabs (Testimonials / Experience / Skills); removed auto-rotating animation; testimonials now use manual prev/next arrow navigation; added placeholder Experience timeline and Skills grid panels.

### v0.73 — 2026-03-29
**Session focus:** SEO infrastructure — created robots.txt (disallows design-system.html, points to sitemap), created sitemap.xml (index + blog, priority 1.0/0.8), added canonical tags to index.html and blog.html (jms-design.com), added noindex/nofollow to design-system.html.

### v0.72 — 2026-03-29
**Session focus:** Folder housekeeping — deleted 4 unused blog-post HTML stubs (blog-post-2 through 5), archived 13 unreferenced images to images/_unused/, renamed 35 used images from underscores to hyphens for SEO (e.g. gozeek_hero.png → gozeek-hero.png), updated all src= and url() references in index.html, blog.html, design-system.html, and styles.css.

### v0.71 — 2026-03-27
**Session focus:** Accessibility quick wins — nav number contrast (#999→#555), placeholder/select contrast, skip-to-content link (index + blog), Formspree form wired up (honeypot + required fields, pending YOUR_FORM_ID), meta descriptions on both pages, testimonial tabs keyboard accessible (tabindex, role=tab, aria-selected, Enter/Space keydown).

### v0.70 — 2026-03-27
**Session focus:** Hero h1 "Brand Stories" italic; about h3 title bold; testimonial binder narrowed to 70% centered; blog page heading split with "Six Years" italic; blog post titles changed to h4 size.

### v0.69 — 2026-03-26
**Session focus:** Design system page — updated hardcoded size labels in design-system.html to match current tokens (H1: 50px, H2: 40px, H3: 32px).

### v0.68 — 2026-03-26
**Session focus:** Testimonial tabs — aligned left; right padding on testimonial text increased to 120px. About — section title changed from h2 to h3 (32px), CSS selectors updated. Design system doc — type scale usage column updated (H2 = section titles, H3 = About title + subsections). Latest Work — padding-bottom increased to 140px. Blog section — padding-bottom increased to 140px.

### v0.67 — 2026-03-26
**Session focus:** Grid — gutters reverted to original minmax(40px, 1fr).

### v0.66 — 2026-03-26
**Session focus:** Design system — H2 updated to 40px in tokens and design-system.md; new --dot-available token (#72DF77, bright green). Grid — gutters changed from minmax(40px,1fr) to minmax(16px,80px) for better small-screen content width. Hero — dot color changed to --dot-available for stronger contrast on blue. About — padding-bottom 170px added to .about-right to prevent Firefox stack-image overlap into row 2. Testimonial tabs — equal fixed width (130px), aligned right via justify-content:flex-end, flex:3 override removed. Work cards — overflow:hidden removed from .work-card to fix "Learn More" link clipping in Edge/Chrome.

### v0.65 — 2026-03-26
**Session focus:** Hero — headline reverted to "Helping Companies Tell Their Brand Stories" (title case); "Explore Work" capitalised. About — title reverted to "I Think About The Message, The Audience, And The Story Before I Open Any File". Testimonials — reduced to 4 tabs; tab 1 labelled "Testimonials" (flex:3, wider), tabs 2–4 unlabelled; removed Audrey Cremoux testimonial; JS updated to cycle 8 testimonials across 4 tabs (active tab = current % 4, rotation happens twice per loop); testimonial padding-right increased to 80px.

### v0.64 — 2026-03-26
**Session focus:** Hero — headline updated to "I help companies tell their brand stories"; card max-width reduced from 640px to 480px. About — title rewritten to "Before I open any file, I think about the message, the audience, and the story."; row 1 vertical alignment changed to center. Testimonials — single folder tab replaced with 9 individual numbered tabs (01–09), active tab highlights in sync with current slide; carousel JS updated so tabs are clickable and loop in sync; arrow button removed.

### v0.63 — 2026-03-26
**Session focus:** Hero — headline simplified to "Helping Companies tell their brand stories". About — layout restructured into two rows: row 1 has title + body text (left) and stacked images (right); row 2 has the testimonial binder spanning full content width below.

### v0.62 — 2026-03-25
**Session focus:** Header — social icons reduced to 28px/12px; hover state now shows black border + black icon; name and title colors changed to black. Hero — h1 reduced to 50px (h2→42px, h3→32px in tokens); blue card expands wider (max-width 520→640px) with reduced vertical padding (80px→60px top/bottom); dot color changed to --blog-green for contrast on blue. About — testimonial folder header background removed; tab text centered. Work — section title spacing increased to 80px; title split to 2 lines with "Selected Work" in italic. Blog section — title split to 2 lines with "Six Years" in bold italic. Contact — "Reach Out" wrapped in em for bold italic. Blog page — intro heading updated to match index.html title.

### v0.61 — 2026-03-25
**Session focus:** Header — background changed to --bg-header (beige), logo removed, identity block added on left (social icons + name/role/location in maroon/dark), nav moved to right column, subtle vertical grid lines added to background. Hero — headline updated to "Helping Companies Tell Their Brand Stories & Connect With Audiences"; "Available to Work" badge with green shimmer dot added above headline; "Explore work →" CTA link added below headline. About — title updated to "I Think About The Message, The Audience, And The Story Before I Open Any File"; body text replaced with 3 new paragraphs; testimonial carousel wrapped in binder folder shape (darker-beige header strip + beige rounded tab). Work — section title "From Brief To Brand: Selected Work" added above the grid. Blog section — title simplified to "What Over Six Years In Design Taught Me". Contact — title updated to "Got A Project In Mind? Reach Out To Start A Conversation". blog.html header updated to match index.html.

### v0.60 — 2026-03-25
**Session focus:** Blog page — nav replaced to match index.html exactly (Home/About/Work/Blog/Contact, no inline SVG scribbles, Blog marked active). Blog tag colors updated to lighter variants (new tokens --blog-yellow #F2DC9E, --blog-green #A8D0A2); blog modal themes use same lighter colors; all modal text uses dark/black (white override for strategy removed). blog-pg-intro-inner padding-bottom removed. Index about section — testimonial authors updated to "Name, Title (Company)" format. About modal — folder-body background reverted to light-blue (--bg-about-modal, same as tab); info-box background changed to --bg-about-modal-header (darker teal). Hero — replaced 10-div piano strip with inline SVG (hero_bg_image.svg); 18 columns of light-blue squares each wrapped in a .sq-col group; on hover odd columns go up/even go down with staggered 25ms delays per column.

### v0.59 — 2026-03-25
**Session focus:** Header — border-bottom replaced with soft scroll shadow (box-shadow appears after 10px scroll, both pages). Hero — removed drag interaction from blue card; replaced bg image with 10-column piano strip that animates on hover (odd columns up, even columns down, staggered delay). About — stack-img--3 moved down 3px (bottom: -130px → -133px); all 9 testimonial authors updated to Name, Title, Company format. Blog section — h5 titles clamped to max 3 lines with min-height for 3 lines; blog-img pinned to bottom of flex column. About modal — folder-header border-radius removed; folder-body bg changed to --bg-about-modal-header (darker teal). Nordic Track modal — branding section title shortened (removed "The Result: " prefix); left gallery column now shows nordic_track_stickers.png. Blog page — header stripped to match index.html (removed header-left/brand block); Strategy tag changed from blue to green; blog post modals now themed to match post tag colour (Branding = yellow bg with dark text, Strategy = green bg with white text).

### v0.58 — 2026-03-24
**Session focus:** All modals — overlay darkened from 0.55 to 0.78 opacity. About modal — folder-header padding-left removed (tab flush left); info-box bg changed to egg-white; close icon changed to black (brightness(0)). NT modal website section — replaced position: absolute on front image with normal-flow flex + margin-top: -80px + align-self: flex-end to fix cropping; removed overflow: visible and padding-bottom workaround.

### v0.57 — 2026-03-24
**Session focus:** NT modal — corrected target section from nt-process to nt-gallery. Gallery first column gets nt-gallery-col--light class with bg --bg-nt-gallery-col (#edeceb); second column gets nordic_track_presentation.png via nt-gallery-img. Reverted nt-process changes (white bg, single image, original nt-process-img-full). Renamed token --bg-nt-process-col → --bg-nt-gallery-col.

### v0.56 — 2026-03-24
**Session focus:** NT modal process section fix — .nt-process-img-full changed from height: 100% to flex: 1 + height: 0 so two cover images split the column height equally; overflow: hidden on the accent column now works correctly with both images visible.

### v0.55 — 2026-03-24
**Session focus:** About section — stack-img--3 (about_image_02) moved down 10px (bottom: -120px → -130px). About modal — info-box bg changed from pale-purple to beige; folder-header gets slightly-darker bg (--bg-about-modal-header: #AECFCB) with matching top border-radius. NT modal process section — left column bg changed to #edeceb (new --bg-nt-process-col token); nordic_track_presentation.png added to right column. New design tokens added: --bg-about-modal-header, --bg-nt-process-col.

### v0.54 — 2026-03-24
**Session focus:** About section — stack-img--1 moved up 30px (top: -30px); stack-img--2 (about_image_03) moved up 30px (bottom: -140px → -110px). About modal — added margin-bottom: 16px to h3 (space below title); added separator lines between info-box items via adjacent sibling selector. Latest Work — reordered cards: GoZeek now first (wc-green/blue) with gozeek_cover.jpg, EcoFabrics stays second, Nordic Track now third (wc-purple/red) with nordic_track_woman.png cover; JS modal triggers updated to match new class positions.

### v0.53 — 2026-03-24
**Session focus:** About modal — label centered in folder tab (justify-content: center); photo gets padding-top 36px; bio text bumped to 18px (--text-body); What I do / What I'm looking for / Location stays 16px; removed border-top divider under h3; three info paragraphs wrapped in .about-modal-info-box with pale-purple background and inner padding; removed old per-line borders.

### v0.52 — 2026-03-24
**Session focus:** About modal — modal label moved inside .about-folder-tab (flex row, centered); close button placed outside folder body in .about-folder-header (flex row, align-items: flex-end); #aboutModal .about-modal-inner changed to align-items: stretch; close icon filtered white.

### v0.51 — 2026-03-24
**Session focus:** About modal — photo changed to height: auto (no crop). Content padding increased to 72px horizontal / 80px bottom. Folder shape: about-modal-inner content wrapped in .about-folder-tab + .about-folder-body; #aboutModal .about-modal-inner set to transparent flex column; tab is 220×48px with rounded top corners; scoped to #aboutModal so project modals unaffected.

### v0.50 — 2026-03-24
**Session focus:** About section — about-stack shifted up 30px via margin-top: -30px. About Me modal — removed name/title overlay (Juliana Marcelino + Graphic & Brand Designer); social icons moved into location row, opposite Odense Denmark, using flexbox justify-content: space-between; icons scaled down to 32×32px (14px inner); top padding on location row reduced from 80px to 24px; old standalone social row removed.

### v0.49 — 2026-03-24
**Session focus:** Hero: blue card is now horizontally draggable via mousedown/mousemove/mouseup; position accumulates across drags; cursor: grab/grabbing added. About: "Get to Know Me" link and divider line removed; stack-img--2 (about_image_03) gains class open-about so clicking it opens the About Me modal.

### v0.48 — 2026-03-24
**Session focus:** About section — added border-top divider line above "Get to Know Me." link (display: block, border-top, margin/padding-top); removed <br>. Image stack — replaced scroll fly-in animation with hover-to-top: images sit in final positions from page load, hovering any image raises it to z-index: 10 with a 1.03 scale lift; --img-rotate custom property per image keeps rotations intact during scale; IntersectionObserver JS removed.

### v0.47 — 2026-03-24
**Session focus:** Header: replaced inline SVG scribbles in nav with CSS ::after pseudo-element using hand_drawn_circle.svg (black via filter: brightness(0)); hover text colour changed to dark; unused scribble-length JS removed. About: link text changed from "More About Me." to "Get to Know Me." placed on a new line via <br>.

### v0.46 — 2026-03-24
**Session focus:** About section — condensed text from 3 paragraphs to 2; "More About Me." inline link added at the end of paragraph 2 with class .open-about to trigger the About Me modal; .about-inline-link style added (bold underline, muted → dark on hover).

### v0.45 — 2026-03-24
**Session focus:** About stack — moved stack-img--2 (about_image_03) and stack-img--3 (about_image_02) down 60px by setting bottom to -60px and -40px respectively, extending them below image 01's baseline.

### v0.44 — 2026-03-24
**Session focus:** About stack — stack-img--1 moved out of absolute positioning into normal flow so it dictates the container height; fixed height removed from .about-stack. stack-img--2 switched from top to bottom: 0, aligning its bottom edge with image 01's bottom edge at any image size.

### v0.43 — 2026-03-24
**Session focus:** Header switched to subgrid (inherits body's 4-column layout); nav placed at content-start/col3-start, logo at col3-start/content-end with justify-self: end. Horizontal padding removed — gutters now handle alignment so nav and logo sit flush with the content area.

### v0.42 — 2026-03-24
**Session focus:** Nav: removed Curriculum link, removed text underline, replaced oval scribble with two animated scribbled underlines on hover; JS updated to set dash length per path. About section: both columns vertically centred (align-items: center). Stack images: about_image_01 tilt set to 0°; about_image_03 moved down (top: 110px).

### v0.41 — 2026-03-24
**Session focus:** Header: removed name logo and social icons, nav left-aligned, 6 items (Home, About, Work, Blog, Curriculum, Contact). Hero: removed "Brand & Graphic Designer" subtitle from blue card. About: removed About Me button, testimonials moved to left column below text, right column replaced with 3 stacked/overlapping images (about_image_01/03/02) with scroll-triggered fly-in animation.

### v0.40 — 2026-03-24
**Session focus:** Header background changed from var(--bg-header) to var(--bg-hero) so it blends with the hero section. About section copy updated with new bio and job-search positioning.

### v0.39 — 2026-03-23
**Session focus:** All blog posts (2–5) reverted to modal pop-ups on both blog.html and index.html. Full content added to all 5 posts in JS. Index page blog section updated: data-post-index on all cards, posts 4 & 5 added as page 2, working pagination (prev/next + page numbers), and a dedicated blog modal wired up. Titles updated to match exact post titles.

### v0.38 — 2026-03-23
**Session focus:** NT modal — Process: removed logo from text col, accent col now full-bleed women image with stretch alignment. New gallery section (Challenge layout, 2nd col offset) added between Branding and Results. Branding section bg → var(--bg-nt-results-row), row1 bg → #edeceb, ebook images get box-shadow. Website section images no longer clipped, shadows added to both. Blog: posts 2–5 converted to separate pages (blog-post-2 through blog-post-5.html), 4 new cards added to blog.html with full content. Index About image already confirmed as juliana_marcelino_foto_02.

### v0.37 — 2026-03-23
**Session focus:** NT modal — Challenge: removed first column (flipped women image), kept business card offset; grid updated to 2-col. Process: replaced both logos with nordic_track_women.png (full-bleed), added nordic_track_logo_02 above section label. Results (05): dark green bg (#175e50), two-col layout with nordic_track_man.png on left and white text (title, body, deliverables) on right.

### v0.36 — 2026-03-23
**Session focus:** NT modal: Challenge box padding increased to 56px/52px; Process columns aligned to center. Intro block expanded to 5 sections (01 About, 02 Challenge, 03 Process, 04 Branding, 05 Results). Former Results section renamed to Branding. New two-column Results section (05) added. Website section renumbered to 06.

### v0.35 — 2026-03-23
**Session focus:** NT Challenge section: added 72px horizontal padding. Results row 1: removed image crop (height: auto). New website section (05) added below Results with nordic_track_website.png as base and nordic_track_website_02.png overlapping from bottom-right.

### v0.34 — 2026-03-23
**Session focus:** Social icon hover: border turns black on hover. NT modal: intro numbers → 58px; process section both columns → white bg; results row 1 wrapped with sage green bg (#B5D5CA) and 320px uniform image height; results row 2 image → ebook_04, updated title and body text.

### v0.33 — 2026-03-23
**Session focus:** About Me modal: background changed to light blue (`--bg-about-modal`), photo grayscale filter removed (full color). Nordic Track modal: challenge text updated with correct copy; results row 1 populated with ebook images (ebook_02, ebook_03, ebook_01).

### v0.32 — 2026-03-20
**Session focus:** Nav scribble — replaced custom path with user's hand-drawn SVG; fixed size 110×38px across all links; JS `getTotalLength()` sets exact `--scribble-len` custom property for accurate dash animation; applied to both `index.html` and `blog.html`

### v0.31 — 2026-03-20
**Session focus:** Nav scribble redesigned as wide flat ellipse (96×32px fixed), single sweep from bottom-right CCW all the way round, short overshoot tail exits at bottom-right

### v0.30 — 2026-03-20
**Session focus:** Nav scribble — fixed size (86×40px) for all links, tail removed, open oval with slight path mismatch at bottom matching Jackie Zhang reference style

### v0.29 — 2026-03-20
**Session focus:** Nav scribble redesigned to near-closed organic oval with small pen-lift stroke at end (inspired by Jackie Zhang), consistent across all word lengths; blog contact bg → `--bg-blog`

### v0.28 — 2026-03-20
**Session focus:** Nav scribble refined — fixed height (48px), `preserveAspectRatio="none"`, updated viewBox + path for clean open-oval-with-tail shape; blog contact bg changed to `--bg-blog`

### v0.27 — 2026-03-20
**Session focus:** Nav scribble updated to open-oval-with-tail shape (maroon stroke, bigger), blog contact bg → `--pale-purple`, tag colour variants (Branding = yellow, Strategy = blue), blog post title hover inherits tag colour via `:has()` rule

### v0.26 — 2026-03-20
**Session focus:** Process section image gap increased; Results section rebuilt as white bg with 2-row grid (3-col row 1, 2-col row 2 with image + label/title/text); Blog index divider removed; Nav scribble hover animation added to both index and blog pages

### v0.25 — 2026-03-20
**Session focus:** Nordic Track modal — `min-height: 480px` set as standard for all `.proj-section`; intro columns center-aligned; process section rebuilt as two full-height columns (`#b5d5ca` accent + `#edeceb` content) with updated title and body text

### v0.24 — 2026-03-20
**Session focus:** Nordic Track challenge section — removed column gap, added "02 Challenge" label inside the box above the title, forced all box text to white

### v0.23 — 2026-03-20
**Session focus:** Nordic Track modal — locked fonts to Roboto + Rift only; challenge section bg → white, col 2 offset down, col 1 image flipped horizontally, box question promoted to h3 heading, box body text set to full white

### v0.22 — 2026-03-20
**Session focus:** Nordic Track modal — Rift font for all headings, intro bg `#58c966`, about text vertically centred, challenge rebuilt as 3-column layout (2 images + offset dark-green box)

#### Changes
- **GoZeek modal — Hero:** Project tags now have white background and `#1d2a9f` text (`.gz-hero .proj-meta-tag`)
- **GoZeek modal — Results:** Section background opacity reduced to 65% (`rgba(160, 214, 205, 0.65)`)
- **GoZeek modal — Website section:** New section added after Results displaying `gozeek_website.png` with `#FDDFE3` background
- **Color token:** Added `--sand: #DADCC2` to complementary palette in `design-tokens.css`
- **Blog background:** `--bg-blog` updated from `var(--egg-white)` to `var(--sand)` (`#DADCC2`)
- **Nordic Track modal:** Full project modal added following GoZeek structure (`.nt-*` classes, JS trigger on `.wc-green .learn-more`)
- **Project modal background:** `.proj-modal-inner` changed from `#1d2a9f` to `var(--white)`
- **Social icon hover:** `.header-icon-link` and `.about-modal-social-link` hover now outlined — transparent background + border, dark icon — matching the `btn-outline` hover pattern

---

### v0.17 — 2026-03-17
**Session focus:** Official color system established, design token architecture refactored, `styles.css` color audit, `design-system.html` demo page created

---

#### Color System — Specification

Formal color system defined with two tiers:

**Primary palette** (5 colors):
| Token | Hex | Role |
|-------|-----|------|
| `--maroon` | `#672527` | Primary highlight / accent (updated from `#7B2020`) |
| `--black` | `#393939` | Body text, nav, buttons |
| `--white` | `#ffffff` | White backgrounds and text |
| `--beige` | `#E2DFCB` | Header, modal background |
| `--egg-white` | `#F4F5E8` | Page background, hero, sections |

**Complementary palette** (7 colors):
| Token | Hex | Role |
|-------|-----|------|
| `--yellow` | `#D8B76A` | Contact section background |
| `--green` | `#548B4D` | About modal name / title accent |
| `--blue` | `#2F53A1` | Hero card, work cards 1 & 6 (was `#1B3DB5`) |
| `--red` | `#ED5D29` | Work cards 3 & 5 (renamed from `--orange`) |
| `--pale-purple` | `#CFAEBC` | Reserved |
| `--darker-beige` | `#CEBFA2` | Reserved |
| `--light-blue` | `#C1E1DC` | Reserved |

---

#### `design-tokens.css` — Architecture Refactor

Token file restructured from a flat list into **3 layers**:

1. **Named palette — Primary** (`--maroon`, `--black`, `--white`, `--beige`, `--egg-white`): raw hex values matching the official spec
2. **Named palette — Complementary** (`--yellow`, `--green`, `--blue`, `--red`, `--pale-purple`, `--darker-beige`, `--light-blue`): supporting colors
3. **Semantic aliases**: usage tokens that point to named palette tokens (no raw hex values in this layer)
   - `--dark: var(--black)` — backward-compat alias, all existing CSS still works
   - `--cream: var(--beige)` — about modal background
   - `--bg-page: var(--egg-white)` — body background (was `#EDE8DC`, now Egg White)
   - `--bg-hero: var(--egg-white)` — hero/about/work sections
   - `--bg-header: var(--beige)` — sticky header + testimonial
   - `--bg-contact: var(--yellow)` — contact section
   - `--bg-social: var(--maroon)` — social circles + footer
   - `--bg-blog: var(--egg-white)` — blog section (was `#DADCC2`)
   - `--wc-blue: var(--blue)` — work cards 1 & 6
   - `--wc-cream: var(--egg-white)` — work cards 2 & 4
   - `--wc-red: var(--red)` — work cards 3 & 5 (renamed from `--wc-orange`)
4. **Utility** (`--color-muted`, `--color-subtle`, `--border-subtle`): fixed values not tied to brand palette

**Removed tokens:**
- `--maroon-dark: #5C1A1C` — no equivalent in new system; references updated to `var(--maroon)`
- `--orange: #C85A28` — replaced by `--red: #ED5D29`
- `--wc-orange: #C85A28` — replaced by `--wc-red: var(--red)`
- `--bg-page: #EDE8DC` — value changed to `var(--egg-white)` (#F4F5E8)
- `--bg-blog: #DADCC2` — value changed to `var(--egg-white)` (#F4F5E8)
- `--cream: #EDE8DC` — value changed to `var(--beige)` (#E2DFCB)

---

#### `styles.css` — Color Audit & Fixes

6 categories of off-system colors resolved (GoZeek modal excepted per design decision):

| Location | Old value | New value | Reason |
|----------|-----------|-----------|--------|
| `body { background-color }` | `var(--cream)` | `var(--bg-page)` | Semantic separation: page bg ≠ modal bg |
| `.wc-purple`, `.wc-violet` (cards 3 & 5) | `#ED5D29` (hardcoded) | `var(--wc-red)` | Now tokenized |
| `.wc-purple .tag`, `.wc-violet .tag` | `#ED5D29` (hardcoded) | `var(--wc-red)` | Now tokenized |
| `.about-modal-inner { background }` | `#A5C5BF` (off-system teal) | `var(--cream)` → Beige | Aligned to new system |
| `.about-modal-social-link { background }` | `var(--maroon-dark)` | `var(--maroon)` | Token removed |
| `.about-modal-name`, `.about-modal-designer` | `#369A2A` (off-system green) | `var(--green)` | Now tokenized |
| About modal + blog modal content | `#2C2C2C` (×17, off-system near-black) | `var(--dark)` | Aligned to `--black: #393939` |

Work card comment updated: "cards 1&6: blue, 2&4: cream, 3&5: **red**" (was "orange")

---

#### `design-system.html` — New Demo Page

New standalone file at root level. Full visual reference for the design system. No server required — opens directly in browser.

**Sections:**
1. **Color Palette** — Primary (5 swatches) + Complementary (7 swatches) + Semantic aliases (6 swatches); each shows token name, hex value, and color block
2. **Typography** — Live rendering of all 9 type tokens (H1–H5, body, btn, logo, sm) with actual fonts and sample text; two-column layout with meta column
3. **Buttons** — `.btn-outline` at default state + hover state side by side; specs listed below
4. **Spacing** — Visual bar chart showing all 6 spacing tokens (xs → 2xl) with pixel values and usage notes
5. **Border Radius** — Three samples: `0px` box, `50%` circle, `20px` tag chip
6. **Icons** — All 6 SVGs rendered at design-system sizes (`linkedIn.svg`, `instagram.svg`, `mail.svg`, `arrow.svg`, `close_window.svg`, `jms_logo.svg`); social icons shown inside 36×36 maroon circles with white filter
7. **Components** — Header/nav bar, work card mini-grid (all 3 card themes), social icon circles, blog/modal tag chips, contact section sample, footer bar

Page styled using `design-tokens.css` (via `<link>`); brand fonts loaded (Adobe Typekit + Google Fonts); page background uses `--beige`.

---

#### `_docs/design-system.md` — Updated

- Color section rebuilt: flat brand/utility tables → **Primary / Complementary / Semantic / Utility** structure
- Removed `--maroon-dark`, `--orange`, `--wc-orange` entries
- Added all new named tokens with usage notes
- Semantic aliases table added with "Points to" column
- Component Quick Reference: About pop-up entry updated → `--cream → --beige`

---

### v0.16 — 2026-03-16
**Session focus:** Design system tokens, CSS compliance enforcement, GoZeek pop-up polish, global tag styling, blog modal refinements, about pop-up copy update

---

#### Design System — New Files

- **`design-tokens.css`** created — CSS custom properties file, single source of truth for all colours, type scale, spacing, button, icon, transition, and radius values
- **`_docs/design-system.md`** created — human-readable reference with tables for every token category
- `styles.css` refactored: `@import './design-tokens.css'` added at top; `:root {}` block removed (tokens now live in separate file)
- ~150 compliance violations fixed across `styles.css`:
  - ~90 hardcoded hex colours → tokens (e.g. `#393939` → `var(--dark)`, `#F4F5E8` → `var(--bg-hero)`)
  - ~25 hardcoded font sizes → tokens (e.g. `16px` → `var(--text-btn)`)
  - ~14 hardcoded transitions → tokens (e.g. `0.2s` → `var(--transition-fast)`)

---

#### GoZeek Pop-up

- Custom cursor (12px yellow circle) and trail animation (10 chasing dots) **removed** from modal and JS
- Section labels updated to match intro column labels:
  - "About" → **"01 About"**
  - "The Challenge" → **"02 Challenge"**
  - "03 Design Process" → **"03 Process"**
- Meta row restructured from a plain text line to outlined tag chips (`border-radius: 20px`):
  - `Role: Freelance Graphic Designer` → single outlined chip
  - `Project Type: Branding, Web Design, Print Design` → 3 separate chips: **Branding**, **Web Design**, **Print Design**

---

#### Global Tag Styling

- `border-radius: 20px` applied to all outline-style tags:
  - `.bpp-tag` (blog post preview cards on `blog.html`)
  - `.blog-modal-tag` (inside blog post modal)
  - `.proj-meta-tag` (GoZeek modal meta row)
- Work card `.tag` (Latest Work section): `border-radius` **removed** — sharp square corners retained (tag is flush with card corner, clipped by `overflow: hidden`)

---

#### Blog Post Modal

- Title color: `#369A2A` (green) → `#2C2C2C` (near-black)
- Title block bottom padding added (`24px`) — creates visual space between title and meta row (tag + date)
- Modal padding increased across all inner sections:
  - Horizontal: `52px → 72px`
  - Top: `28px → 48px`
  - Share row bottom: `48px → 56px`
- **Share button added** at bottom-right of modal:
  - Follows design system button tokens fully (`--btn-bg`, `--btn-color`, `--btn-border-color`, `--btn-border-width`, `--btn-font-size`, `--btn-font-weight`, `--btn-letter-spacing`)
  - `border-radius: var(--radius-none)` — sharp corners (design system standard)
  - Share row uses `justify-content: flex-end` — button sits at right edge
  - On click: copies `window.location.href` to clipboard; "Link copied!" confirmation fades in for 2 seconds then fades out

---

#### About Pop-up

- "What I'm looking for" paragraph split into **two separate lines**, each with a bottom border divider:
  - **Text 2**: "What I'm looking for: Graphic Designer, Brand Designer, or Visual Designer positions."
  - **Text 3** (new — `.about-modal-text-3`): "Location: in-house teams in Denmark (Odense, Copenhagen, Aarhus) or remote roles within the EU."

---

### v0.15 — 2026-03-16
**Session focus:** GoZeek project pop-up (full build), blog page heading + pop-up, index page blog section polish, about & pop-up width adjustments

---

#### Index Page — General
- Blog header nav link → now redirects to `blog.html`
- Hero card text: `align-items: flex-start → center` (vertically centred)
- Hero card horizontal padding: `60px → 80px`
- About pop-up width: `850px → 1000px`

---

#### Index Page — Blog Section
- "View All Posts" button added below pagination (text button, `text-decoration: underline`)
- `text-transform: uppercase` removed from `.blog-view-all`; `letter-spacing: 0.06em → 0.02em`

---

#### Blog Page (`blog.html`)
- Section heading changed: "What's on my mind" → "Insights I've Gained From Freelancing, Opening A Business Abroad, And Working In The Industry For Over 6 Years"
- `padding-top` removed from blog post list
- Page heading tag: `<h1> → <h2>` (`.blog-pg-heading`)
- **Blog post pop-up** implemented (modal, same structure as About pop-up):
  - Width: `1200px`
  - Header label: "03 blog"
  - Hero: image only — no overlapping title
  - Info row: date replaces "Odense, Denmark"; tag (outline style) on the opposite side
  - Post title displayed as modal subtitle
  - First blog post content added (Branding Assets article) with full text and branding assets table (24-item grid)

---

#### GoZeek Project Pop-up — New Feature
Each work card opens a project pop-up (1200px). GoZeek is the first built.

**Pop-up Global**
- Background: `#1d2a9f`
- All headings: `font-family: 'Poppins', sans-serif`
- Custom cursor: 12px solid `#FEC909` circle (`stroke: none` — no outline)
- **Cursor trail**: 10 easing dots (`position: fixed`, `z-index: 99999`) appended to `<body>`; each dot smaller + more transparent; smoothly chase cursor on `mousemove`; hidden when cursor leaves modal

**Hero Section** (`background: #1d2a9f`)
- "GoZeek" title color: `#FEC909`
- Subtitle + meta: `color: #fff`
- Meta (Role / Project Type): `font-size: 16px`
- Section nav removed from hero (moved to Intro section)
- Spacing between hero and intro section reduced

**Intro Section** (`background: #A0D6CD`, below hero)
- `gozeek_hero.png` centred in section
- 4 columns below image: `01 About · 02 Challenge · 03 Process · 04 Result`
  - Numbers + labels: `color: #393939`; `text-align: center`; horizontally centred
  - No border/line above nav
  - Opacity: `80%`
  - Hover animation: column translates upward (`translateY`)

**About Section**
- Title: "Building a Visual Identity Ready for the Next Level" — "Next Level" → `#EC68A7`
- Body text replaced with GoZeek app description paragraph
- Label "In Short" → "About"; moved above title
- Image changed to `gozeek_about.png`; not cropped (resized); flipped horizontally (`scaleX(-1)`)
- Line separator removed
- Padding added around title and text content
- Content vertically aligned to middle (`align-items: center`)

**Challenge Section** (`background: #002A85`)
- Layout: 2 rows with padding + gap between columns/rows
- **Row 1** — 3 equal columns (`border-radius: 43px` each):
  - Col 1: title "Designing Around the Brand's Strengths" (`bg: #EC68A7`); text left-aligned, vertically centred
  - Col 2: `gozeek_museum_02` image
  - Col 3: `gozeek_museum_03` image
- **Row 2** — 2 columns (`border-radius: 43px` each):
  - Col 1: `bg: #F6E2E3`; "The Challenge" label + body paragraph; `font-size: 18px` (standard body); extra padding
  - Col 2: `gozeek_museum_04` image

**Process Section** (`background: #fff`)
- Layout: 2 columns — `1fr / 2fr`
- Col 1 (1/3): `eye.png` (enlarged) above title + body text; "Wanted to Use" → `#EC68A7`
- Col 2 (2/3): `gozeek_presentation` image
- Eye brow animation on hover (SVG brow paths translate upward)

**Results Section** (`background: #A0D6CD`)
- Layout: 2×2 grid
  - Row 1 Col 1: `gozeek_linkedin.png`
  - Row 1 Col 2: "04 Results" label + title + body text
  - Row 2 Col 1: Testimonial quote — *"I can definitely recommend working with Juliana…"* — Anne Rahbek, Founder (styled with large `#EC68A7` opening mark, italic body, uppercase attribution)
  - Row 2 Col 2: `gozeek_folder.png`
- Title: "The Result: A Brand the Founders Could Believe In" — "Believe In" → `#EC68A7`
- All cell content vertically aligned to middle
- Images with matching `border-radius`
- Padding on text cells
- Challenge text col Row 2/Col 1 corrected to `font-size: 18px` (was 16px)
- Hero meta corrected to `font-size: 16px` (was 18px via `var(--text-body)`)

---

#### New Assets Used
| File | Used in |
|------|---------|
| `gozeek_hero.png` | GoZeek pop-up — intro section |
| `gozeek_about.png` | GoZeek pop-up — about section |
| `gozeek_museum_02.png` | GoZeek pop-up — challenge row 1 |
| `gozeek_museum_03.png` | GoZeek pop-up — challenge row 1 |
| `gozeek_museum_04.png` | GoZeek pop-up — challenge row 2 |
| `gozeek_presentation.png` | GoZeek pop-up — process section |
| `gozeek_linkedin.png` | GoZeek pop-up — results section |
| `gozeek_folder.png` | GoZeek pop-up — results section |
| `eye.png` | GoZeek pop-up — process section |

---

### v0.14 — 2026-03-14
**Session focus:** Global font-size audit, pop-up content & styling overhaul, testimonials height fix, blog page creation, contact form update, latest work polish, blog layout & new page

---

#### Global / Typography
- Body text, menu links, and contact form inputs confirmed at **18px**
- Button `font-size` (all buttons incl. "Learn more" in project card): `→ 16px`
- Header nav number labels: `→ 16px`
- Blog pagination numbers: `→ 16px`
- Latest Work `.card-desc` description: `→ 18px`

---

#### Header / Navigation
- About nav link `href` set to `#about` so it scrolls to the About section

---

#### About section
- "About Me" button now opens the pop-up (`data-target="about-popup"` / JS trigger wired up)

---

#### About pop-up
- **Subtitle** "Curious Creative, Lifelong Book Nerd, Explorer Of Vintage Bags And Furniture." → `font-weight: 700` (bold)
- Added **2px solid line** above the new info block (`.popup-divider-top`)
- Added **Text 1**: "What I do: Brand Design, UI Design, Marketing Design."
  - "What I do:" → `font-weight: 700`; rest of sentence → regular weight
- Added **1px solid line** below Text 1 (`.popup-divider-mid`)
- Added **Text 2**: "What I'm looking for: Graphic Designer, Brand Designer, or Visual Designer positions with in-house teams in Denmark (Odense, Copenhagen, Aarhus) or remote roles within the EU."
  - "What I'm looking for:" → `font-weight: 700`; rest of sentence → regular weight
- Added **1px solid line** below Text 2 (`.popup-divider-bot`)
- "01 About me" label + "Odense, Denmark" location: `font-size → 16px`
- Social icon hover: background changed to black (`#393939`) from the previous maroon tint

---

#### Testimonials
- Testimonial box given a **fixed height of 301px** so all slides occupy the same space
- Slide animation (fade/translate) scoped only to the **text and icon** — the box itself no longer resizes or animates between testimonials

---

#### Latest Work
- Added **bottom padding** inside each work card between the "Learn more" link and the card's lower edge (`padding-bottom` on `.card-body`)
- Description font-size confirmed → 18px (enforced via `.card-desc`)

---

#### Blog (index.html — homepage preview strip)
- Section title "Insights" → **"What's on my mind"**, forced onto two lines
- Section title line-width constrained to match main content column (not full bleed)
- Blog posts restructured into **3 columns** grid
- Tags ("Branding", "Strategy") styled with an **outline rectangle** border (no fill)
- Full stop removed from blog post titles
- **HTML order**: meta row → image/rect → title (title now sits below the image)
- Blog post images standardised to the **same dimensions** (`object-fit: cover`)
- Solid rule below section title: `1px → 2px`
- Gap between that rule and the post grid: reduced

---

#### Contact (index.html)
- Removed paragraph "I'm Available For Freelance Or Full-Time Roles." (stand-alone line deleted)
- `<h2>` text changed to: **"I'm Available For Freelance Or Full-Time Roles. Reach Out To Start A Conversation"**
- All contact-section text set to `color: #393939` (black)
- Added `<select>` field to the contact form with label **"Subject"** (formerly "Type of work") and options: *Freelance Project · Full-time Role · Other*
- `border-radius` removed from the `<select>` element (square corners)
- Contact section `.contact-section`: `align-items: center` added — left heading and right form now vertically centred relative to each other

---

#### Blog page — new (`blog.html`)
- **New page created** — standalone blog listing page
- Shares the same `<header>` and `<footer>` as `index.html`
- Layout inspired by hey-barista.com/short-talks: clean, editorial
- Section heading: "What's on my mind" (two lines), width matches main content
- Heading underline: **2px** solid rule; gap between rule and posts reduced
- Posts in a **3-column grid** (`blog-pg-grid`)
- Each post: meta row (tag + year) → image → title below image
- Tags styled with **outline rectangle** (border, no fill)
- Post images: fixed uniform dimensions (`object-fit: cover`)
- Contact form section inserted **above the footer** (same component as index)
- Pagination font-size: **16px**

---

### v0.13 — 2026-03-13
**Session focus:** About pop-up design, hero/about/work/blog/contact content & style updates, testimonials refresh

#### Changes

**About pop-up**
- Width: `480px → 650px → 850px`
- Photo: `juliana_ marcelino_foto.jpg → juliana_marcelino_foto_02.png`; horizontal padding `24px → 52px`; portrait shape (`height: 520px`); `object-position: center 20%` to avoid cutting face; `width: 62%` centred with `margin: 0 auto`
- Name: `<h2>` → `<h1>`; `font-size: var(--text-h1)` (60px); color `#D04F1A → #369A2A`
- Designer title: `<p>` → `<h2>`; `font-size: var(--text-h2)` (50px); color `#672527 → #369A2A`; italic bold
- Name + title overlay: repositioned from `left: 50%; transform: translateX(-50%)` → `left: 52px` (left-aligned, matches content padding / Curious text); `bottom: -55px` (overlap below photo)
- Location row top padding: `48px → 80px` (clears H1+H2 name block)
- All horizontal padding bumped `40px → 52px` (header, photo block, divider margins, content, social icons)
- "Curious Creative…" quote: `font-size: var(--text-h3)` (35px, Guyot); `font-weight: 400 → 700` (bold)
- Bio text: fully replaced with 4-paragraph version (freelancing journey, brand/graphic role, multicultural perspective)
- `contact-role` em elements (Freelance / Full-Time Roles): `font-style: normal; font-weight: 700; color: #393939` → `font-style: italic; font-weight: 400; color: #672527`

**Hero**
- "Digital Experiences" → **"Digital Design"**
- "Brand Strategy" subtitle → `font-style: italic; font-weight: 400`
- Blue card content: `align-items: flex-start → center` (vertically centred)

**About section**
- Title color → `#393939` (black)
- "Brand Stories and Genuine Connections" → `font-style: italic; font-weight: 400`
- Section background: `var(--cream) / #EDE8DC → #F4F5E8`

**Latest Work**
- Second row (cards 4–6: FreshFit Meals, Ecom Milan, TaskHero) → `display: none`
- Nordic Track: description → "Developing a Brand from Zero for a Business Education Platform"; tag → **branding**
- GoZeek: description → "Designing a Visual Identity for a Museum Adventure App"
- Section background → `#F4F5E8`

**Testimonials** — all 9 replaced:
1. Audrey Cremoux, Founder
2. Chloé Skye Weiser, Founder
3. Carlos Monteiro, Founder
4. Thomas Midtgaard, VP of Marketing
5. Anne Rahbek, Founder
6. Camilla Hviid, Frivilligkoordinator
7. David Sato, Ernst & Young
8. Sofia Gregoire, Kerry Group
9. Nina Vindell, Senmatic

**Blog**
- Section title color → `#393939` (black)
- "Freelancing, Opening A Business Abroad" → `font-style: italic; font-weight: 400`

**Contact**
- Swapped elements: `<h2>` is now "Reach Out To Start A Conversation About Your Project Or Team Needs." (bold, black, no italic)
- `<p class="contact-subtitle">` is now "I'm Available For *Freelance* Or *Full-Time Roles.*"
- `.contact-role` (Freelance / Full-Time Roles): italic, regular weight, `#672527`

---

### v0.12 — 2026-03-12
**Session focus:** Header logo swap, hero card fine-tuning, project name corrections, footer icon & gap clean-up, SVG colour fix

#### Changes
- **Header** — Logo `font-size: 35px → 32px`; "Odense, Denmark" text removed; replaced with `<img class="header-logo-right" src="images/jms_logo.svg">`; `.header-location` CSS replaced by `.header-logo-right { height: 80px; justify-self: end }`; CSS filter removed after SVG fill corrected directly
- **SVG** — `images/jms_logo.svg` fill `#da5d00 → #672527`; footer `brightness(0) invert(1)` filter still produces white (unaffected by fill change)
- **Hero** — Card `justify-self: start → end` (biased right: ~80% col 3, ~20% col 2); `margin-right: 80px` added to shift card 80px left from `content-end`
- **Latest Work — Project names**
  - Card 1 (`wc-green`): "FreshFit Meals" → **Nordic Track**
  - Card 4 (`wc-light`): "TaskHero" → **FreshFit Meals**
  - Card 5 (`wc-violet`): "NordicTrack" → **Ecom Milan**
  - Card 6 (`wc-forest`): "FreshFit Meals" → **TaskHero**
- **Footer** — Mail icon (`mail.svg`) removed from `.footer-social`; icon gap `8px → 12px`

---

### v0.11 — 2026-03-12
**Session focus:** Header location text, hero card repositioned, tag size, pagination numbers, footer icon clean-up

#### Changes
- **Header** — Logo `font-size: 30px → 35px`; added `<div class="header-location">Odense,<br>Denmark</div>` as 3rd header grid cell; `.header-location` styled Roboto Bold 35px, `justify-self: end`
- **Hero** — Card `grid-column: col3-start/full-end → content-start/content-end`; removed `margin-right: 48px`; `justify-self: end` kept (card right-edge at content-end = 35% in col 2, 65% in col 3)
- **Latest Work** — Tag `font-size: 10px → 18px`; `letter-spacing: 0.08em → 0.04em`
- **Blog pagination** — Removed `<span class="page-dot">` + `.page-dot` CSS; added `<div class="page-numbers">` with three `<span class="page-num">` items (first has `.active`); `.page-numbers` flex row gap 16px; active num bold/dark, inactive at 45% opacity; container widened `260px → 340px`
- **Footer icons** — Removed circle (no `width/height/border-radius/background`); icons now bare on maroon bg; `filter: brightness(0) → brightness(0)invert(1)` (white); size `16px → 20px`

---

### v0.10 — 2026-03-12
**Session focus:** Global colour update (#393939 text), header/hero/work card/blog/footer refinements

#### Changes
- **Global** — `--dark: #1A1A1A → #393939`; all `var(--dark)` usages (text, pagination dot, borders) now use `#393939`
- **Header** — `background: var(--cream) → #E2DFCB`; `logo font-size: 25px → 30px`; removed `text-transform: uppercase` (name now "Juliana Marcelino")
- **Hero** — Card `background: var(--blue) → #2F53A1`; repositioned to `grid-column: col3-start / full-end`, `justify-self: end`, `margin-right: 48px` (shifted right: ~35% col 3, ~65% col 4)
- **Work cards** — All 6 colour themes updated:
  - Cards 1 & 6 (`wc-green`, `wc-forest`) → `#2F53A1`
  - Cards 2 & 4 (`wc-tan`, `wc-light`) → `#F4F5E8` (light); text/icons `#393939`
  - Cards 3 & 5 (`wc-purple`, `wc-violet`) → `#ED5D29`
  - Tag colours match card colours exactly; cream-card tags use `color: #393939`
- **Blog** — Background line opacity `0.65 → 0.40` on all 5 gradient lines (4 vertical + 1 horizontal)
- **Footer** — Icon circle `rgba(255,255,255,0.15) → #D8B76A`; icon filter `brightness(0)invert(1) → brightness(0)` (dark on golden); footer info `font-size: 18px → 20px`; `.footer-logo` gets `margin-left: auto` (right-aligned in column)

---

### v0.9 — 2026-03-12
**Session focus:** Hero bg image; blog H2 + 4-line grid; work card redesign; footer social icons

#### Changes
- **Hero** — `<img class="hero-bg-img">` added behind the card in the same grid row/column; card `z-index: 1`, image `z-index: 0`; card padding `52px → 80px` to sit taller than bg image
- **Blog heading** — `<h3>` → `<h2>` in HTML; CSS selectors updated to `.blog-section > h2`
- **Blog grid lines** — 3 lines → 4 lines at 20/40/60/80%; colour `#393939 → rgba(57,57,57,0.65)`
- **Blog images** — `width: 438px; height: 482px; max-width: 100%`; `.blog-rect min-height: 300px → 482px`
- **Work cards** — `aspect-ratio: 640/845`; new `.card-img-wrap` (aspect 576/552, margin 5%) + `.card-body`; tag `163×72px absolute top-left`; all 6 cards restructured in HTML
- **Footer** — email corrected to `hello@jms-design.com`; col 2 nav removed; social icons in col 1 via `.footer-social` + `.footer-icon-link`; body text `14px → 18px`

---

### v0.9 — 2026-03-12
**Session focus:** Blog grid background, heading alignment, number alignment, dot size; contact 4-col subgrid with full-height divider

#### Changes
- **Blog — Section heading**
  - Added `margin: 0 auto 64px` (replaces `margin-bottom: 64px`) so block is centred within its column span, not just text-aligned

- **Blog — Post card numbers**
  - `.blog-card` `text-align: center → left` — numbers now align with the left edge of titles

- **Blog — Pagination dot**
  - `width/height: 10px → 5px` (very small)

- **Blog — Section background**
  - `background` changed to `background-color` + `background-image` with 4 CSS gradient layers:
    - 3 vertical lines at `25%`, `50%`, `75%` of section width (`#393939`, 1px)
    - 1 horizontal line at `50%` section height (`#393939`, 1px)

- **Contact — Layout rebuild**
  - `grid-template-columns: 1fr 1fr → subgrid` (inherits body 4-col grid)
  - Section padding removed (`140px 80px → none`) — padding moved into columns so divider runs full section height
  - `.contact-left` → `grid-column: content-start / col3-start` (body col 2); `padding: 140px 80px 140px 48px`
  - `.contact-right` → `grid-column: col3-start / content-end` (body col 3); `padding: 140px 48px 140px 80px`
  - `border-right: 1px solid #393939` on `.contact-left` now spans the full section height (CSS Grid stretch default)

---

### v0.8 — 2026-03-12
**Session focus:** Typography tag audit — blog heading centred, post titles H5 + left-aligned

#### Changes
- **Hero** — confirmed: title already `<h1>` (Guyot Bold 60px) ✓
- **About** — confirmed: section title already `<h2>` (Guyot Bold 50px) ✓
- **Latest Work** — confirmed: project titles already `<h3>` (Guyot Regular 35px) ✓

- **Blog — Section heading**
  - `text-align: center` added to `.blog-section > h3`

- **Blog — Post titles**
  - Changed from `<h3>` to `<h5>` in HTML (all 3 cards: posts 01, 02, 03)
  - CSS selectors renamed: `.blog-card h3` → `.blog-card h5`; `.blog-rect h3` → `.blog-rect h5`
  - `text-align: left` added to `.blog-card h5` (overrides card-level `text-align: center`)

---

### v0.7 — 2026-03-12
**Session focus:** Logo size, blog heading tag, pagination dot, contact colour correction + internal padding, footer line-height + logo

#### Changes
- **Header**
  - Logo font-size: `20px → 25px`

- **Blog**
  - Section heading changed from `<h2>` to `<h3>` in HTML (post titles remain `<h3>` via `.blog-card h3`)
  - CSS selector updated: `.blog-section h2` → `.blog-section > h3` (direct child, avoids conflict with post-title `.blog-card h3`)
  - **Pagination dot added**: `<span class="page-dot"></span>` inserted between prev/next arrow buttons; styled as `10px` solid circle (`background: var(--dark); border-radius: 50%`)

- **Contact**
  - Colour corrected: all `#DADCC2` references replaced with `#393939`
    - `.contact-left h2 { color }`, `border-right color`, `input { color }`, `input border-bottom rgba`, `input:focus border-color`, `input::placeholder color`
  - Removed `margin: 80px 0` (outer margin); vertical breathing room is now purely internal padding
  - Padding increased: `100px 80px → 140px 80px` (section)
  - `.contact-left` padding: `0 80px 0 0 → 0 80px 0 48px` (added inner left pad so text wraps, doesn't stretch edge-to-edge)
  - `.contact-right` padding: `0 0 0 80px → 0 48px 0 80px` (added inner right pad to mirror)

- **Footer**
  - `line-height: 1.9 → 1.4` on `.footer-col p`, `.footer-col > a`, `.footer-nav a`
  - `.footer-col h4` `margin-bottom: 10px → 4px`
  - `.footer-logo` `width: 80px → 150px`

---

### v0.6 — 2026-03-12
**Session focus:** Header sizing, blog full-width + pagination, contact polish, footer 4-col rebuild

#### Changes
- **Header**
  - Logo font-size: `30px → 20px`
  - Nav number labels: `11px → 14px`

- **Blog**
  - Section now spans `full-start / full-end` with `background: #DADCC2` and `display: grid; grid-template-columns: subgrid` so children snap to content columns
  - Post titles changed from `<h5>` (Roboto 20px) to `<h3>` (Guyot Regular 35px)
  - Blog cards: `text-align: center` (numbers + titles centred)
  - `.blog-rect`: inherits `text-align: left` override so number/title align naturally inside the rectangle
  - `.blog-rect h3` (was `h5`) set to `color: #fff`
  - **Pagination added** below `.blog-grid`: two `<button class="page-arrow">` with `arrow.svg`; prev arrow flipped via `scaleX(-1)`; container is `max-width: 260px; margin: auto` for centred placement

- **Contact**
  - `margin: 80px 0` added (breathing room above and below the section)
  - `gap: 48px → 0` (visual separation now handled by vertical line)
  - `.contact-left` `padding-right: 40px → 80px` + `border-right: 1px solid #DADCC2` (1pt divider)
  - `.contact-right` `padding-left: 40px → 80px`
  - Heading color: `#fff → #DADCC2`
  - Input text color: `#fff → #DADCC2`
  - Input border-bottom: `rgba(255,255,255,…) → rgba(218,220,194,…)` to match `#DADCC2`
  - Input placeholder: same colour update

- **Footer** — Complete rebuild
  - Layout: `display: flex → display: grid; grid-template-columns: repeat(4, 1fr)`
  - Background: `var(--maroon-dark) #5C1414 → #672527`
  - **Col 1:** Name / Brand & Graphic Designer / email / city
  - **Col 2:** Nav links (About, Work, Blog, Contact) via `footer-nav`
  - **Col 3:** Empty
  - **Col 4:** `jms_logo.svg` at 80px, white via `filter: brightness(0) invert(1)`
  - Removed old `.footer-left`, `.footer-right`, `.footer-links`, `.jms-logo` span-circle approach

---

### v0.5 — 2026-03-12
**Session focus:** Header cleanup, blog rect layout, contact section restyle

#### Changes
- **Header**
  - Logo font-size: `40px → 30px`
  - Traffic-light dots removed from HTML (macOS decorative circles — red/yellow/green)
  - `.header-left` gap removed (single child now)

- **Blog**
  - `.blog-card .blog-num` font-size: `11px → 20px`
  - Post 2: number moved **inside** `.blog-rect` (sibling of title, not card sibling)
  - `.blog-rect` changed from fixed `aspect-ratio: 4/3` to `flex: 1` — fills full card height automatically by stretching to match tallest card in the row
  - `.blog-rect` layout: `justify-content: space-between` — number sits at top, title pinned to bottom
  - `.blog-rect .blog-num` color: `rgba(255,255,255,0.6)` (lighter on dark bg)

- **Contact**
  - Background: `#C85A28 (--orange) → #D8B76A`
  - Gap between columns: `80px → 48px`
  - `.contact-left`: `padding-right: 40px` added
  - `.contact-right`: `padding-left: 40px` added
  - Submit button now matches About Me button: `background: #393939; color: #fff; border: 1.5px solid #393939`; hover: transparent fill with `color: #393939`

---

### v0.4 — 2026-03-12
**Session focus:** Header icons, typography polish, hero centering, work & blog cards

#### Changes
- **Global CSS**
  - Added icon override block after global `img` rule: `.header-icon-link img`, `.carousel-arrow img`, `.learn-more-arrow` opt out of `width:100%/height:100%` stretch

- **Header**
  - Vertical padding increased: `20px → 32px` top/bottom
  - Traffic lights + logo wrapped further: new `.header-brand` flex-column (icons stacked above logo)
  - Social icons added above logo name, each in a `36px` circle (`background: #672527`), icons white via `filter: brightness(0) invert(1)`
    - Mail → `mailto:hello@jms-design.com`
    - LinkedIn → `linkedin.com/in/julianamarcelinosilva/`
    - Instagram → `instagram.com/jms.design.dk/`
  - Logo: `font-size: 40px; font-family: Roboto; font-weight: 700`
  - Nav links: added `font-weight: 700`

- **Hero**
  - Card changed from right-column only (`col3-start/content-end`) to centered: `grid-column: content-start/content-end; justify-self: center; max-width: 520px`

- **About**
  - Photo height: `320px → 400px`
  - `object-position: center top` (face stays visible)

- **Latest Work**
  - `.card-desc` font-size: `12px → 16px`
  - All "Learn more" links now flex row with `arrow.svg` (28px, white filter on dark cards; no filter on light card)
  - GoZeek card: `gozeek_cover.jpg` added as `.card-cover` (position absolute, fills card); gradient overlay (`z-index:1`) added via `::after`; all card text lifted to `z-index: 2`

- **Blog**
  - Posts restructured: order is **number → title (H5) → image/rect**
  - Post 1: `blog_cover_2.png` as `<img class="blog-img">`
  - Post 2: `.blog-rect` (blue `#2F53A1`, `aspect-ratio: 4/3`), title in white at bottom
  - Post 3: `blog_cover_01.png` as `<img class="blog-img">`
  - Blog titles changed from `<h3>` to `<h5>` (Roboto 20px)

---

### v0.3 — 2026-03-12
**Session focus:** Visual refinements & content fixes

#### Changes
- **Header**
  - Converted from `display: flex` to `display: grid` (3-col: logo | nav | spacer) to center navigation
  - Nav link color updated to `#393939`
  - Added `text-decoration: underline` with `text-underline-offset: 4px` to `.nav-label` spans
  - Traffic lights + logo wrapped in `.header-left` flex container

- **Hero**
  - Removed JS-generated checkered grid background
  - Applied solid background color `#F4F5E8`
  - Subtitle text changed to **"Brand & Graphic Designer"**; set to `font-size: 20px; font-weight: 700`
  - H1 title split across 4 lines: *Combining / Brand Strategy / with Digital / Experiences*

- **About — Photo**
  - Replaced grey placeholder `<div>` with real `<img>` (`juliana_ marcelino_foto.jpg`)
  - `object-fit: cover; object-position: top` to keep face in frame

- **About — Testimonial Carousel**
  - Background color updated to `#E2DFCB`
  - Horizontal padding increased: `32px → 48px` per side
  - Arrow changed from `→` text to `arrow.svg` image (36px wide)
  - Arrow hover: `translateX(6px)` slide right

- **About — Button**
  - Changed from outlined to filled: `background: #393939; color: #fff`
  - Hover effect: transparent fill, `color: #393939` (inverse)

---

### v0.2 — 2026-03-12
**Session focus:** Typography, grid, carousel & structural CSS split

#### Changes
- Extracted inline styles from `index.html` into separate `styles.css`
- Added font imports: Guyot Headline (Adobe Fonts) + Roboto (Google Fonts)
- Established 4-column page grid with named lines: `full-start`, `content-start`, `col3-start`, `content-end`, `full-end`
- Set global type scale: H1 60px · H2 50px · H3 35px · H4 30px · H5 20px · Body 18px
- Nav links enlarged: `12px → 15px`
- Hero card moved to column 3 only (`col3-start / content-end`); `padding: 100px 0` added
- About section: horizontal padding `0 → 48px`
- Testimonial converted to auto-rotating carousel (5s interval, arrow manual nav, fade animation)
- Created `images/` folder

---

### v0.1 — 2026-03-12
**Session focus:** Initial build from XD screenshots

#### Structure built
- `index.html` — single-file with embedded CSS
- 7 sections: Header · Hero · About · Latest Work · Blog · Contact · Footer

#### Design decisions
- 4-column CSS grid on `<body>` for layout control
- MacOS-style traffic light dots in header
- Hero: JS-generated checkered background (maroon / olive / yellow-olive palette)
- Work grid: 3×2 card layout with colour-coded project cards
- Blog: 3 numbered article cards
- Contact: orange (`#C85A28`) section with underline-only form inputs
- Footer: dark maroon (`#5C1414`) with JMS circle logo mark

---

## Colour Tokens
| Token           | Value     | Used in                          |
|-----------------|-----------|----------------------------------|
| `--cream`       | `#EDE8DC` | Page background                  |
| `--dark`        | `#1A1A1A` | Default text                     |
| `--maroon`      | `#7B2020` | Italic accent (headings)         |
| `--maroon-dark` | `#5C1414` | Footer background                |
| `--blue`        | `#1B3DB5` | Hero card background             |
| `--orange`      | `#C85A28` | Contact section background       |
| Hero BG         | `#F4F5E8` | Hero section                     |
| Testimonial BG  | `#E2DFCB` | Testimonial carousel             |
| Nav / Button    | `#393939` | Nav links, About Me button       |

## Typography
| Tag | Family        | Size  | Weight  |
|-----|---------------|-------|---------|
| H1  | Guyot Headline | 60px | Bold    |
| H2  | Guyot Headline | 50px | Bold    |
| H3  | Guyot Headline | 35px | Regular |
| H4  | Roboto         | 30px | Bold    |
| H5  | Roboto         | 20px | Regular |
| p   | Roboto         | 18px | Regular |

## Page Sections — index.html
| Section       | Grid column              | Notes                                  |
|---------------|--------------------------|----------------------------------------|
| Header        | `full-start / full-end`  | Sticky, 3-col inner grid               |
| Hero          | `full-start / full-end`  | Subgrid; card in `col3-start/content-end` |
| About         | `content-start / content-end` | 2-col internal grid, 48px side padding |
| Latest Work   | `content-start / content-end` | 3×2 work card grid                |
| Blog strip    | `content-start / content-end` | 3-col preview cards               |
| Contact       | `full-start / full-end`  | Gold BG, subgrid, vertically centred cols |
| Footer        | `full-start / full-end`  | Maroon `#672527`, 4-col grid           |

## Page Sections — blog.html
| Section       | Notes                                                      |
|---------------|------------------------------------------------------------|
| Header        | Shared with index — same HTML/CSS                          |
| Blog header   | "What's on my mind" (2 lines), 2px rule, content-width     |
| Blog grid     | 3-column; meta → image → title; outline tags               |
| Contact       | Same contact form component as index                       |
| Footer        | Shared with index — same HTML/CSS                          |

## Assets Used
| File                          | Used in            |
|-------------------------------|--------------------|
| `juliana_ marcelino_foto.jpg` | About photo        |
| `arrow.svg`                   | Testimonial nav    |
| `arrow.svg` (viewBox 489×188) | Work cards, testimonial nav |
| `jms_logo.svg`                | (available, unused)|
| `instagram.svg`               | Header social icon |
| `linkedIn.svg`                | Header social icon |
| `mail.svg`                    | Header social icon |
| `gozeek_cover.jpg`            | GoZeek work card + pop-up about section (fallback) |
| `gozeek_hero.png`             | GoZeek pop-up — intro section                      |
| `gozeek_about.png`            | GoZeek pop-up — about section                      |
| `gozeek_museum_02.png`        | GoZeek pop-up — challenge row 1 col 2              |
| `gozeek_museum_03.png`        | GoZeek pop-up — challenge row 1 col 3              |
| `gozeek_museum_04.png`        | GoZeek pop-up — challenge row 2 col 2              |
| `gozeek_presentation.png`     | GoZeek pop-up — process section col 2             |
| `gozeek_linkedin.png`         | GoZeek pop-up — results row 1 col 1               |
| `gozeek_folder.png`           | GoZeek pop-up — results row 2 col 2               |
| `eye.png`                     | GoZeek pop-up — process section col 1             |
| `blog_cover_2.png`            | Blog post 1                                        |
| `blog_cover_01.png`           | Blog post 3                                        |
| `close_window.svg`            | About, blog, and GoZeek pop-up close button        |

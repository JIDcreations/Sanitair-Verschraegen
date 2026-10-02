---
name: Sanitair Verschraegen
description: One aanspreekpunt from ruwbouw to droombadkamer, drawn as one continuous blue installation line.
colors:
  blue: "#0081b8"
  blue-strong: "#00699a"
  blue-deep: "#0a4f73"
  field: "#0077aa"
  ink: "#0f2a3a"
  steel: "#53616b"
  hair: "#d6e0e7"
  mist: "#eef4f8"
  bg: "#fbfcfd"
  surface: "#ffffff"
  on-strong: "#ffffff"
  error: "#b42318"
typography:
  display:
    fontFamily: "'Barlow Condensed', 'Arial Narrow', sans-serif"
    fontSize: "clamp(3rem, 0.6rem + 4.6vw, 5rem)"
    fontWeight: 700
    lineHeight: 0.92
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "'Barlow Condensed', 'Arial Narrow', sans-serif"
    fontSize: "clamp(2.5rem, 1.6rem + 3vw, 4.25rem)"
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: "-0.005em"
  title:
    fontFamily: "'Barlow Condensed', 'Arial Narrow', sans-serif"
    fontSize: "clamp(2.25rem, 1.5rem + 2.6vw, 3.75rem)"
    fontWeight: 700
    lineHeight: 0.9
    letterSpacing: "-0.005em"
  statement:
    fontFamily: "'Barlow Condensed', 'Arial Narrow', sans-serif"
    fontSize: "clamp(2rem, 1.4rem + 2.2vw, 3.25rem)"
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  body:
    fontFamily: "Barlow, system-ui, sans-serif"
    fontSize: "1.125rem"
    fontWeight: 400
    lineHeight: 1.6
  lede:
    fontFamily: "Barlow, system-ui, sans-serif"
    fontSize: "1.1875rem"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Barlow, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.01em"
rounded:
  base: "3px"
  bend: "18px"
  fitting: "50%"
spacing:
  gutter: "clamp(16px, 4vw, 48px)"
  indent: "76px"
  indent-compact: "44px"
  pipe-x: "21px"
  section: "clamp(88px, 12vw, 168px)"
  max: "1320px"
components:
  button-primary:
    backgroundColor: "{colors.blue-strong}"
    textColor: "{colors.on-strong}"
    typography: "{typography.label}"
    rounded: "{rounded.base}"
    padding: "0 24px"
    height: "54px"
  button-primary-hover:
    backgroundColor: "{colors.blue-deep}"
    textColor: "{colors.on-strong}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.base}"
    padding: "0 24px"
    height: "54px"
  button-line-hover:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.bg}"
  button-small:
    padding: "0 18px"
    height: "44px"
  input:
    backgroundColor: "{colors.bg}"
    textColor: "{colors.ink}"
    rounded: "{rounded.base}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.base}"
    padding: "0 16px"
    height: "44px"
  chip-checked:
    backgroundColor: "{colors.blue-strong}"
    textColor: "{colors.on-strong}"
  filter-active:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.bg}"
    rounded: "{rounded.base}"
    height: "44px"
  form-card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.base}"
    padding: "clamp(24px, 3.5vw, 48px)"
  mark:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.base}"
    padding: "0 14px 0 12px"
    height: "40px"
  mark-pressed:
    backgroundColor: "{colors.blue-strong}"
    textColor: "{colors.on-strong}"
---

# Design System: Sanitair Verschraegen

## Overview

**Creative North Star: "De leiding"**

The whole site is one installation. A single 2px brand-blue line leaves the VM monogram in the nav, runs down a fixed lane at the left of the content, and branches off with rounded 90-degree elbows and small ring fittings into every heading that matters: the hero headline, each service, the projects, and finally the offerte, where it turns white inside the one full blue field. The line is the argument that one firm connects every trade; nothing else on the page is ornament.

Everything around the line stays quiet and technical. A near-white ground, deep blue-black ink, cool steel grey for secondary copy, and real project photography with square corners. Display type is Barlow Condensed, echoing the condensed lettering of the logo; running text is Barlow at a generous 18px for an older, often mobile audience. Density is low: large section gaps, long left indent, photos given real area.

The page is light only. A `[data-theme="dark"]` override block and dark-logo images remain in the stylesheet and markup, but nothing sets the attribute; treat them as inert, not as a supported theme.

**Key Characteristics:**
- One blue hue, used for the line, the primary action and one closing field.
- A pipe lane at the left; all content indents past it.
- Condensed, heavy, often uppercase display type against plain Barlow text.
- Square photos, 3px rectangles, curves reserved for the pipe.
- Scroll-drawn line with a fully drawn static fallback.

## Colors

A single-hue world: brand blue in three strengths on a cool near-white, with blue-tinted neutrals.

### Primary
- **Logo Blue** (blue): sampled from the original banner. The pipe stroke, ring fittings, nav underline, list ticks, credential rules, icons beside text, focus outlines, the third hero line and other large display text. Its contrast on the ground is 4.23:1, so it never sets small text.
- **Deep Fitting Blue** (blue-strong): every text-bearing blue fill: primary button, checked chip, pressed mark, skip link, marked-count link. 6.02:1 with white.
- **Night Main** (blue-deep): hover state of the primary button and the text colour of the white button on the blue field.
- **Offerte Field** (field): the one full-bleed blue section at the close. Brand blue nudged darker so white body text holds AA (4.98:1). Inside it the pipe turns white.

### Neutral
- **Pipe-Drawing Ink** (ink): all headings and body text, line-button stroke, active filter fill, hover border on inputs.
- **Steel** (steel): lede, section intros, step copy, hints, brand list, footer. 6.21:1 on the ground.
- **Hairline** (hair): fact-list rules, filter borders, picked-projects dashed frame, nav stuck shadow line.
- **Mist** (mist): image placeholders behind figures and project tiles, form status panel.
- **Ground** (bg): page background; also the fill inside ring fittings so the ring reads as a fitting over the line.
- **Surface** (surface): the form card.
- **Error Red** (error): validation border and message only.

### Named Rules
**The One Blue Rule.** Blue is the only hue. Red exists only for form errors. No second accent, no gradients, no tinted section bands except the single blue offerte field.

**The Text-Blue Rule.** Logo Blue draws; Deep Fitting Blue carries text. Any blue fill under white text, or any blue text below large-text size, uses blue-strong.

## Typography

**Display Font:** Barlow Condensed (with Arial Narrow, sans-serif), weights 500/600/700
**Body Font:** Barlow (with system-ui, sans-serif), weights 400/500/600 and 400 italic
Self-hosted woff2 in `assets/fonts/`; Barlow Condensed 700 and Barlow 400 are preloaded.

**Character:** A heavy condensed face that sounds like the van lettering and the logo, set tight and short, paired with a plain, open grotesque for reading.

### Hierarchy
- **Display** (700, clamp(3rem → 5rem), 0.92, uppercase): hero headline, three forced lines on desktop. The realisaties page head runs larger (clamp(3.25rem → 6rem)). Under 900px the hero drops to clamp(2.1rem, 9.2vw, 3.5rem).
- **Headline** (700, clamp(2.5rem → 4.25rem), 0.95): section heads in sentence case; the offerte head uses the same size in uppercase.
- **Title** (700, clamp(2.25rem → 3.75rem), 0.9, uppercase): service names. Step titles are a smaller title (clamp(1.75rem → 2.375rem), 1.05, sentence case).
- **Statement** (600, clamp(2rem → 3.25rem), 1.08): the owners statement and the gallery closing line; condensed prose at speaking size.
- **Body** (400, 1.125rem, 1.6): running text, 34-52ch measures (46ch in services, 52ch in section intros).
- **Lede** (400, 1.1875rem): section intros and contact lead; the hero lede scales to 1.3125rem.
- **Label** (600, 1.0625rem, 0.01em): buttons; form labels 600 at 1rem.
- **Brand list** (Barlow Condensed 500, uppercase, 0.04em tracking, steel): the only tracked uppercase in the system, used for supplier names.

### Named Rules
**The Condensed Voice Rule.** Every heading is Barlow Condensed 700 with line-height at or under 1.05. Uppercase is for the hero, service names, the offerte head and page heads; section heads and step titles stay sentence case.

**The Tabular Phone Rule.** Phone numbers and counts use tabular numerals; the big phone in the offerte field is set at headline size in condensed 700.

## Layout

A centred 1320px container with fluid gutters (clamp(16px, 4vw, 48px)). Inside it, the pipe lane: the main line sits at 21px from the gutter (the centre of the VM monogram), and content starts 76px in. At 900px and below the lane shrinks to 17px / 44px indent. Section rhythm is one large step (clamp(88px, 12vw, 168px)) above each section; sub-blocks use 48-160px clamps.

Compositions use a 12-column grid inside the indent and change per service so the page does not read as repeated cards: text 5 / photos 6 for sanitair, full-width title then photo 5 / text 6 for verwarming, text then a three-photo strip for wellness. The hero is a two-column grid (1.3fr / 0.9fr) with a tall photo overlapped by a smaller one. Projects are a six-column mosaic with 16px gaps; the realisaties gallery is a masonry of CSS columns (3 × 280px).

Breakpoints: 1080px (tighter nav, phone number collapses to icon), 900px (single column, hamburger menu, mobile call bar fixed at the bottom with Bellen and Offerte aanvragen, form card goes edge to edge), 380px (button padding 16px).

### Named Rules
**The Pipe Lane Rule.** Nothing but the line and its branches lives in the left lane. Every section, grid and gallery starts at the indent.

## Elevation & Depth

Flat by default. Depth is carried by layering photos and by the line passing behind fittings, not by shadows on UI. Shadows are soft, tinted with the ink blue (rgb 10 50 75), and limited to things that physically sit on top of something: the overlapping hero photo, the floating mark button on photos, the form card on the blue field, and the open mobile menu. The sticky nav gets only a 1px hairline when it detaches, over a 92% ground with backdrop blur.

### Shadow Vocabulary
- **Photo lift** (`box-shadow: 0 24px 48px -20px rgb(10 50 75 / .45)` plus an 8px ground-coloured outline as a mat): the smaller hero photo overlapping the large one.
- **Card on field** (`box-shadow: 0 40px 80px -40px rgb(10 50 75 / .55)`): the form card inside the blue field; removed under 900px.
- **Floating control** (`box-shadow: 0 6px 18px -8px rgb(10 50 75 / .5)`): the mark button on project photos.
- **Menu drop** (`box-shadow: 0 16px 24px -16px rgb(10 50 75 / .3)`): the open mobile menu panel.

### Named Rules
**The Sits-On-Top Rule.** A shadow is allowed only where one object overlaps another. Sections, lists and tiles stay flat.

## Shapes

Two geometries. Rectangles (buttons, inputs, chips, filters, the form card, the mark button, the status panel) take a barely softened 3px corner; photos and figures are fully square. Curves belong to the pipe: elbows bend on an 18px radius (14px on the compact mobile step branches), fittings are 12px rings with a 2px stroke filled with the ground colour. Fully round shapes appear only for icon-only controls (lightbox buttons, the remove badge on picked thumbnails). The 2px line weight recurs in UI: nav hover underline, link-arrow underline, credential top rules, the 10×2px tick before fact items, focus outlines.

### Named Rules
**The Two Geometries Rule.** Rectangles are 3px or square; curves are pipework. No pill-shaped buttons or tags.

## Components

### Buttons
Solid, plain, workmanlike.
- **Shape:** 3px corners, 54px tall (44px small, 50px in the call bar), 2px border slot on every variant so variants align.
- **Primary:** Deep Fitting Blue fill, white label, 0 24px padding.
- **Line:** transparent with a 2px ink border and ink label; fills ink with ground-coloured text on hover.
- **White:** on the blue field only (realisaties closing band): white fill, Night Main text, pale blue (#e3f1f8) hover.
- **Hover / Focus / Active:** 0.25s colour transitions on the system ease-out; active nudges down 1px; focus is a 2px blue outline offset 3px (white inside the blue field).

### Chips
- **Style:** form multi-select chips are checkbox labels, 44px tall, 1.5px grey border, 3px corners, Barlow 500.
- **State:** hover borders ink; checked fills Deep Fitting Blue with white text. Realisaties filters share the shape with a hairline border and fill ink when pressed, with a steel tabular count.

### Cards / Containers
- **Corner Style:** 3px (form card), square (photos, project tiles).
- **Background:** surface on the blue field; project tiles and figures sit on mist while loading.
- **Shadow Strategy:** see Card on field; nothing else is a card.
- **Internal Padding:** clamp(24px, 3.5vw, 48px).

### Inputs / Fields
- **Style:** ground fill, 1.5px mid-grey stroke, 3px corners, 52px minimum height, Barlow 1.0625rem; label above in 600, optional marker in steel 400.
- **Focus:** border turns Deep Fitting Blue with a 3px 30% blue halo; hover border turns ink.
- **Error:** red border plus a red 0.9375rem message below; empty messages collapse.
- **Picked projects:** a dashed hairline frame holding 76px square thumbnails with a round ink remove badge.

### Navigation
- **Style:** sticky 76px bar (64px under 900px), logo left, four Barlow 500 links, phone with blue icon, small primary button. Links get a 2px blue underline that scales in from the left on hover and for the current page.
- **Mobile:** links hide behind a 44px menu button; the open panel drops below the bar with condensed 600 links at 1.375rem separated by hairlines. A fixed call bar at the bottom carries Bellen (line) and Offerte aanvragen (primary) and hides while the offerte section is visible.

### Mark ("Dit wil ik ook")
A small white control floating at the bottom-right of each project photo: 40px tall, 3px corners, floating-control shadow, bookmark icon. On fine pointers it collapses to the icon and expands its label on tile hover or focus. Pressed, it fills Deep Fitting Blue with a filled bookmark; the marked count appears in the nav and bumps on change, and marked photos travel into the form.

### De leiding (signature)
The pipe system that carries the thesis.
- **Main line:** one 2px blue vertical inside the page run, aligned to the monogram centre, spanning hero to brands.
- **Tap:** any heading marked as a tap grows a branch: an elbow that leaves the main line, rises 56px and turns 90 degrees on an 18px bend toward the heading, ending in a 12px ring fitting level with the first line of text.
- **Hero feed:** a U-shaped run leaves the main line under the hero and rises into the bottom edge of the hero photo, ending in a ring.
- **Manifold:** in the werkwijze, one header pipe runs along the top of the three steps with a vertical drop and ring into each; under 900px each step gets its own elbow instead.
- **On the field:** inside the blue offerte field the line is white, rising from the top of the section into the heading; its ring is filled with the field colour.
- **Motion:** on load the line flows out of the logo (1.1s clip reveal) and the hero branch and ring follow. Where `animation-timeline` is supported, the main line draws with page scroll and each branch, drop and ring draws as its element enters view. Without support, and under reduced motion, every pipe is fully drawn and static.

## Do's and Don'ts

### Do:
- **Do** branch every new major heading off the main line with the tap pattern (elbow on an 18px bend, 12px ring) instead of adding icons or labels above it.
- **Do** start all content at the indent (76px, 44px under 900px) and keep the lane for pipework only.
- **Do** use Deep Fitting Blue (#00699a) for any blue fill carrying text and keep Logo Blue (#0081b8) for line, icons and large display type.
- **Do** keep photos square-cornered on a mist placeholder, and use real project photography.
- **Do** keep the line fully drawn whenever scroll-driven animation is unsupported or reduced motion is requested.
- **Do** keep phone and offerte one tap away: nav phone and button on desktop, fixed call bar under 900px.

### Don't:
- **Don't** introduce a second accent hue, gradients or tinted bands; the blue offerte field is the only coloured section.
- **Don't** draw pipe branches that do not connect back to the main line, or vary the 2px stroke.
- **Don't** use pill-shaped buttons, tags or chips; rectangles stay at 3px.
- **Don't** put shadows on flat content (sections, lists, tiles); shadows mark overlap only.
- **Don't** set small text in Logo Blue; it is 4.23:1 on the ground.
- **Don't** rely on the dark-theme override block; it is inert and the site ships light only.

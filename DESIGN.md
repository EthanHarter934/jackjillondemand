---
name: Jack & Jill On Demand
description: Family-owned Central Oregon property services — The Reliable Neighbor
colors:
  cyan: "#29abe2"
  cyan-bright: "#2bb6f0"
  navy: "#143a6b"
  navy-deep: "#0e2545"
  royal: "#1e63c9"
  ink: "#14161a"
  slate: "#4a5568"
  mist: "#eaf6fd"
  mist-2: "#f4fafe"
  white: "#ffffff"
  line: "#e2e8f0"
typography:
  display:
    fontFamily: "Poppins, system-ui, sans-serif"
    fontSize: "clamp(2.4rem, 5.4vw, 4rem)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "Poppins, system-ui, sans-serif"
    fontSize: "clamp(1.9rem, 4vw, 2.8rem)"
    fontWeight: 700
    lineHeight: 1.1
  title:
    fontFamily: "Poppins, system-ui, sans-serif"
    fontSize: "1.18rem"
    fontWeight: 700
    lineHeight: 1.2
  body:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Poppins, system-ui, sans-serif"
    fontSize: "0.8rem"
    fontWeight: 600
    letterSpacing: "0.18em"
rounded:
  sm: "12px"
  md: "18px"
  lg: "28px"
  pill: "999px"
spacing:
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "48px"
  section: "clamp(3.5rem, 7vw, 6rem)"
components:
  button-primary:
    backgroundColor: "{colors.cyan}"
    textColor: "{colors.white}"
    rounded: "{rounded.pill}"
    padding: "0.85rem 1.5rem"
  button-primary-hover:
    backgroundColor: "{colors.cyan-bright}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.navy}"
    rounded: "{rounded.pill}"
    padding: "0.85rem 1.5rem"
  button-dark:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.white}"
    rounded: "{rounded.pill}"
    padding: "0.85rem 1.5rem"
  card-service:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: "1.7rem"
---

# Design System: Jack & Jill On Demand

## Overview

**Creative North Star: "The Reliable Neighbor"**

Jack & Jill On Demand reads like the most capable, trustworthy person on the block who just happens to do this professionally. The visual system is clear, energetic, and warm — cyan-bright against deep navy anchors every screen in honest confidence, while white-ground layouts and open spacing signal that nothing is hidden. It feels like talking to someone you already trust.

The system is decisive without being aggressive. Pill-shaped buttons, soft card radius, and a structured grid convey the professionalism a Central Oregon homeowner will recognize: organized and local, not corporate. The scroll-reveal is the handshake — unhurried, steady. Caveat script makes a single appearance per hero, humanizing the brand without letting warmth become sloppiness.

The awards strip in full-width navy is a quiet declaration: this is the neighborhood choice. That band runs wall-to-wall, not as decoration, but as a grounding layer that says we've been here and we've been chosen.

**Key Characteristics:**
- Cyan accent on white ground — readable trust, not aggressive
- Pill-shaped CTAs — approachable and action-ready
- Three-level navy-tinted shadow vocabulary
- Caveat script used once per hero for handwritten warmth
- Scroll-reveal at 700ms — unhurried, steady pacing

## Colors

A bright Pacific-sky cyan against deep Oregon-night navy, grounded in near-black ink and open white.

### Primary
- **Pacific Sky Cyan** (`#29abe2`): The action color. Primary buttons, hero headline highlight, eyebrow text, icon chips, hover accents. Appears on ≤15% of any screen.
- **Bright Cyan** (`#2bb6f0`): Hover state for the primary button only. Never used at rest as a background.

### Secondary
- **Oregon Night Navy** (`#143a6b`): Headlines, nav text, service card headings, ghost button text, and the awards strip background.
- **Deep Navy** (`#0e2545`): Family-of-brands section background, hero radial gradient origin.
- **Royal Blue** (`#1e63c9`): Gradient partner for the CTA band and hero radial tint. Not used alone on buttons.

### Neutral
- **Ink** (`#14161a`): Primary h1 and body text. Near-black with warmth — not pure black.
- **Slate** (`#4a5568`): Lead paragraphs, supporting copy, card descriptors.
- **Mist** (`#eaf6fd`): Icon chip backgrounds and section accent tints.
- **Mist-2** (`#f4fafe`): Hero and promise-band gradient backgrounds. The lightest tint.
- **White** (`#ffffff`): Page background, card surfaces, form fields.
- **Line** (`#e2e8f0`): All borders, dividers, and field outlines at rest.

### Named Rules
**The Cyan Economy Rule.** Cyan appears on primary interactive elements, the hero highlight span, and icon highlights only. No cyan section backgrounds. Its rarity is what makes it click.

## Typography

**Display Font:** Poppins (system-ui fallback)
**Body Font:** Inter (system-ui fallback)
**Accent Font:** Caveat (cursive) — `.script` inline spans only, one per hero

**Character:** Poppins brings sturdy, friendly roundness to headings that matches community trust without stiffness. Inter's legibility keeps body copy fast and transparent. No mystery — just clarity.

### Hierarchy
- **Display** (800, clamp 2.4–4rem, lh 1.1, ls –0.02em): Hero h1. One per page. Gets the cyan `.hl` highlight span.
- **Headline** (700, clamp 1.9–2.8rem, lh 1.1): Section h2. Ink on light; white on dark backgrounds.
- **Title** (700, 1.18rem, lh 1.2): Service card h3, info card h3. Navy by default.
- **Body** (400, 1rem, lh 1.6): Lead paragraphs, descriptors, footer copy. Max ~50ch per line.
- **Label** (600, 0.8rem, ls 0.18em, uppercase): Eyebrow text, nav links, pill badge labels. Cyan on light surfaces.

### Named Rules
**The One Script Rule.** Caveat appears only as an inline `.script` span inside a heading — never in a paragraph, never as a heading font itself. One instance per hero maximum.

## Layout

Container max-width 1180px, 24px horizontal padding. Hero: two-column grid (1.05fr / 0.95fr), copy left, visual right, collapses to single column at 920px with the visual first. Services: three-column (two at 920px, one at 640px). Promise band: four-column stat grid (two at 920px). Section vertical rhythm: `clamp(3.5rem, 7vw, 6rem)`. The awards strip breaks the max-width to run edge-to-edge in full navy. Scroll-reveal: 700ms ease, 24px translateY lift, 80ms stagger per `.d1`–`.d4`.

Breakpoints: 920px (tablet — hero stacks, grids collapse to 2-col), 640px (mobile — nav hidden, grids to 1-col, ghost phone button hidden). `prefers-reduced-motion` disables all animation.

## Elevation & Depth

Three navy-tinted shadow levels. All shadows use `rgba(20, 58, 107, ...)` so depth reads as navy depth — the brand color is present even in shadow.

### Shadow Vocabulary
- **Subtle** (`0 2px 8px rgba(20,58,107,.08)`): Card hover warm-up and pill badge ambient.
- **Medium** (`0 12px 30px rgba(20,58,107,.12)`): Hero card, service card on hover, form card.
- **Large** (`0 24px 60px rgba(20,58,107,.18)`): Hero card at rest, floating logo badge. One per view.

### Named Rules
**The Flat-By-Default Rule.** Surfaces are flat at rest. Shadows appear only on hover interaction and on the single hero visual per page. No decorative shadow on static cards.

## Shapes

Pill-shaped buttons (999px radius) are the brand's primary tactile signature — the full loop echoes the brand's approachable personality. Three-step card radius: small 12px (icon chips, secondary UI), medium 18px (service cards, info blocks, form fields), large 28px (hero card, CTA band). Near-square corners are not used in this system.

## Components

### Buttons
- **Shape:** Pill (999px radius), Poppins 600, 0.98rem
- **Primary:** Cyan (`#29abe2`) background, white text, 0.85rem×1.5rem padding, cyan shadow lift
- **Hover / Focus:** –3px translateY, shadow intensifies, cyan-bright background
- **Ghost:** Transparent, navy border at 22% opacity → cyan border and cyan text on hover. Same pill.
- **Dark:** Navy background, white text. Hover deepens to navy-deep with –3px lift.

### Cards / Containers
- **Service Card:** White background, 1px line border at rest, 18px radius, 1.7rem padding. Top cyan→royal gradient bar `scaleX(0→1)` on hover. Icon chip: 52px, 14px radius, mist background, cyan icon, slight rotate on hover.
- **Hero Card:** White, 28px radius, large shadow, 1.4rem padding. Floating logo badge inside: white, 20px radius, medium shadow.
- **Family Cards:** `rgba(255,255,255,.05)` background on navy-deep, medium radius, translucent white border. Hover lifts –6px and brightens.

### Inputs / Fields
- **Style:** Mist-2 background, 1px line border, 10px radius
- **Focus:** Cyan border, 3px cyan glow (`rgba(41,171,226,.15)`), white background
- **Label:** Poppins 600, 0.88rem, navy, above the field

### Navigation
- **Style:** Sticky frosted glass (85% white, 12px blur, saturate 160%), 76px height, 1px line bottom border
- **Links:** Poppins 500, 0.95rem, slate; 2px cyan underline draws left-to-right on hover (250ms)
- **Logo:** 46px logo, Poppins 700 navy brand name, cyan micro-label below
- **Mobile:** Hamburger at 640px, nav-links hidden

### Pill Badges
Credential chips in the hero (Licensed, Bonded, Insured, Best of Bend): white background, 1px line border, pill radius, subtle shadow, Poppins 600 0.8rem navy, 15px cyan icon left.

### Award Strip
Full-width navy band below the hero. Four awards in centered flex row. Poppins 600, 0.92rem white, cyan-bright icons (22px), muted secondary text beneath each label.

## Do's and Don'ts

### Do:
- **Do** use cyan only on primary interactive elements, the hero highlight span, and icon accents. Never as a page background.
- **Do** use pill-shaped buttons for all CTAs — the rounded silhouette is non-negotiable for this brand.
- **Do** include the awards strip (full-width navy band) after the hero on every homepage-level page.
- **Do** animate service card icon chips with a slight –4deg rotate on hover.
- **Do** use `clamp()` for all display type sizes.

### Don't:
- **Don't** use Caveat in body copy or as a heading font — it's a single inline accent span only.
- **Don't** add shadows to static non-interactive elements.
- **Don't** use royal blue as a standalone button color — it belongs in gradients only.
- **Don't** remove the translucent blob shapes from the hero — they're part of the brand's energy.
- **Don't** use colored backgrounds on interior page sections — white ground with cyan accents only.

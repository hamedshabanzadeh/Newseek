---
name: Newseek
description: A minimal, Persian-first news research prompt generator with glassmorphic surfaces and restrained indigo accents.
colors:
  background-primary: "#eef1f8"
  background-secondary: "rgba(255, 255, 255, 0.97)"
  text-primary: "#172033"
  text-secondary: "#687386"
  border-default: "#e3e8f0"
  interactive-primary: "#111827"
  interactive-primary-soft: "#eef1f6"
  accent-primary: "#4f46e5"
  accent-soft: "#eef2ff"
  success-green: "#0f9f6e"
typography:
  display:
    fontFamily: "Vazirmatn, Tahoma, Arial, sans-serif"
    fontSize: "clamp(28px, 4vw, 38px)"
    fontWeight: 900
    lineHeight: 1
    letterSpacing: "-0.8px"
  headline:
    fontFamily: "Vazirmatn, Tahoma, Arial, sans-serif"
    fontSize: "22px"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.35px"
  body:
    fontFamily: "Vazirmatn, Tahoma, Arial, sans-serif"
    fontSize: "13px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Vazirmatn, Tahoma, Arial, sans-serif"
    fontSize: "12px"
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: "0"
    textTransform: "uppercase"
  label-hint:
    fontFamily: "Vazirmatn, Tahoma, Arial, sans-serif"
    fontSize: "12px"
    fontWeight: 400
    lineHeight: 1.7
    color: "{text-secondary}"
spacing:
  xs: "8px"
  sm: "12px"
  md: "16px"
  lg: "24px"
  xl: "32px"
rounded:
  sm: "12px"
  md: "14px"
  lg: "15px"
  xl: "24px"
  pill: "999px"
components:
  button-primary:
    backgroundColor: "{interactive-primary}"
    textColor: "#ffffff"
    rounded: "{rounded.md}"
    padding: "12px 16px"
  button-primary-hover:
    backgroundColor: "{interactive-primary}"
    textColor: "#ffffff"
    rounded: "{rounded.md}"
    padding: "12px 16px"
  button-ghost:
    backgroundColor: "rgba(255, 255, 255, 0.82)"
    textColor: "{text-primary}"
    rounded: "{rounded.sm}"
    padding: "10px 13px"
  button-ghost-hover:
    backgroundColor: "rgba(255, 255, 255, 0.82)"
    textColor: "{text-primary}"
    rounded: "{rounded.sm}"
    padding: "10px 13px"
  button-ai:
    backgroundColor: "#ffffff"
    textColor: "{text-primary}"
    rounded: "{rounded.md}"
    padding: "10px 12px"
  button-ai-hover:
    backgroundColor: "#f8fafc"
    textColor: "{text-primary}"
    rounded: "{rounded.md}"
    padding: "10px 12px"
  input-default:
    backgroundColor: "#fbfcfe"
    textColor: "{text-primary}"
    rounded: "{rounded.lg}"
    padding: "14px"
    height: "48px"
  input-focus:
    backgroundColor: "#fbfcfe"
    textColor: "{text-primary}"
    rounded: "{rounded.lg}"
    padding: "14px"
    height: "48px"
  chip-accent:
    backgroundColor: "{accent-soft}"
    textColor: "#3730a3"
    rounded: "{rounded.pill}"
    padding: "8px 11px"
  card-field:
    backgroundColor: "#fbfcfe"
    textColor: "{text-primary}"
    rounded: "{rounded.lg}"
    padding: "13px"
  panel-glass:
    backgroundColor: "rgba(255, 255, 255, 0.97)"
    textColor: "{text-primary}"
    rounded: "{rounded.xl}"
    padding: "24px"
  panel-glass-mobile:
    backgroundColor: "rgba(255, 255, 255, 0.97)"
    textColor: "{text-primary}"
    rounded: "20px"
    padding: "17px"
  textarea-prompt:
    backgroundColor: "rgba(255, 255, 255, 0.68)"
    textColor: "#243047"
    rounded: "18px"
    padding: "17px"
    height: "410px"
  toggle-off:
    backgroundColor: "#cbd5e1"
    rounded: "{rounded.pill}"
    width: "40px"
    height: "23px"
  toggle-on:
    backgroundColor: "{accent-primary}"
    rounded: "{rounded.pill}"
    width: "40px"
    height: "23px"
---

# Design System: Newseek

## Overview

**Creative North Star: "The Research Studio"**

Newseek's interface is a calm, purposeful workspace where Persian-speaking users focus on researching news without visual distraction. The design feels clear and minimal, using generous spacing, subtle glassmorphic surfaces, and a restrained palette of cool tones anchored by a confident indigo accent. Information hierarchy is strong and consistent; every visual element—from typography to shadow to button state—exists to support clarity and action rather than decoration. The aesthetic is refined and contemporary, never cold: subtle background gradients, precise type pairings, and thoughtful transitions create perceived depth and movement without adding cognitive load.

**Key Characteristics:**
- Minimal, focused workspace free of visual clutter
- Glassmorphism (translucent, blurred surfaces) creates perceived depth
- Strong information hierarchy via typography and spacing
- Cool-toned neutrals with restrained indigo accents
- Confidence over caution; clarity over expression
- Responsive across mobile, tablet, and desktop; RTL-first
- Accessibility baked in (contrast, focus states, semantic HTML)

## Colors

The palette is cool and measured: soft blue-grays for surfaces and text, punctuated by a single confident indigo accent used sparingly for primary actions. Neutrals recede to make content and hierarchy visible.

### Primary (Interactive)
- **Very Dark Blue-Gray** (#111827): Primary call-to-action buttons ("Generate Prompt"), high-confidence, trust-building. Dark but not black; readable white text on all backgrounds.
- **Focused Indigo** (#4f46e5): Active states, form focus rings, accent highlights, chip backgrounds. Used on ~10% of any screen or less. Its rarity is the point—it draws the eye to the next action.

### Soft / Supportive
- **Background Mist** (#eef1f8): Primary page background. Neutral, calm, recedes visually. Pairs with subtle radial gradients (purple + green at edges) for perceived depth.
- **Panel White** (rgba(255, 255, 255, 0.97)): Modal, card, and dialog backgrounds. Nearly opaque; slight transparency supports glassmorphism effect.
- **Accent Halo** (#eef2ff): Background for chip and accent UI elements. Very light purple, pairs with darker indigo text.

### Neutral / Structure
- **Calm Clear** (#687386): Secondary copy, hints, placeholder text. Readable at 13px but visually quiet; never used for primary labels.
- **Border Subtle** (#e3e8f0): Dividers, card borders, input borders. Very light; provides structure without weight.
- **Success Green** (#0f9f6e): Status indicators only ("Auto-Save On" pill). Muted green, readable and distinct.

### Named Rules
**The Indigo Reserve Rule.** Accent indigo (#4f46e5) is used exclusively for:
1. Primary call-to-action buttons ("Generate Prompt").
2. Form focus rings and input outlines (4px halo).
3. Chip backgrounds (topic tags).
4. Active state toggles.
5. Link text in footers and help copy.

Never use indigo for disabled states, secondary content, or decorative elements. Its scarcity signals importance.

**The Neutral Retreat Rule.** On any given screen, no more than two neutral colors should be visually primary. The rest support hierarchy and structure:
- Text: Always use primary text (#172033) for headers and primary copy.
- Secondary text: Use muted gray (#687386) only for hints, helper text, and affordances.
- Surfaces: Background Mist for large areas; Panel White for interactive sections; Border Subtle for structure only.

## Typography

**Display Font:** Vazirmatn (Persian-native, 900 weight for headlines)
**Body Font:** Vazirmatn (400–700 weight)
**Fallback Stack:** Tahoma, Arial, sans-serif

**Character:** Vazirmatn is geometric, modern, and designed for Farsi. Paired with ample line-height and letter-spacing, it feels spacious and easy to read. The typeface is neither decorative nor cold; it is friendly and professional. Weight choices are deliberate: 900 for top-level headlines (confidence), 700 for section heads (authority), 400 for body text (clarity).

### Hierarchy
- **Display** (900, clamp(28px, 4vw, 38px), 1): Wordmark "Newseek" or app title. Centered, commanding presence without aggression. Used once per screen.
- **Headline** (700, 22px, 1.1): Section headers ("چه چیزهایی را دنبال می‌کنی؟", "جستجوی اخبار را تنظیم کن"). Bold, scannable, anchors each section.
- **Label/Eyebrow** (800, 12px, 1.2, uppercase): Step counters ("۱. علایق خبری"), field labels ("بازه زمانی"), status pills. Compact, hierarchical cue. Always 12px.
- **Body** (400, 13px, 1.6): Paragraph copy, helper text, hints. Default size; comfortable to read; generous line-height.
- **Label Hint** (400, 12px, 1.7): Helper text under fields ("موضوع‌ها در همین مرورگر ذخیره می‌شوند."). Slightly lighter than body; reads secondary without confusion.

### Named Rules
**The Single Typeface Rule.** Newseek uses Vazirmatn exclusively. No serif fallback, no hand-crafted alternatives. This guarantees visual coherence across browsers and platforms.

**The Weight Intention Rule.** Weight is not for decoration:
- 300 or 400: Never. Not readable at default sizes.
- 500 or 600: Sparingly, for slight emphasis within body copy.
- 700+: Section headers, action labels, confident affordances.

**The Spacing Abundance Rule.** Every text element gets ample line-height (1.2 minimum) and letter-spacing where appropriate. Newseek is never cramped.

## Layout

Newseek uses a centered column layout optimized for Persian and responsive across all devices.

**Container:** `min(920px, calc(100% - 32px))`—max 920px wide, responsive margins that shrink on mobile to 16px each side.

**Grid System:**
- **Main grid:** 1 column (centered). All sections stack vertically.
- **Settings grid:** 2 columns desktop (grid-template-columns: repeat(2, minmax(0, 1fr))), 1 column mobile.
- **AI model buttons grid:** 5 columns desktop, 2 columns mobile, 8px gap.

**Spacing & Rhythm:**
- Section padding: 24px (desktop), 17px (mobile)
- Margin between sections: 18px
- Input/button height: 48px (comfortable touch target on mobile)
- Gap between related inputs: 9–10px
- Card padding: 13px (compact, efficient use of space)

**Vertical Rhythm:**
- Header to section: 24px margin-bottom
- Subsection to content: 14–20px margin-bottom
- Field to next field: 10–15px gap (via grid/flexbox, never margin collapsing)
- Divider: 23px margin top/bottom (symmetrical breathing room)

**Responsive Breakpoint:** 700px (targeting tablets and below)
- Container width compresses to full width minus 20px.
- Grid columns collapse to 1.
- AI button grid: 2 columns (Grok button spans both and centers).
- Panel padding: 17px (instead of 24px).
- Font sizes for headlines slightly reduce.
- Status pills hide (display: none).

**RTL Primacy:** Direction is `rtl` on the root `<html>`. All padding, margin, text-align, and flex behavior account for RTL. Flexbox `gap` and `flex-direction` work naturally with RTL; no hacky `direction: ltr` overwrites except where explicitly needed (ltr wordmark).

## Elevation & Depth

Newseek uses glassmorphism and translucency to create layering without relying on harsh shadows or harsh color shifts.

**Shadow Vocabulary:**
- **Surface shadow:** `0 18px 55px rgba(31, 41, 55, 0.08)`—Used on `.panel`, cards, and major components. Very subtle, ambient. Suggests proximity without overwhelming.
- **Hover/lift shadow:** `0 13px 32px rgba(17, 24, 39, 0.2)`—Appears on `:hover` for buttons and interactive elements. Slightly darker and larger than surface shadow, signals interaction.
- **Inset highlight:** `inset 0 1px 0 rgba(255, 255, 255, 0.75)`—Subtle top-inset on `.prompt-glass` and `.prompt-output` to suggest a light source from above.
- **Card/input focus:** `0 0 0 4px rgba(79, 70, 229, .08)`—Indigo halo on focused inputs and fields. Very soft, doesn't overpower.

**Glassmorphism Layer:**
- `.panel`: `backdrop-filter: blur(14px) saturate(125%); -webkit-backdrop-filter: blur(14px) saturate(125%);` + `background: rgba(255, 255, 255, 0.97)` + `border: 1px solid rgba(226, 232, 240, 0.92)`.
- `.prompt-glass`: Richer: `background: linear-gradient(135deg, rgba(255, 255, 255, 0.74), rgba(238, 242, 255, 0.62)); backdrop-filter: blur(24px) saturate(125%);` with `::before` pseudo-element (decorative purple circle, filtered).

**Depth Strategy:** Surfaces feel layered not through harsh shadows but through:
1. **Translucency:** Panels are 97% opaque, allowing background gradients to peek through.
2. **Blur:** Backdrop-filter blur creates perceived distance.
3. **Subtle gradients:** Background radial gradients (purple at top-right, green at bottom-left) add visual movement without clutter.
4. **Borders:** 1px light borders separate interactive surfaces from the background.
5. **Interaction response:** Buttons translate up 1px on `:hover` (not a click animation, just a subtle lift).

**Named Rules:**
**The Flat-By-Default Rule.** Surfaces are flat at rest. Shadows, blur, and color shifts appear only as response to state (`:hover`, `:focus`, `:active`). There are no "floating" cards with heavy drop shadows.

**The Translucent Surface Rule.** Never paint a fully opaque surface. Always use `rgba()` with transparency and a backdrop-filter so the layers below are subtly visible. This creates perceived depth without visual separation anxiety.

## Shapes

Newseek's corner radius vocabulary is minimal and purposeful: square corners are not used.

**Border Radius Scale:**
- **12px (`--radius-md` renamed to `rounded-sm`):** Ghost buttons, status pills, small UI affordances. Slightly rounded; not aggressive.
- **14px (`rounded-md`):** Input fields, primary buttons, most interactive elements. The workhorse radius; suggests interaction without being decorative.
- **15px (`rounded-lg`):** Card containers, field cards, section panels. Slightly more rounded than inputs; comfortable, refined.
- **24px (`rounded-xl` / `--radius-lg`):** Major panels (`.panel`, `.builder-panel`, `.handoff-panel`), prompt output glass. Distinctly rounded; signals "container" or "workspace."
- **999px (`rounded-pill`):** Toggles, chips, pills, and fully rounded affordances. Used only for pill-shaped elements (topic chips, status pills).

**Named Rules:**
**The Consistent Roundness Rule.** Never use an arbitrary radius not in the scale. The rhythm of corners creates visual coherence.

**The Pill-for-Chips Rule.** Tags, chips, and status indicators are always `border-radius: 999px`. This creates a distinct, memorable affordance that is different from panel corners.

## Components

### Buttons

**Primary Action Button** (`.primary-btn`, `.generate-btn`)
- Background: `{interactive-primary}` (#111827)
- Text color: #ffffff
- Padding: 0 16px (height: 48px via `display: flex; align-items: center; justify-content: center`)
- Border: none
- Border-radius: `{rounded.lg}` (14px or 15px)
- Font weight: 700–800 (confident)
- Transition: 0.18s ease
- `:hover`: Transform -1px (lift), slightly brighter shadow
- `:active`: Revert transform to 0 (press down)
- Used for: "Generate Prompt", "Update" (primary, single action per screen)

**Ghost Button** (`.ghost-btn`, `.copy-btn`)
- Background: `rgba(255, 255, 255, 0.82)`
- Text color: `{text-primary}`
- Border: 1px solid `{border-default}`
- Padding: 10px 13px
- Border-radius: `{rounded.sm}` (12px)
- Font weight: 400–500
- Transition: 0.18s ease
- `:hover`: Border color #cdd4df, transform -1px (lift)
- Used for: Secondary actions, copy buttons, dismiss actions

**AI Model Button** (`.ai-btn`)
- Background: #ffffff
- Border: 1px solid `{border-default}`
- Border-radius: `{rounded.md}` (14px)
- Padding: 10px 12px (height: ~68px, flexbox column)
- Transition: 0.16s ease (background, border, box-shadow, transform)
- `:hover`: Background #f8fafc, border #94a3b8, shadow 0 8px 18px rgba(15, 23, 42, 0.07)
- `:active`: Transform 1px down, background #f1f5f9, no shadow
- Used for: AI provider selection (ChatGPT, Claude, Gemini, etc.)

### Inputs & Form Fields

**Text Input** (`.topic-entry-row input`)
- Height: 48px (touch-friendly)
- Padding: 0 14px
- Border: 1px solid `{border-default}`
- Border-radius: `{rounded.lg}` (14px)
- Background: #fbfcfe (very light, almost white)
- Outline: none (focus ring via box-shadow)
- `:focus`: Border-color rgba(79, 70, 229, 0.6), box-shadow 0 0 0 4px rgba(79, 70, 229, 0.08)
- Font: inherit (Vazirmatn)

**Select Dropdown** (`.field-card select`)
- Border: 0 (transparent)
- Background: transparent (inherits card background)
- Color: `{text-primary}`
- Outline: none
- Font weight: 700 (emphasizes selection)
- Contained in `.field-card` (rounded 15px, padding 13px, background #fbfcfe, border 1px solid `{border-default}`)

**Textarea / Prompt Output** (`.prompt-output`)
- Height: 410px–620px (resizable)
- Padding: 17px
- Border: 1px solid rgba(214, 221, 234, 0.9)
- Border-radius: 18px
- Background: `rgba(255, 255, 255, 0.68)`
- Color: #243047
- Line-height: 2 (comfortable reading on long prose)
- Direction: rtl (Persian text)
- Resize: vertical (user can adjust height)
- Outline: none (focus ring via box-shadow)
- `:focus`: Border-color rgba(79, 70, 229, 0.42), box-shadow 0 0 0 4px rgba(79, 70, 229, 0.06)

### Chips & Tags

**Topic Chip** (`.topic-chip`)
- Display: inline-flex, align-items: center, gap: 8px
- Background: `{accent-soft}` (#eef2ff)
- Color: #3730a3 (darker indigo)
- Border: 1px solid #dfe3ff
- Border-radius: `{rounded.pill}` (999px)
- Padding: 8px 11px
- Font size: 13px, font-weight: 700
- Close button (child `button`): 20x20px, circular, background rgba(55, 48, 163, 0.08)

**Status Pill** (`.status-pill`)
- Color: `{success-green}` (#0f9f6e)
- Background: #ecfdf5 (very light green)
- Border: 1px solid #d1fae5
- Border-radius: `{rounded.pill}` (999px)
- Padding: 6px 9px
- Font size: 11px
- Used for: "Auto-Save On"

### Toggle Switch

**Toggle Container** (`.toggle-row`)
- Display: flex, gap: 10px
- Padding: 13px
- Border: 1px solid `{border-default}`
- Border-radius: 15px
- Background: #fbfcfe

**Toggle UI** (`.toggle-ui`)
- Width: 40px, height: 23px
- Border-radius: `{rounded.pill}` (999px)
- Background: #cbd5e1 (default gray)
- `:checked`: Background `{accent-primary}` (#4f46e5)
- `::after` pseudo-element: 17x17px white circle, shadow, positioned right with 3px padding, slides left on `:checked`

**Toggle Label** (`.toggle-row strong` / `small`)
- Strong: 13px, font-weight: 700 (bold label)
- Small: 12px, line-height: 1.8, color `{text-secondary}` (hint text)

### Panels & Containers

**Builder Panel** (`.panel.builder-panel`)
- Background: `{background-secondary}` (rgba(255, 255, 255, 0.97))
- Border: 1px solid rgba(226, 232, 240, 0.92)
- Border-radius: `{rounded.xl}` (24px)
- Box-shadow: `{shadow}` (0 18px 55px rgba(31, 41, 55, 0.08))
- Backdrop-filter: `blur(14px) saturate(125%)`
- Padding: 24px (17px on mobile)

**Prompt Glass** (`.prompt-glass`)
- Background: `linear-gradient(135deg, rgba(255, 255, 255, 0.74), rgba(238, 242, 255, 0.62))`
- Border: 1px solid rgba(255, 255, 255, 0.7)
- Border-radius: `{rounded.xl}` (24px)
- Box-shadow: 0 20px 60px rgba(79, 70, 229, 0.11), inset 0 1px 0 rgba(255, 255, 255, 0.8)
- Backdrop-filter: `blur(24px) saturate(125%)`
- Padding: 22px
- `::before`: Decorative purple circle (210x210px, opacity 0.1, blurred), positioned top-left

### Section Heading

**Section Head** (`.section-head`)
- Display: flex, justify-content: space-between, gap: 14px
- Align-items: flex-start
- Margin-bottom: 20px (14px on mobile)

**Eyebrow Label** (`.eyebrow`)
- Color: `{accent-primary}` (#4f46e5)
- Font weight: 800
- Font size: 12px
- Uppercase convention

**Section H2** (`.section-head h2`)
- Margin: 4px 0 0
- Font size: 22px (19px on mobile)
- Font weight: 700
- Letter-spacing: -0.35px

## Do's and Don'ts

### Do ✅
- Use indigo accent sparingly; it draws attention and signals the next action.
- Center all layouts and use `min()` for responsive width.
- Maintain 48px minimum height on interactive elements (buttons, inputs) for touch-friendly mobile.
- Use `backdrop-filter: blur()` on translucent surfaces for glassmorphism.
- Keep border-radius consistent with the defined scale (12px, 14px, 15px, 24px, 999px).
- Pair Vazirmatn with generous line-height (1.2 minimum for headlines, 1.6 for body).
- Use `rgba()` colors to preserve layering; never paint fully opaque surfaces.
- Translate buttons up 1px on `:hover`, never scale or change dimensions.
- Set `direction: rtl` on the root and let flexbox/grid respond naturally; avoid rtl overrides.
- Provide clear focus rings (4px indigo halo) on all interactive elements.

### Don't ❌
- Don't use indigo for secondary or disabled states; reserve it for primary actions.
- Don't create fully opaque surfaces; always use transparency + backdrop-filter.
- Don't use serif fonts or hand-crafted typography variants; Vazirmatn only.
- Don't add unnecessary visual weight via shadows or gradients; keep it minimal.
- Don't force LTR layout overrides; design RTL-first.
- Don't omit focus rings or hover states; accessibility is not optional.
- Don't use corners smaller than 12px or arbitrary radii outside the scale.
- Don't mix shadow styles (use the defined vocabulary only).
- Don't add decorative elements that don't support clarity or information hierarchy.
- Don't use animation longer than 0.22s or more complex than a simple translate/fade; motion should be subtle and responsive.
- Don't forget: every visual detail serves the product's core purpose (help users research news with clarity).

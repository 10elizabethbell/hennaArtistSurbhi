---
name: Henna Artist Surbhi
description: A calm, personal booking page for a one-woman henna artist in North Brunswick, NJ.
colors:
  sage-paper: "#f3f5f1"
  card-white: "#ffffff"
  leaf-field: "#e3e9e2"
  henna-leaf: "#1f4d3c"
  deep-leaf: "#123227"
  ink: "#123227"
  body-text: "#2c3a33"
  soft-text: "#4f5d55"
  on-dark: "#f7f4ec"
  on-dark-soft: "#d2e6d9"
  karwachauth-gold: "#e6b04a"
  gold-bright: "#f0c46a"
  gold-ink: "#7e5410"
  hairline: "rgba(18,50,39,.12)"
  focus: "#1f4d3c"
  error: "#a8261c"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(40px, 11.4vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.2
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "13px"
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: "0.08em"
rounded:
  focus: "6px"
  field: "10px"
  card: "24px"
  pill: "999px"
spacing:
  gutter-phone: "20px"
  gutter-desktop: "40px"
  band-phone: "64px"
  band-desktop: "96px"
  stack-sm: "16px"
  stack-md: "28px"
  column-gap: "72px"
components:
  button-primary:
    backgroundColor: "{colors.karwachauth-gold}"
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.gold-bright}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.title}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  input-text:
    backgroundColor: "{colors.leaf-field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.leaf-field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card-white}"
  form-card:
    backgroundColor: "{colors.card-white}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  photo-card:
    backgroundColor: "{colors.deep-leaf}"
    rounded: "{rounded.card}"
  float-text-circle:
    backgroundColor: "{colors.karwachauth-gold}"
    textColor: "{colors.ink}"
    size: "60px"
---

# Design System: Henna Artist Surbhi

## Overview

**Creative North Star: "The Quiet Leaf"**

A phone-first page built from whole-width bands of colour, the way a henna cone lays down leaf and stain: green grounds, warm paper between them, one festival gold. Nothing competes with her photograph. Type is soft and round (Cal Sans) at display sizes and plain system text everywhere else, so the page reads as one person speaking, not a salon brochure.

Density is low. Each band carries one idea, one heading, and at most one action. The green bands carry a faint 135-degree line texture, so the colour feels like cloth rather than a flat fill. Depth comes from colour changes between bands, not from stacked cards; only her photo and the floating text circle cast shadows.

Green, never wine: the system is deliberately cool-leafed so it cannot be mistaken for a wine/rani/marigold competitor. The warm red-brown of real henna stain lives in her photography, not in the UI.

**Key Characteristics:**
- Full-bleed bands alternating light (sage paper) and dark (henna-leaf or deep-leaf green).
- One accent, Karwachauth gold, used as a fill; a darker gold ink carries it as text on light.
- Cal Sans at weight 400 for every heading, button, label-on-form and phone number; system sans for running text.
- Pills and generous 24px cards; no hard edges anywhere except hairline rules in the facts list.
- Motion is one entrance (the hero heading's letters bouncing in) and one small fade-up below the fold.

## Colors

Two greens, a sage paper, and one gold; everything else is a tint of the deep green.

### Primary
- **Karwachauth Gold** (karwachauth-gold): the only accent. Fills primary buttons, the floating text circle, the arrow disc on hover and text selection. On dark bands it may also be text (the accent word in a heading, the phone icon, footer link hover).
- **Bright Gold** (gold-bright): hover fill for the primary button only.
- **Gold Ink** (gold-ink): gold as text or icon on light grounds (header phone icon, accent words on paper, close-band phone icon and hover). Passes 5.8:1 on paper.

### Secondary
- **Henna Leaf** (henna-leaf): the hero band (textured) and, after the open house ends, the close band (untextured). Also the Instagram glyph colour and the text caret.
- **Deep Leaf** (deep-leaf): the booking band and footer, always with the diagonal texture; also the photo card's loading ground.

### Neutral
- **Sage Paper** (sage-paper): page ground, header, the open-house and close bands, and the browser theme colour.
- **Card White** (card-white): the booking form card and the Instagram row inside the hero.
- **Leaf Field** (leaf-field): the resting fill of text inputs and chips on the white form card.
- **Ink** (ink): every heading on light, all text on gold, and the selected-chip fill. Same value as Deep Leaf, different role.
- **Body Text** (body-text): running text on paper.
- **Soft Text** (soft-text): secondary text on light (ledes, hints, placeholders, small labels).
- **On Dark** (on-dark) and **On Dark Soft** (on-dark-soft): headings and running text on green bands. The hero H1 is pure white.
- **Hairline** (hairline): 1px rules between open-house facts.
- **Focus** (focus): outline and border colour for focus and hover on light surfaces.
- **Error** (error): field error text and border only.

### Named Rules
**The Gold Fills Rule.** Gold is a fill on any band; as text it appears only on green. On paper or white, gold text and icons use Gold Ink.

**The Alternating Bands Rule.** Bands alternate light and dark top to bottom. When a band is removed (the open house after `CONFIG.EVENT_END`), re-colour the neighbours so two light or two dark bands never touch: booking goes to paper, close goes to henna leaf.

**The Leaf Not Wine Rule.** UI grounds and accents stay green and gold. Red-brown appears only as the henna stain in her photographs.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** system sans (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** A rounded, friendly display face at a single weight, set against invisible native body text, so the headings carry the voice and the reading text gets out of the way.

### Hierarchy
- **Display** (400, clamp(40px, 11.4vw, 80px) on phones, clamp(56px, 5.6vw, 76px) from 1024px, line-height 1.02, max 13ch): the hero H1 only, white on henna leaf.
- **Headline** (400, clamp(30px, 7.6vw, 48px), 1.08): one H2 per band. The close band's big phone number (clamp(30px, 9vw, 52px), line-height 1) sits at this level.
- **Title** (400, 18px, 1.2): Cal Sans for buttons, form labels and legends, the header phone number (18px, 20px on desktop) and the brand name (23px, 26px on desktop). Open-house fact values step up to clamp(21px, 5.8vw, 26px).
- **Lede** (system, clamp(17px, 4.6vw, 19px)): the paragraph under a band heading, max 38ch; the hero promise runs clamp(17px, 4.7vw, 20px) at 1.5, max 32ch (40ch on desktop).
- **Body** (system 400, 16px, 1.7): all running text. Inputs use 16px so iOS never zooms.
- **Label** (system 600, 13px, 0.08em, uppercase): open-house fact terms (Dates, Timing, Where). The brand subline uses the same treatment at 11px, 0.1em.
- **Small** (system, 14px): field hints, errors, the after-submit note, the Instagram handle.

### Named Rules
**The One Weight Rule.** Cal Sans is only ever weight 400. Hierarchy comes from size and from the switch between display and system faces, never from bolding the display face.

**The Spoken Number Rule.** Phone numbers are set in Cal Sans with a phone icon, never in body text, and never wrap.

## Layout

A single 1160px max-width container with a 20px gutter on phones and 40px from 760px. Bands pad 64px top and bottom on phones and 96px from 760px; the hero runs 56/64px, then 80/96px.

Phones get one column throughout. Hero buttons stack full width; the photo card sits under them (max 460px wide) with the Instagram row directly beneath. From 760px the hero buttons sit side by side (min 220px). From 1024px the system goes two-column with a 72px column gap: hero copy beside a 400px photo column; open-house heading and CTA left, facts right; booking heading (sticky at 40px) beside a wider form (1fr : 1.2fr, 64px gap); close heading left, big phone number bottom-right.

Stacks use a small set of gaps: 16px within a heading group, 20px in the hero copy, 22px between form fields, 28px before a band's CTA. Text measures are capped (13ch display, 32 to 40ch ledes, 640px heading group, 560px facts, 600px form).

All fixed elements respect safe-area insets; the footer pads 96px plus the bottom inset so the floating circle never covers its links.

## Elevation & Depth

Flat by default. Depth comes from band colour and the diagonal line texture (`repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`), which sits on the hero, booking band and footer. Two things lift, and only two.

### Shadow Vocabulary
- **Photo lift** (`box-shadow: 0 18px 40px rgba(6,22,16,.35)`): her work photo in the hero, so it reads as a held print on the green.
- **Float lift** (`box-shadow: 0 10px 28px rgba(10,30,22,.3)`): the floating text circle, to separate it from whatever band it is over.

### Named Rules
**The Two Lifts Rule.** Only the work photo and the floating circle cast shadows. Cards, buttons, inputs and the Instagram row stay flat.

**The Faint Thread Rule.** The diagonal texture is barely visible (3.5% white). It belongs to green bands; paper bands are never textured.

## Shapes

Soft and round throughout. Containers use a 24px radius (form card, photo card); the Instagram row uses 20px. Every button and chip is a full pill. Inputs use a gentler 10px. Circles are reserved for icon discs: the 44px arrow disc and the 60px floating circle. The focus outline is drawn with a 6px radius (round on the circle). The only straight lines in the system are the 1px hairlines between open-house facts.

Icons are inline SVG line drawings, stroke 2 to 2.6, round caps and joins, coloured by `currentColor` (arrow, phone, chat bubble, Instagram).

## Components

### Buttons
Big, round and thumb-sized.
- **Shape:** full pill, 56px minimum height, 26px side padding, 2px border, Cal Sans 18px. An optional 20px icon leads the label with a 10px gap.
- **Primary:** gold fill, ink text, gold border. Used for "Book your slot", the open-house CTA and the form submit (full width on phones and in the form).
- **Ghost:** transparent, on-dark text, 70% on-dark border. Only on green (the hero's "Text Surbhi").
- **Hover (pointer devices only):** primary goes to bright gold; ghost border goes white over a 10% white wash; in the form, the submit also gains a 2px focus-colour outline.
- **Active:** scales to 0.98 over 120ms. Colour transitions run 200ms.
- **Focus:** 3px outline offset 3px; focus green on light, gold on green bands.

### Chips
- **Style:** pill radio labels, 48px tall, leaf-field fill, 2px transparent border, system 16px ink text, 10px gaps, wrapping. The native radio is visually hidden but stays focusable.
- **State:** hover draws a focus-green border; selected inverts to an ink fill with white text; keyboard focus draws a 3px outline.

### Cards / Containers
- **Form card:** white, 24px radius, padding clamp(20px, 5vw, 32px), no border, no shadow, sitting on the deep-leaf band.
- **Photo card:** 3:4 portrait crop of her real work (never stretched to a background), 24px radius, photo lift shadow.
- **Instagram row:** white, 20px radius, at least 76px tall, under the photo. Instagram glyph in henna leaf, a Cal Sans line ("Click to see more of my work.") with the handle in 14px soft text beneath, and a 44px arrow disc on the right that turns gold on hover and focus.

### Inputs / Fields
- **Style:** leaf-field fill, 2px transparent border, 10px radius, 52px minimum height (textarea 110px, vertical resize), system 16px ink text, soft-text placeholders. Labels and legends in Cal Sans 18px; "(optional)" in 14px soft text beside them.
- **Hover / Focus:** border turns focus green; no outline glow.
- **Error:** border and a 14px message in error red appear only after submit; the error clears as soon as the field has text.

### Navigation
- **Header:** paper band, 64px tall (76px desktop). Brand left as a two-line lockup (Cal Sans "Surbhi" over an uppercase 11px "Henna artist"); tap-to-call number right with a gold-ink phone icon. No menu. All targets at least 44px tall.
- **Footer:** deep-leaf textured band, on-dark-soft text, one line of identity and an "Elsewhere" link row in on-dark that turns gold on hover.

### Eyebrow pill
Ellie's house-style choice (pitch-site calm style, after lpmr.co.uk, 2026-10-19), kept even though Impeccable bans kickers. A `<p>`, never a heading: 14px system 500, 9px × 14px padding, pill radius, a 7px gold dot, a faint ink tint on paper (`rgba(18,50,39,.06)`) or a 12% white tint on green. No arrow, no hover, no shadow, so it can't read as a button. Used above the hero H1 and a few band headings only ("Karwachauth open house · Oct 26–28" / "Henna by Surbhi" after the event, "Three days only", "Book by text").

### Open-house facts band
A time-bound band on paper: a headline, a definition list of three facts (uppercase label left in a 96px column, Cal Sans value right, hairlines between), a "Limited slots" line and a primary button that pre-selects the Karwachauth chip. After `CONFIG.EVENT_END` it is removed, the hero's open-house line swaps to its `data-after` text, and the bands re-colour per the Alternating Bands Rule.

### Close band
Paper band (henna leaf after the event) with the artist's name as a headline, one soft line of reassurance, and the phone number at headline size with a gold-ink (gold on green) icon.

### Floating text circle
A 60px gold circle with an ink chat icon, fixed 16px from the bottom-right plus safe-area inset. It slides up from 120px below (350ms, `cubic-bezier(.2,.8,.2,1)`) once the hero leaves view, and slides away while the form is on screen. When hidden it is removed from the tab order. One circle, never a bottom bar.

### Motion
- **Hero heading bounce-in:** with JS, each letter of the H1 slides in from 50px right with an overshoot (1s, `cubic-bezier(.34,1.56,.64,1)`), 20ms apart; words never break. When the last letter lands, the plain heading is restored so kerning and selection come back. The accessible name is the full sentence throughout.
- **Fade-up:** elements that start below the first screen rise 12px and fade in over 400ms ease-out as they enter. Anything visible at load is never hidden.
- **Reduced motion:** no letter split, no fade-up (everything visible in place), no button or float transitions, no smooth scrolling.

## Do's and Don'ts

### Do:
- **Do** alternate light and dark bands, and re-colour neighbours whenever a band is added or removed.
- **Do** use Karwachauth gold as a fill, with ink text on it; switch to gold ink for gold text on paper or white.
- **Do** put the diagonal line texture on green bands only (hero, booking, footer).
- **Do** set headings, buttons, form labels and phone numbers in Cal Sans 400, and everything else in system sans at 16px/1.7.
- **Do** keep every touch target at least 44px tall (buttons 56px, chips 48px, inputs 52px).
- **Do** show her real work at its own 3:4 shape inside a 24px-radius card with the photo lift.
- **Do** restrict hover styles to `(hover: hover)` so taps don't leave them stuck on.
- **Do** keep content visible at rest; motion only enhances what JS and motion preferences allow.

### Don't:
- **Don't** use wine, rani pink or marigold as UI colours; red-brown belongs only to the henna stain in her photos.
- **Don't** put gold text (#e6b04a) on paper or white.
- **Don't** add shadows beyond the photo lift and float lift.
- **Don't** bold Cal Sans or add a second display weight.
- **Don't** stretch a portrait photo into a full-bleed hero background.
- **Don't** replace the floating circle with a sticky bottom bar, or show it while the form is in view.
- **Don't** hide first-screen content behind a fade-in.

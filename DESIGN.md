---
name: Alex Mudge — Data & Insights Lead
description: A CV-first personal record for an Oxford-based Data & Insights Lead — one professional record card, project work filed as attached exhibits.
colors:
  ink: "#1c2530"
  ink-light: "#dfe6ec"
  ink-dim: "#4b5a6b"
  ink-dim-dark: "#97a3af"
  ink-muted: "#576573"
  ink-muted-dark: "#8b96a2"
  stamp: "#a3242f"
  stamp-dark: "#e2555f"
  paper: "#e9edf1"
  paper-dark: "#14181d"
  paper-2: "#f4f6f8"
  paper-2-dark: "#1b2129"
  paper-deep: "#d7dee5"
  paper-deep-dark: "#0c0f13"
  rule: "rgba(28, 37, 48, 0.20)"
  rule-strong: "rgba(28, 37, 48, 0.40)"
typography:
  name:
    fontFamily: "Source Serif 4, Georgia, serif"
    fontSize: "clamp(1.7rem, 3.4vw, 2.35rem)"
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: "-0.01em"
  heading:
    fontFamily: "Courier Prime, Courier New, monospace"
    fontSize: "0.82rem"
    fontWeight: 700
    letterSpacing: "0.1em"
  body:
    fontFamily: "Source Serif 4, Georgia, serif"
    fontSize: "1.02rem"
    fontWeight: 400
    lineHeight: 1.85
  field:
    fontFamily: "Courier Prime, Courier New, monospace"
    fontSize: "0.82rem"
    fontWeight: 400
    letterSpacing: "0.02em"
  label:
    fontFamily: "Courier Prime, Courier New, monospace"
    fontSize: "0.63rem"
    fontWeight: 700
    letterSpacing: "0.1em"
rounded:
  none: "0px"
spacing:
  sm: "0.75rem"
  md: "1.5rem"
  lg: "2.25rem"
  xl: "2.5rem"
components:
  stamp-status:
    backgroundColor: "transparent"
    textColor: "{colors.stamp}"
    rounded: "{rounded.none}"
    padding: "0.4rem 0.75rem"
  exhibit-card:
    backgroundColor: "{colors.paper-2}"
    rounded: "{rounded.none}"
    padding: "1.5rem"
  release-btn-primary:
    backgroundColor: "transparent"
    textColor: "{colors.stamp}"
    rounded: "{rounded.none}"
    padding: "0.7rem 1.4rem"
---

# Design System: Alex Mudge — Data & Insights Lead

## Overview

**Creative North Star: "The Personnel Record"**

The site is one professional record, not a portfolio grid. It reads like an institutional personnel/records-office document: a bordered record card holds identity and career facts in a real field grid, career history sits in a service-record table, capabilities read as a signed-off competency checklist, and project work is filed underneath as numbered, staple-marked exhibits — evidence attached to the record, not the record itself.

This is a deliberate replacement of an earlier dark, neon-cyan, terminal/hacker-console identity, made on the explicit direction to remove that look entirely. Nothing here is dark-mode-first, glowing, particle-animated, or gradient-driven. Depth comes from real stacked-paper offset (two faint sheets behind the record) and 1px rule lines, never from colored glow or blur. Color is restrained to two neutral inks (paper stock and body ink) plus exactly one accent — a stamp-red reserved for status marks and proof moments (an "Open to Work" stamp, exhibit tags, the primary contact action) — never for ambient branding or category color-coding.

Two typefaces do distinct jobs: Source Serif 4 sets the record's own prose (name, summary, exhibit titles — content that was "typeset"), and Courier Prime sets everything that reads as filled-in or typed data (field labels and values, dates, reference codes, tags, buttons). Mixing the two within one role is a system violation, not a variant.

Capabilities and exhibits cross-reference each other by code (e.g. exhibit "Refs: C1 · C2 · A2" link to capability items "C1", "A2"), a real "see also" mechanic borrowed from card-catalog cross-referencing, not decorative section numbering — which is why capability ref codes stay but generic section numbers (§1/§2/§3) were removed as undifferentiated decoration.

**Key Characteristics:**
- One record-card shell, not a multi-hero portfolio layout; project work is explicitly subordinate, filed as exhibits
- Restrained palette: two neutral inks + one stamp-red accent used only for status/proof, never ambient
- Serif for the record's own prose, monospace exclusively for typed/filled data fields
- Depth from real stacked-paper offset and hairline rules; no glow, no blur-as-decoration, no gradients
- Cross-reference codes (exhibit ↔ capability) are functional, not decorative section numbering

## Colors

Two neutral inks carry the whole page; the one stamp-red accent is spent only on status and proof, never spread across categories.

### Primary
- **Ink** (`#1c2530` light-mode text / `#dfe6ec` dark-mode text): The record's own prose and every field value — the document's base "typed in black ink" voice.

### Secondary
- **Stamp Red** (`#a3242f` light / `#e2555f` dark): The single accent. Used only for status (the "Open to Work" stamp), proof/pending marks (the reserved AI-rollout exhibit's "On File · Pending" stamp), and the one primary contact action. Never used as a decorative brand color, a hover glow, or a category tag color.

### Neutral
- **Paper** (`#e9edf1` light bg / `#14181d` dark bg): The record card's own stock.
- **Paper 2** (`#f4f6f8` light / `#1b2129` dark): Nav bar and exhibit-card surface, one step off the record stock.
- **Paper Deep** (`#d7dee5` light / `#0c0f13` dark): The stacked-sheet layers behind the record, used only for the depth device.
- **Ink Dim** (`#4b5a6b` light / `#97a3af` dark): Secondary reading copy — the summary paragraph, exhibit descriptions.
- **Ink Muted** (`#576573` light / `#8b96a2` dark): Field labels, reference codes, footer — tuned to clear 4.5:1 contrast against both paper tones (do not reuse the pre-redesign muted values; they read under 4:1).
- **Rule** (`rgba(28,37,48,0.20)` light-mode base opacity) / **Rule Strong** (`0.40`): Every hairline border and divider in the system, at two opacities for resting vs. emphasized.

### Named Rules
**The One-Accent Rule.** Stamp-red is spent only on status and proof — never on ambient decoration, never split across categories the way the previous system used cyan/violet/amber. If a second category needs distinguishing, it is distinguished by position, label, or rule-line, never by a second color.

**The No-Glow Rule.** Depth and hierarchy come from stacked-paper offset shadows (real offset + soft blur) and rule-line opacity, never from colored glow, backdrop blur, or gradients. This is the explicit repudiation of the previous system's cyan glow.

## Typography

**Display/Prose Font:** Source Serif 4 (with Georgia fallback)
**Typed/Data Font:** Courier Prime (with Courier New fallback)

**Character:** Source Serif 4 is the record's own printed voice — the name, the summary, exhibit titles. Courier Prime is reserved for anything that reads as filled-in data: field labels and values, dates, reference codes, tags, and buttons. The pairing dramatizes "typeset document" versus "typed-in answer," which is the whole visual joke of a personnel record.

### Hierarchy
- **Name** (700, `clamp(1.7rem, 3.4vw, 2.35rem)`, line-height 1.05): The one outsized element on the page — the NAME field value. Not a hero headline; it is sized this way because it is the biggest field in the grid, nothing more.
- **Section Heading** (700, `0.82rem`, letter-spacing `0.1em`, uppercase, Courier Prime): SUMMARY / CAPABILITIES / ATTACHED EXHIBITS / AUTHORIZED CONTACT. No numbering prefix — removed a §1–§4 decorative sequence during finish review because it carried no cross-referencable information, unlike the capability ref codes, which do.
- **Body** (400, `1.02rem`, line-height 1.85, max 68ch, Source Serif 4): The summary paragraph — the only long-form prose on the page.
- **Field Value** (400, `0.82–0.95rem`, Courier Prime, tabular-nums): Every filled-in data point — ref no., role, location, dates, tags, reference codes.
- **Field Label** (700, `0.63rem`, letter-spacing `0.1em`, uppercase, Courier Prime, ink-muted): The small caption above every field value.

### Named Rules
**The Typed-vs-Set Rule.** Text the document "printed" (name, summary prose, exhibit titles) is Source Serif 4. Text that reads as "filled in" (field values, tags, ref codes, buttons) is Courier Prime. A role that mixes the two is a defect, not a variant.

## Layout

A single centered record (`max-width: 900px`), presented as one bordered card divided into stacked sections by hairline rules, never as separate floating cards or a multi-hero scroll. Order is CV-first: header field grid → summary + service history → capabilities → attached exhibits → authorized contact — deliberately subordinating the project portfolio to the record it sits inside, per explicit direction.

The header is a field grid (ID-photo box + REF/NAME/ROLE/LOCATION + status stamp) rather than a hero. Exhibits present as a two-column card grid on desktop, collapsing to one column under 760px; the service-history table collapses from a real `<table>` to stacked label/value rows on the same breakpoint. Capability groups (`A — Data Modelling`, `B — BI & Reporting`, `C — Engineering`) sit three-across on desktop, one column on mobile.

## Elevation & Depth

Flat by default, with one deliberate depth device: the record card sits atop two faint offset copies of itself (`::before`/`::after`, translated a few pixels and given a soft neutral shadow), reading as a real stack of paper sheets rather than a floating card. No other element in the system uses a shadow; hover states move (`translateY`) rather than lift with new shadow.

### Shadow Vocabulary
- **Stacked-sheet shadow** (`box-shadow: 3px 4px 10px rgba(28,37,48,0.16)` light / `rgba(0,0,0,0.55)` dark): Applied once, to the record's own `::before` pseudo-element, simulating the sheet beneath it. Real offset, real blur, neutral tint — never colored.

### Named Rules
**The Stacked-Paper Rule.** Depth is a physical fact (real paper sheets sitting under the top one), not a floating-card effect. One shadow instance in the whole system; everywhere else, depth is rule-line opacity only.

## Shapes

Zero border radius throughout — every box (record, exhibit, field grid, buttons, stamps, ID-photo) is a hard rectangle, matching a real paper document's corners. The one exception to squareness is the rotated stamp elements (status stamp, pending stamp), which are still rectangular but sit at a slight rotation (`-3deg`/`-4deg`) to read as a physically pressed rubber stamp rather than aligned UI chrome. Borders are always 1px hairlines at `--rule` or `--rule-strong`; no card in the system uses a soft rounded corner.

## Components

Every component reads as a real paper-record artifact rather than a modern UI primitive: field grids, ruled tables, staple marks, and rubber stamps instead of hero sections, icon-badge cards, and pill tags.

### Stamps
- **Shape:** 2px solid border, zero radius, rotated -3° to -4°, Courier Prime uppercase.
- **Status stamp:** Stamp-red border and text on transparent ground; plays a one-time press-in animation on load (scale + rotate settling via `cubic-bezier(0.16, 1, 0.3, 1)`) — the system's one authored motion moment.
- **Pending stamp:** Same shape, used on the reserved "on file" exhibit to mark unfilled content honestly rather than fabricating it.

### Field Grid
- **Style:** Label (Courier Prime, ink-muted, uppercase, 0.63rem) stacked above value (Courier Prime or Source Serif 4 depending on role). No border around individual fields; the grid gap and label/value pairing alone create structure.

### Exhibits (Cards)
- **Shape:** Zero radius, 1px `--rule` border shifting to `--rule-strong` on hover, `translateY(-2px)` lift, no shadow.
- **Marks:** An exhibit-tag label ("Exhibit A") oversetting the top edge like a tab, and a small drawn staple mark in the top corner — literal filing-cabinet detail, not decoration.
- **Reference footer:** A "Refs: A1 · A2 · C2" line linking to the matching capability items — the system's cross-reference mechanic, functional (real anchor links), not decorative.
- **Reserved slot:** One exhibit renders as an explicit diagonal-hatch "pending" card rather than being omitted or faked — the honest placeholder for AI/Copilot rollout work PRODUCT.md flags as not yet evidenced.

### Buttons
- **Primary (Authorized Contact):** Transparent ground, stamp-red border and text; inverts to solid stamp-red on hover. The only place stamp-red appears as a fill.
- **Secondary:** Transparent ground, `--rule-strong` border, ink text; border darkens to full ink on hover.

### Tables (Service History)
- **Style:** Real `<table>`, hairline row dividers, Courier Prime for entry/period columns (tabular-nums), Source Serif 4-weight-700 for the role column.

### Navigation
- **Style:** Sticky, flat (no blur), Courier Prime uppercase-free small links, hairline bottom border. No logo glow, no active-state color beyond stamp-red on hover.

## Do's and Don'ts

### Do:
- **Do** keep Courier Prime exclusively for typed/filled data (fields, tags, ref codes, buttons) and Source Serif 4 exclusively for the record's own prose.
- **Do** spend stamp-red only on status, proof, and the one primary action — never as ambient brand color or a second/third category color.
- **Do** build depth from real stacked-paper offset and rule-line opacity; never reach for glow, backdrop blur, or a gradient.
- **Do** mark unfilled/future content honestly (a labeled "pending" exhibit) rather than fabricating placeholder case studies.
- **Do** keep cross-reference codes (exhibit ↔ capability) functional, real anchor links — not decorative section numbering.

### Don't:
- **Don't** reintroduce the previous dark/neon-cyan/terminal-console identity, gradients, glow, or particle-canvas motion — this system exists specifically to replace it.
- **Don't** add rounded corners; every shape in this system is a hard rectangle except the deliberately rotated stamps.
- **Don't** color-code categories with multiple accent hues; one stamp-red accent, spent only on status/proof, is the whole system.
- **Don't** use a Unicode glyph or emoji as an icon (a drawn checkmark, not `✓`, and inline SVG for arrows/marks).
- **Don't** add a decorative section-number sequence (§1/§2/§3, 01/02/03) that carries no cross-referencable information — the ref-code cross-reference stays because it is functional, generic sequence numbering does not.

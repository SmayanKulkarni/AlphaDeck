---
name: Banking Dark UI
description: A focused dark-mode Power BI system for trustworthy portfolio risk review.
colors:
  canvas: "#0C111B"
  rail: "#101827"
  panel: "#151F2E"
  raised: "#1C2A3D"
  line: "#2C3D52"
  text: "#F1F5FA"
  muted: "#AABAD0"
  teal: "#61D4B3"
  blue: "#76B7FA"
  amber: "#F2C46D"
  violet: "#BCACF3"
  red: "#F19199"
typography:
  display:
    fontFamily: "Segoe UI, sans-serif"
    fontSize: "24pt"
    fontWeight: 700
    lineHeight: 1.2
  body:
    fontFamily: "Segoe UI, sans-serif"
    fontSize: "11pt"
    fontWeight: 400
    lineHeight: 1.4
  label:
    fontFamily: "Segoe UI, sans-serif"
    fontSize: "10pt"
    fontWeight: 600
rounded:
  compact: "4px"
  panel: "8px"
spacing:
  compact: "12px"
  standard: "16px"
  section: "24px"
components:
  metric-card:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.text}"
    rounded: "{rounded.panel}"
    padding: "16px"
  active-navigation:
    backgroundColor: "{colors.raised}"
    textColor: "{colors.text}"
    rounded: "{rounded.compact}"
    padding: "12px"
  filter-field:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.text}"
    rounded: "{rounded.compact}"
    padding: "12px"
---

# Design System: Banking Dark UI

## Overview

**Creative North Star: "The Night Shift Control Room"**

This system treats banking analytics as an operational surface: calm, dark, highly legible, and deliberately free of decorative noise. It is built to make portfolio health and risk exceptions easy to scan during a fast review.

**Key Characteristics:**

- Tonal navy layering rather than bright card shadows.
- One purposeful accent per chart, with red reserved for risk and exception signals.
- Compact, native Power BI controls with generous alignment and whitespace.

## Colors

The palette is a deep neutral field that lets portfolio metrics and analytical signals carry the visual hierarchy.

### Primary

- Teal is the affirmative portfolio accent for healthy value measures, selected states, and the overview identity.

### Secondary

- Blue supports lending and geographic comparison without competing with the primary accent.

### Tertiary

- Amber signals deposits, funding, and attention-worthy composition; violet distinguishes supporting segments; red is reserved for risk.

### Neutral

- Canvas, rail, panel, raised surface, line, text, and muted text form the structural hierarchy.

**The Signal-Only Accent Rule.** Accent color communicates data meaning, not decoration; no single chart should become a rainbow.

## Typography

Segoe UI gives the native report a clear, familiar analytical voice.

### Hierarchy

- **Display:** used for report and section titles.
- **Body:** used for chart context and supporting explanation.
- **Label:** used for slicers, card labels, and navigation.

**The Scan-First Rule.** Labels clarify a decision or metric; they never compete with the number or chart they support.

## Layout

A fixed left rail establishes location and page navigation. The main canvas uses a simple review sequence: title and filters, KPI row, then a balanced two-column analytical grid. Spacing follows a 12/16/24 rhythm. The former duplicated landing and summary view is consolidated into Portfolio overview; the original summary page identifier remains hidden for compatibility.

## Elevation & Depth

Depth comes from tonal layering, not drop shadows: canvas is the deepest plane, rail and panels are the working plane, and selected navigation uses the raised tone. Borders are subtle separators only.

**The Flat-By-Default Rule.** Do not add ornamental shadows, gradients, or glass effects to native report surfaces.

## Shapes

The visual language is quietly structured: small 4px corners for controls and restrained 8px corners for panels and cards. Boundaries are drawn with the line color only where they improve grouping.

## Components

### Cards / Containers

- **Style:** dark panel surface, restrained rounded corners, clear metric-first hierarchy.
- **Internal Padding:** 16px.

### Inputs / Fields

- **Style:** compact native slicers on the panel surface, with white text and muted supporting labels.

### Navigation

- **Style:** left-rail labels use muted text at rest and a raised background with bright text for the active page. Use Power BI's page tabs for navigation.

## Do's and Don'ts

### Do:

- **Do** use teal, blue, amber, violet, and red consistently by analytical meaning.
- **Do** keep the KPI row to the metrics needed for the current page decision.
- **Do** retain native filters and cross-filter behavior when simplifying a chart.

### Don't:

- **Don't** reintroduce redundant donut or funnel visuals where ranked bars are clearer.
- **Don't** use red for non-risk data.
- **Don't** display cohort-derived current-balance changes as time-series growth.

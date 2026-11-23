---
name: Adaptive Fit AI — v2 Minimalist Training & AI Coach
description: Mobile-first and desktop-adaptive Apple Minimalist workout, nutrition, and full-screen AI coach web app.
colors:
  apple-blue: "#0066CC"
  apple-cyan: "#0077B6"
  apple-green: "#187932"
  apple-orange: "#B25000"
  apple-red: "#C92A2A"
  system-ground: "#F7F7F8"
  dark-ground: "#000000"
  card-white: "#FFFFFF"
  dark-card: "#111114"
  subtle-fill: "#F2F2F5"
  segment-fill: "#E8E8ED"
  space-black: "#121316"
  ink-primary: "#111114"
  ink-secondary: "#5C5C66"
  ink-muted: "#86868F"
  border-hairline: "rgba(0, 0, 0, 0.065)"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, SF Pro Display, SF Pro Text, IBM Plex Sans Thai, sans-serif"
    fontSize: "2.15rem"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.03em"
    fontFeature: "tabular-nums"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, SF Pro Display, SF Pro Text, IBM Plex Sans Thai, sans-serif"
    fontSize: "1.75rem"
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: "-0.03em"
    fontFeature: "tabular-nums"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, SF Pro Display, SF Pro Text, IBM Plex Sans Thai, sans-serif"
    fontSize: "1.05rem"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-0.02em"
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, SF Pro Display, SF Pro Text, IBM Plex Sans Thai, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 500
    lineHeight: 1.5
  caption:
    fontFamily: "-apple-system, BlinkMacSystemFont, SF Pro Display, SF Pro Text, IBM Plex Sans Thai, sans-serif"
    fontSize: "0.8125rem"
    fontWeight: 500
    lineHeight: 1.4
  label:
    fontFamily: "JetBrains Mono, ui-monospace, SFMono-Regular, monospace"
    fontSize: "0.75rem"
    fontWeight: 600
    lineHeight: 1.2
    fontFeature: "tabular-nums"
rounded:
  sm: "8px"
  md: "10px"
  lg: "12px"
  xl: "18px"
  pill: "999px"
spacing:
  xs: "6px"
  sm: "10px"
  md: "14px"
  lg: "16px"
components:
  button-primary:
    backgroundColor: "{colors.apple-blue}"
    textColor: "{colors.card-white}"
    rounded: "{rounded.pill}"
    padding: "8px 14px"
    height: "38px"
  button-water:
    backgroundColor: "{colors.apple-cyan}"
    textColor: "{colors.card-white}"
    rounded: "{rounded.pill}"
    padding: "5px 12px"
    height: "32px"
  bento-card:
    backgroundColor: "{colors.card-white}"
    textColor: "{colors.ink-primary}"
    rounded: "{rounded.xl}"
    padding: "16px"
  bento-hero-dark:
    backgroundColor: "{colors.space-black}"
    textColor: "{colors.system-ground}"
    rounded: "{rounded.xl}"
    padding: "16px"
---

# Design System: Dumbbell 8W — Apple Minimalist Training & Energy Bento

## Overview

**Creative North Star: "Apple Health & Fitness Minimalist Bento"**

This system organizes daily workout logging, hydration tracking, BMI/TDEE calculation, and Gemini AI calorie scanning into a clean, light-filled 2-column Bento Grid inspired by Apple Health and iOS 18. Crisp white squircle cards (`#FFFFFF`) rest on a soft cool system gray ground (`#F5F5F7`), anchored by a single Space Black (`#1D1D1F`) Hero Energy Bento card and a floating Dynamic Island rest timer capsule.

Every screen honors a strict Zero Emoji Policy, replacing decorative pictographs with SF Symbols-inspired monoline vector icons inside tinted rounded squares. All numbers use `tabular-nums` so set weights, countdown clocks, and API quota counters remain perfectly aligned.

**Key Characteristics:**
- Clean adaptive palette (`#F7F7F8` light ground / `#000000` dark ground, `#FFFFFF` / `#111114` Bento cards, `#121316` Hero Energy Bento and Dynamic Island timer).
- Minimalist Shell: 54px single-row mobile topbar + floating 5-tab dock (`วันนี้`, `ซ้อม`, `อาหาร`, `แชท AI`, `ฉัน`) on `< 960px`; 244px left sidebar on desktop (`>= 960px`) + 292px live context rail (`>= 1280px`) on the dedicated AI Chat tab.
- Progressive disclosure via native `<dialog class="app-sheet">` bottom sheets (`sheetFoodLog`, `sheetWorkoutTools`, `sheetReadiness`, `sheetExerciseDetail`, `sheetAiTools`, `sheetSystemStatus`, `pwaInstallDialog`) so primary feeds stay calm and clutter-free.
- Zero Emoji Policy across all interfaces and AI outputs.

## Colors

The color system pairs Apple's neutral iOS system surfaces with five high-contrast semantic accents for training, hydration, completion, caution, and quota limits.

### Primary
- **Apple Action Blue** (`#0066CC`): Primary CTA buttons, active dock tab, and primary focus rings.

### Secondary
- **Apple Hydration Cyan-Blue** (`#0062B8` / `#007AFF`): Water intake readouts, capsule meters, and quick-add hydration buttons.

### Tertiary
- **Apple Fitness Green** (`#1D7D36` / `#34C759`): Completed workout sets, protein goal progress, and nominal Gemini API quota status.
- **Apple Caution Orange** (`#B25000` / `#FF9500`): Knee and lower-back safety callouts, skipped exercise state, and 70%+ API quota warnings.
- **Apple Critical Red** (`#C92A2A` / `#FF3B30`): Cardio activity badge, over-target calorie bar, 19 kg dumbbell load alerts, and exhausted API quota banners.

### Neutral
- **Apple System Gray 6** (`#F7F7F8` light / `#000000` dark): Main viewport background.
- **Pure Bento White** (`#FFFFFF` light / `#111114` dark): Card surface and active segmented button fill.
- **Grouped Inner Fill** (`#F2F2F5`) and **Segmented Track** (`#E8E8ED`): Set rows, inline guide sheets, and segmented day picker track.
- **Apple Space Black** (`#121316`) and **Dark Subtle** (`rgba(255,255,255,0.08)`): Hero Energy Bento card and Dynamic Island rest timer.
- **Primary Ink** (`#111114` light / `#F5F5F7` dark), **Secondary Ink** (`#5C5C66`), and **Muted Ink** (`#86868F`): High-contrast text hierarchy passing WCAG AA across all surfaces.

### Named Rules
**The One Dark Anchor Rule.** Only the Hero Energy Bento card and the floating Dynamic Island timer pill use Space Black (`#1D1D1F`); all other cards stay crisp white (`#FFFFFF`) so the page remains airy and calm.

## Typography

**Display & Body Font:** `-apple-system, BlinkMacSystemFont, 'SF Pro Display', 'SF Pro Text', 'IBM Plex Sans Thai', sans-serif`
**Label / Telemetry Font:** `'JetBrains Mono', ui-monospace, SFMono-Regular, monospace`

**Character:** Apple system sans-serif paired with `IBM Plex Sans Thai` for effortless Thai legibility, reinforced by tabular numerals on every metric.

### Hierarchy
- **Display** (`700`, `2.15rem`, `1.1`, `-0.03em`): Hero Energy remaining calorie readout.
- **Headline** (`700`, `1.75rem`, `1.15`, `-0.03em`): Primary metric inside 1-column Bento cards (water ml, workout progress, weight kg, BMI).
- **Title** (`700`, `1.05rem`, `1.2`, `-0.02em`): App title, exercise card titles, and mini-tile values.
- **Body** (`500`, `0.9375rem`, `1.5`): Bento card headings, form inputs, and primary row content.
- **Caption** (`500`–`600`, `0.8125rem`, `1.4`): Secondary descriptions, execution steps, and pill buttons.
- **Label** (`600`–`700`, `0.75rem`, `1.2`, `tabular-nums`): Status pills, dock tab labels, and timer chips.

### Named Rules
**The Tabular Metric Rule.** Every numeric readout, timer, weight input, and quota counter enforces `font-variant-numeric: tabular-nums`.

## Layout

Responsive minimalist workspace: on mobile (`< 960px`), a 54px single-row frosted topbar and floating 5-tab capsule dock wrap a centered container (`680px` max-width on standard tabs); on desktop (`>= 960px`), a 244px left navigation rail pairs with a generous main canvas (and on `>= 1280px` during the dedicated `แชท AI` view, a 292px live telemetry context rail sits alongside the full-height chat stream with date controls hidden). Secondary forms and tools open inside `<dialog class="app-sheet">` bottom sheets/modals rather than cluttering the main feed.

## Elevation & Depth

Cards use a subtle `1px solid var(--border-hairline)` border paired with whisper-light shadow (`0 1px 2px rgba(0,0,0,0.03), 0 6px 20px rgba(0,0,0,0.025)`) against `#F7F7F8` (or crisp border-only contrast in `#000000` dark mode). Navigation bars use frosted glass (`backdrop-filter: saturate(180%) blur(20px)`).

## Shapes

- **Bento Cards:** `18px` rounded corners (`--radius-card`).
- **Inner Tiles & Inset Lists:** `12px` rounded corners (`--radius-inner`).
- **Inputs & Controls:** `10px` rounded corners (`--radius-control`).
- **Icon Badges & Segmented Buttons:** `8px` rounded corners (`--radius-sm`).
- **Buttons, Status Badges & Progress Bars:** `999px` full capsule geometry (`--radius-pill`).

## Components

### Buttons
- **Shape:** Full capsule (`999px` radius), `38px` standard height (`32px` compact).
- **Variants:** Primary Apple Blue (`#0066CC`), Water Cyan (`#0062B8`), Completed Green (`#1D7D36`), Space Black (`#1D1D1F`), and Subtle Gray (`#F2F2F7`).

### Bento Cards
- **Corner Style:** `18px` radius, `16px` internal padding, `12px` vertical stack gap.
- **Header Pattern:** `30x30px` tinted icon badge (`8px` radius) paired inline with a bold `0.9375rem` title and an optional right-aligned status pill.

### Segmented Day Picker
- 7-column iOS segmented control (`#E8E8ED` background, `4px` padding, `12px` radius) where the selected day lifts onto a `#FFFFFF` pill (`8px` radius).

### Dynamic Island Rest Timer
- Floating Space Black (`#121316`) capsule positioned above the floating 5-tab bottom dock, housing a tabular countdown clock (`#FF9F0A` while running, `#30D158` when finished) and quick preset chips (`60s`, `90s`, `120s`).

## Do's and Don'ts

### Do:
- **Do** organize summary metrics into 1-column and 2-column Bento cards on `#F5F5F7`.
- **Do** use monoline SVG icons inside `30x30px` tinted containers.
- **Do** keep all text sizes on the 6-step scale (`0.75rem`, `0.8125rem`, `0.9375rem`, `1.05rem`, `1.75rem`, `2.15rem`).

### Don't:
- **Don't** use emojis or Unicode symbols anywhere in the interface.
- **Don't** combine borders with drop shadows on Bento cards.
- **Don't** place kicker/eyebrow labels above card headings.

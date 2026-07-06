---
name: Luminous Utility
colors:
  surface: '#f8f9ff'
  surface-dim: '#d4dae7'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eef4ff'
  surface-container: '#e7eefb'
  surface-container-high: '#e2e8f5'
  surface-container-highest: '#dce3f0'
  on-surface: '#151c25'
  on-surface-variant: '#464555'
  inverse-surface: '#2a313b'
  inverse-on-surface: '#eaf1fe'
  outline: '#777587'
  outline-variant: '#c7c4d8'
  surface-tint: '#4d44e3'
  primary: '#3525cd'
  on-primary: '#ffffff'
  primary-container: '#4f46e5'
  on-primary-container: '#dad7ff'
  inverse-primary: '#c3c0ff'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#684000'
  on-tertiary: '#ffffff'
  tertiary-container: '#885500'
  on-tertiary-container: '#ffd4a4'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#0f0069'
  on-primary-fixed-variant: '#3323cc'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb95f'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#f8f9ff'
  on-background: '#151c25'
  surface-variant: '#dce3f0'
typography:
  display:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  mono:
    fontFamily: Geist
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-max: 1200px
  edge-margin-mobile: 16px
  edge-margin-desktop: 40px
  gutter: 24px
  stack-gap: 12px
  section-gap: 48px
---

## Brand & Style

The design system is centered on high-performance habit tracking, blending the structural clarity of Linear with the approachable minimalism of Apple. It targets users who value focus and organizational velocity. 

The aesthetic is **Modern Minimalist with Glassmorphic accents**. It prioritizes extreme legibility and "breathable" interfaces through generous whitespace and a restricted color palette. Interactions should feel instantaneous and fluid, utilizing soft transitions to provide a sense of calm productivity. The mood is disciplined yet encouraging, reducing cognitive load to help users focus entirely on their daily routines.

## Colors

The palette is anchored by a deep Indigo primary, used for focused actions and brand presence. The system relies heavily on a "layered white" approach in light mode, using `#F9FAFB` for the base and pure white for elevated cards. 

In dark mode, the system shifts to a deep charcoal gray (rather than true black) to maintain the soft border aesthetic. 
- **Success/Warning/Danger**: Used sparingly for status indicators and completion streaks.
- **Neutrals**: Used for structural borders (`#F3F4F6` in light mode) and secondary text metadata.
- **Glassmorphism**: Overlays and navigation bars use a background blur (20px) with a 70% opacity white/dark-gray tint and a 1px white/transparent border.

## Typography

This design system utilizes **Inter** for all primary communication to ensure maximum legibility across different pixel densities. **Geist** is introduced for labels and technical data (like habit counts or streaks) to provide a modern, "developer-tool" precision inspired by Linear.

Hierarchy is established through weight and letter spacing rather than excessive size changes. Large displays and headlines use tighter letter spacing to appear more cohesive, while small labels use increased tracking for clarity.

## Layout & Spacing

The layout philosophy follows a **Fluid-Fixed Hybrid**. Main content resides within a centered 1200px container on desktop, while sidebars and navigation utilize fluid percentage widths with hard minimums.

- **Grid**: A 12-column grid is used for dashboard views.
- **Rhythm**: Spacing is based on a 4px baseline, with 12px and 24px being the most frequent increments for internal card padding and element spacing respectively.
- **Mobile**: Margins shrink to 16px. Complex horizontal data (like weekly heatmaps) should switch to a horizontal scroll or condensed "dot" view.

## Elevation & Depth

Hierarchy is defined through **Tonal Layering and Low-Contrast Outlines** rather than heavy shadows.

- **Level 0 (Base)**: `#F9FAFB` background.
- **Level 1 (Cards)**: White background with a 1px solid border (`#F3F4F6`). No shadow, or a very faint 2px ambient blur.
- **Level 2 (Active/Hover)**: A soft, diffused shadow (0px 4px 12px rgba(0,0,0,0.03)) to indicate interactivity.
- **Overlays/Modals**: Glassmorphism effect with a `backdrop-filter: blur(20px)` and a slightly thicker 1.5px border to separate from the background.

## Shapes

The shape language is consistently rounded to evoke a friendly, modern feel. 
- **Small elements** (Checkboxes, Tags): 6px radius.
- **Standard elements** (Buttons, Inputs): 8px radius.
- **Large containers** (Cards, Modals): 16px radius.
- **Interactive States**: When an item is clicked or active, the shape remains consistent, but the border-weight or color shifts to the primary indigo.

## Components

- **Buttons**: Primary buttons are solid Indigo with white text. Secondary buttons use a white background with a subtle gray border. Transitions for hover should be 150ms ease-in-out, shifting background-color slightly darker.
- **Habit Chips**: Small, pill-shaped indicators for categories (e.g., "Health", "Work"). Use a 10% opacity version of the category color for the background with high-contrast text.
- **Checkboxes**: Custom-designed 20px squares with a 6px radius. When checked, they fill with the Primary or Success color and display a thin Lucide-style checkmark.
- **Cards**: The fundamental building block. 16px internal padding, 1px border. Habit cards feature a "Mini-Trend" Sparkline in the corner.
- **Inputs**: Clean, border-bottom only or subtle 1px gray border. Focus state uses a 2px Indigo ring with an offset.
- **Progress Rings**: Circular progress indicators used for daily goals, featuring a 4px stroke width and a light gray track.
- **Icons**: 20px Lucide icons with a 1.5px stroke weight, consistently aligned with text baselines.
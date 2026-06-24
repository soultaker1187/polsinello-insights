---
name: Institutional Pro
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#424751'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#737783'
  outline-variant: '#c2c6d3'
  surface-tint: '#255dad'
  primary: '#00346f'
  on-primary: '#ffffff'
  primary-container: '#004a99'
  on-primary-container: '#9bbdff'
  inverse-primary: '#abc7ff'
  secondary: '#515f74'
  on-secondary: '#ffffff'
  secondary-container: '#d5e3fc'
  on-secondary-container: '#57657a'
  tertiary: '#2e354a'
  on-tertiary: '#ffffff'
  tertiary-container: '#444c61'
  on-tertiary-container: '#b5bcd6'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d7e2ff'
  primary-fixed-dim: '#abc7ff'
  on-primary-fixed: '#001b3f'
  on-primary-fixed-variant: '#00458f'
  secondary-fixed: '#d5e3fc'
  secondary-fixed-dim: '#b9c7df'
  on-secondary-fixed: '#0d1c2e'
  on-secondary-fixed-variant: '#3a485b'
  tertiary-fixed: '#dae2fd'
  tertiary-fixed-dim: '#bec6e0'
  on-tertiary-fixed: '#131b2e'
  on-tertiary-fixed-variant: '#3f465c'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-sm:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 18px
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
  table-header:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  container-padding: 24px
  gutter: 16px
  table-cell-padding: 8px 12px
  stack-compact: 8px
  stack-default: 16px
---

## Brand & Style

This design system is engineered for high-stakes environments where data density and precision are paramount. The brand personality is **authoritative, analytical, and systematic**, targeting technical architects and data stewards who require a tool that feels like a professional instrument rather than a consumer application.

The design style is **Corporate / Modern** with a lean toward **Functional Minimalism**. It prioritizes information hierarchy over decorative elements, utilizing a structured grid and a restrained palette to reduce cognitive load during complex configuration tasks. The emotional response should be one of absolute reliability and clarity—eliminating ambiguity in schema mapping and large-scale data operations.

## Colors

The palette is anchored by **Civic Blue** (#004A99), a deep, high-contrast primary used for core actions and active states, signifying stability and trust. **Institutional Slate** (#475569) serves as the secondary color, providing a professional tone for iconography and secondary UI elements.

- **Primary (Civic Blue):** Core interactive elements, progress bars, and primary buttons.
- **Secondary (Institutional Slate):** Sub-navigation, secondary buttons, and descriptive icons.
- **Tertiary (Deep Slate):** High-density text and headers to ensure maximum legibility.
- **Surface/Neutral:** A range of cool grays (Slate 50 to 200) defines the workspace containers, ensuring a clean backdrop for complex data tables.
- **Semantic Colors:** Success (Emerald), Warning (Amber), and Error (Rose) are used sparingly and at high saturation to ensure alerts are unmistakable.

## Typography

The typography system is designed for legibility in dense interfaces. **Hanken Grotesk** provides a sharp, contemporary edge for headlines, while **Inter** ensures that body text and data values remain highly readable at smaller scales.

**JetBrains Mono** is utilized for technical labels, schema keys, and data types to distinguish "system" values from "user" content. For data-heavy tables, the `table-header` style uses increased letter spacing and uppercase styling to provide clear structural anchoring without requiring heavy borders.

## Layout & Spacing

The layout follows a **Fluid Grid** model optimized for wide-screen data management. A 12-column system is used for dashboard layouts, while configuration views (like schema mapping) utilize a split-pane approach with a fixed 320px sidebar and a flexible content area.

- **Data Density:** A strict 4px baseline grid is used. For tables and lists, we employ "Compact" spacing by default, allowing for maximum vertical information density.
- **Breakpoints:** 
  - **Desktop (1440px+):** 24px margins, 16px gutters.
  - **Tablet (768px - 1439px):** 16px margins, 12px gutters; sidebars collapse into icons.
  - **Mobile:** Not recommended for configuration; read-only summary views only.

## Elevation & Depth

To maintain a "Pro" feel, the system uses **Tonal Layers** and **Low-contrast Outlines** rather than heavy shadows. This creates a flat, organized workspace that feels like a single cohesive sheet of glass or paper.

- **Base Layer:** The application background is Slate 50.
- **Surface Layer:** Primary content containers use a white fill with a 1px border in Slate 200.
- **Active Layer:** Elements currently being edited or mapped receive a subtle primary-tinted glow (2px blur, 10% opacity Civic Blue) to guide focus.
- **Modals/Overlays:** Use a slightly more pronounced shadow (0 4px 12px rgba(15, 23, 42, 0.08)) to indicate temporary context switching.

## Shapes

The design system uses a **Soft (0.25rem)** roundedness level to maintain a professional, architectural feel. 

- **Small Components:** Checkboxes, inputs, and buttons use a 4px radius.
- **Cards & Tables:** Use an 8px radius (`rounded-lg`) for outer containers.
- **Chips:** Specifically for advanced filtering, chips use a slightly higher 12px radius to distinguish them from actionable buttons.

## Components

### Data Tables & Multi-select
Tables are the core of this system. They feature sticky headers, checkbox columns for bulk actions, and row-hover states in a very light blue tint. Selected rows use a distinct Slate 100 background with a 2px Civic Blue left-edge highlight.

### Advanced Filtering Chips
Filters are displayed as a horizontal row above data tables. They consist of a label and a value (e.g., `Status: Active`). Clicking a chip opens a popover for refined selection. Active chips are filled with a light Civic Blue tint; inactive chips have a Slate 200 outline.

### Schema Mapping Interface
For connecting source fields to destinations, use a "Link and Node" visual. Source fields are on the left, destinations on the right. Mapping lines are drawn with a 1.5px stroke in Institutional Slate, turning Civic Blue when a specific field is hovered or selected.

### Progress Indicators (Large Exports)
Exports use a dedicated status bar at the bottom of the viewport or a prominent card in a "Downloads" tray. The indicator includes:
1. **Linear Progress Bar:** 4px height, Civic Blue fill.
2. **Status Label:** (e.g., "Exporting 1.2M rows...")
3. **Percentage & Time Remaining:** Monospaced (JetBrains Mono) for stable width during updates.

### Input Fields
Standardized with a 1px Slate 300 border that thickens to 2px Civic Blue on focus. Labels are positioned above the field in `body-sm` bold.
---
name: Heritage Terminal
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
  secondary: '#565e74'
  on-secondary: '#ffffff'
  secondary-container: '#dae2fd'
  on-secondary-container: '#5c647a'
  tertiary: '#483201'
  on-tertiary: '#ffffff'
  tertiary-container: '#614815'
  on-tertiary-container: '#dbb87a'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d7e2ff'
  primary-fixed-dim: '#abc7ff'
  on-primary-fixed: '#001b3f'
  on-primary-fixed-variant: '#00458f'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#ffdea7'
  tertiary-fixed-dim: '#e5c283'
  on-tertiary-fixed: '#271900'
  on-tertiary-fixed-variant: '#5b4310'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
  heritage-gold: '#b39359'
  terminal-navy: '#0f172a'
  institutional-blue: '#004a99'
  slate-border: '#e2e8f0'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-sm:
    fontFamily: Hanken Grotesk
    fontSize: 20px
    fontWeight: '500'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  data-mono:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.02em
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  heritage-tag:
    fontFamily: Hanken Grotesk
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 12px
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  container-max: 1440px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 40px
  terminal-gap: 1px
---

## Brand & Style

This design system embodies the concept of "Institutional Heritage." It merges the high-density, data-driven efficiency of a **Financial Terminal** with the prestigious, stable aura of a multi-decade real estate advisory. The aesthetic is precise, authoritative, and unapologetically professional.

The design style is a sophisticated **Corporate Modern** with a focus on high-information density. It utilizes structured grids and tonal layering to organize complex data sets while maintaining a premium feel through generous margins around key identity elements. A "since 1989" marker is used as a functional stamp of authority, appearing as a subtle architectural detail in headers and footers to ground the modern interface in established history.

Visuals should feel calibrated and intentional. Avoid decorative flourishes; every line, border, and shade must serve the purpose of clarity and trust.

## Colors

The palette is anchored by **Institutional Blue** and **Terminal Navy**, providing the weight and seriousness of a global financial entity. The primary blue is used for key actions and focus states, while navy serves as the foundation for typography and high-level structural components.

To emphasize the "Since 1989" legacy, we introduce **Heritage Gold** (#b39359). This is a sophisticated, muted secondary accent used sparingly to denote premium status, verification markers, and heritage-related highlights. It should never be used for primary actions, but rather as a "seal of quality."

The background utilizes a very clean, neutral slate-white to reduce eye strain in data-heavy views, maintaining the terminal's utility without the harshness of pure white.

## Typography

Typography is the primary tool for creating the "Financial Terminal" look. **Hanken Grotesk** provides a sharp, modern geometric feel for headlines, ensuring the brand looks forward. **Inter** is utilized for all body copy and data points, chosen for its exceptional legibility at small sizes and high-density environments.

Numerical data should use the `data-mono` style to ensure alignment in tabular views, mimicking a Bloomberg or Reuters terminal. The `heritage-tag` is reserved specifically for "EST. 1989" markers and legacy badges, often paired with a subtle horizontal rule or border to frame the text.

## Layout & Spacing

The layout utilizes a **Fixed Grid** system on desktop (12 columns, 1440px max width) to maintain a controlled, institutional appearance. On data-heavy "Terminal" pages, the system shifts to a high-density logic where elements are separated by `terminal-gap` (1px borders) rather than large white-space gutters.

Spacing follows a strict 4px base unit. Internal component padding should be tight (8px-12px) to maximize information density, while the macro-layout uses larger margins (40px+) to frame the "Polsinello Insights" content as high-value. Breakpoints occur at 768px (Tablet) and 1024px (Desktop).

## Elevation & Depth

To maintain the professional "Financial Terminal" aesthetic, the design system avoids heavy, organic shadows. Instead, it uses **Tonal Layers** and **Low-Contrast Outlines**.

Hierarchy is created by stacking surfaces:
- **Level 0 (Base):** Slate-white background.
- **Level 1 (Cards/Panels):** Pure white surfaces with a 1px `slate-border`.
- **Level 2 (Dropdowns/Modals):** Pure white with a very subtle, tight 4px blur shadow (Color: Terminal Navy @ 5% opacity) to provide just enough separation from the base.

Interactive elements use "Inner Tonal Depth"—a slightly darker background on hover—rather than an elevation increase.

## Shapes

The shape language is "Soft" yet disciplined. A universal 4px (`0.25rem`) corner radius is applied to buttons, input fields, and panels. This subtle rounding softens the industrial feel of the terminal grid without making it appear "consumer-grade" or overly casual.

Large container sections may use the 8px (`rounded-lg`) radius, but the majority of functional UI elements must remain at the base level to maintain a precision-engineered look.

## Components

### Buttons
Primary buttons use **Institutional Blue** with white text. Secondary buttons use a `slate-border` and **Terminal Navy** text. The "Heritage Button" used for exclusive advisory CTAs may use a **Heritage Gold** border with navy text. All buttons have a 4px radius and bold Inter labels.

### Heritage Markers
A core component of this system is the **Legacy Stamp**. This is a small, encapsulated label containing "EST. 1989". It should be placed at the top-right of major cards or nested within the navigation bar to subtly reinforce the team's longevity.

### Data Cards
Cards are flat with 1px borders. Header sections of cards should have a subtle grey background (`#f1f5f9`) to separate the title from the content. Use high-contrast navy for values and slate-grey for labels.

### Inputs & Tables
Input fields use a 1px `slate-border` and turn **Institutional Blue** on focus. Tables are the heart of the terminal aesthetic: use thin horizontal dividers, no vertical borders, and `data-mono` typography for all numerical figures. Row zebra-striping is encouraged for readability in large data sets.

### Chips/Badges
Chips are used for market status (e.g., "Active", "Sold"). They use low-saturation background tints of the status color with high-saturation text to remain professional and readable.
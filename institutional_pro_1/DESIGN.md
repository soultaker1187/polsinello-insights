---
name: Institutional Pro
colors:
  surface: '#f9f9ff'
  surface-dim: '#d9d9e1'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3fa'
  surface-container: '#ededf5'
  surface-container-high: '#e7e8ef'
  surface-container-highest: '#e2e2e9'
  on-surface: '#191c21'
  on-surface-variant: '#424751'
  inverse-surface: '#2e3036'
  inverse-on-surface: '#f0f0f8'
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
  tertiary: '#003273'
  on-tertiary: '#ffffff'
  tertiary-container: '#00489e'
  on-tertiary-container: '#9dbcff'
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
  tertiary-fixed: '#d8e2ff'
  tertiary-fixed-dim: '#adc6ff'
  on-tertiary-fixed: '#001a42'
  on-tertiary-fixed-variant: '#004395'
  background: '#f9f9ff'
  on-background: '#191c21'
  surface-variant: '#e2e2e9'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Hanken Grotesk
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
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
    lineHeight: 16px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  container-max: 1440px
  gutter: 20px
---

## Brand & Style
The design system is engineered for **Institutional Pro**, a platform built for real estate intelligence where precision is the primary currency. The brand personality is authoritative, established, and uncompromisingly professional. It draws inspiration from financial terminals and architectural blueprints to create a "technical-industrial" aesthetic.

The design style utilizes **Modern Corporate** principles with a leaning toward **High-Contrast Utilitarianism**. It rejects soft, consumer-grade "friendliness" in favor of structured information density and rigorous alignment. The emotional response should be one of absolute trust, signaling that the data presented is verified, institutional-grade, and ready for high-stakes decision-making. 

Visual signals like subtle grid lines and monospaced numerical data reinforce the heritage of professional excellence "Since 1989," blending legacy authority with modern technical capabilities.

## Colors
The palette is rooted in "Institutional Blue," a deep, stable hue that anchors the interface. "Slate Navy" is reserved for high-level navigation and structural framing, providing a sense of permanence and depth.

"Data Blue" serves as the primary action and interactive accent, ensuring that path-to-task elements are distinct from the brand's primary anchoring colors. "Success Green" is used strictly for positive financial trends and "complete" statuses, maintaining a professional distance from typical consumer "vibrancy." Surfaces utilize cool grays and off-whites to minimize eye strain during long analytical sessions while maintaining a crisp, architectural clarity.

## Typography
Typography in the design system is a hierarchy of function. **Hanken Grotesk** provides a sharp, modernist headline structure that feels established and bold. **Inter** is the workhorse for all body and tabular data, chosen for its exceptional legibility at small sizes and high information density.

For financial metrics and property coordinates, use a monospaced font (JetBrains Mono) to ensure tabular alignment and numerical clarity. Labels should frequently use the `label-caps` style to differentiate metadata from primary content, reinforcing the "technical suite" feel.

## Layout & Spacing
The system uses a **Fixed Grid** philosophy for dashboard views and a **Fluid 12-Column Grid** for content-heavy pages. The spacing rhythm is based on a 4px baseline, but defaults to 16px (md) for standard component gaps to maintain an airy, professional breathing room despite high data density.

- **Desktop (1280px+):** 12 columns, 24px margins, 20px gutters.
- **Tablet (768px - 1279px):** 8 columns, 20px margins, 16px gutters.
- **Mobile (Up to 767px):** 4 columns, 16px margins, 12px gutters.

In data-heavy tables, vertical spacing should be "compact" (8px cell padding) to maximize the visible information per screen, mimicking a financial terminal.

## Elevation & Depth
This design system avoids heavy shadows and deep blurs. Depth is primarily communicated through **Tonal Layers** and **Low-Contrast Outlines**.

- **Level 0 (Background):** #f8fafc (Cool Gray 50).
- **Level 1 (Cards/Surface):** #ffffff with a 1px border (#e2e8f0).
- **Level 2 (Hover/Active):** A subtle, ultra-diffused shadow (0px 4px 12px rgba(15, 23, 42, 0.05)) to indicate interactivity without breaking the flat, architectural aesthetic.
- **Modals:** High-contrast 1px border in #0f172a (Slate Navy) to clearly define the focus area against the background.

## Shapes
The shape language is "Soft" but disciplined. A 4px (0.25rem) radius is the standard for buttons, input fields, and small cards. This slight rounding prevents the UI from feeling aggressive while maintaining the precision of a professional tool. 

Larger containers like primary dashboard panels may use up to 8px (0.5rem), but pill-shapes and high-radius curves are strictly prohibited to avoid a "consumer-tech" or "social media" appearance.

## Components
- **Buttons:** Primary buttons use Institutional Blue (#004a99) with white text. Secondary buttons use a Slate Navy outline. All buttons use 4px corner radius and "Medium" weight Hanken Grotesk text.
- **Input Fields:** Use 1px #e2e8f0 borders. On focus, the border shifts to Data Blue (#3b82f6) with a 0px blur 2px offset "halo" in a lighter tint.
- **Cards:** White backgrounds, 1px border (#e2e8f0), no shadow. Headers within cards should have a subtle bottom border to separate titles from data.
- **Data Tables:** Alternate row striping using #f1f5f9. Headers should be `label-caps` in Slate Navy.
- **Chips/Badges:** Square corners or 2px radius only. Use "Success Green" for positive trends with a 10% opacity background of the same color for high legibility.
- **Sidebar:** Slate Navy (#0f172a) background with light-gray text for a high-contrast, "authoritative" navigation frame. Use the "Since 1989" mark in a small, low-contrast footer within the sidebar.
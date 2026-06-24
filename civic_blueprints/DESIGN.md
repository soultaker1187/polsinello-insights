# Design System Document: The Data Architect

## 1. Overview & Creative North Star

### Creative North Star: "The Digital Curator"
In a landscape of cluttered real estate portals, this design system rejects the "warehouse" aesthetic in favor of high-end editorial clarity. We do not just show listings; we curate market intelligence. The "Digital Curator" philosophy balances the cold precision of data with the warm, aspirational nature of luxury real estate.

By breaking the rigid, box-heavy grid common in the industry, we utilize **intentional asymmetry**, **overlapping elements**, and **tonal layering**. This system moves away from "Standard Web 2.0" by treating the screen as a series of physical, translucent planes. We lean into high-contrast typography scales to ensure that while the data is dense, the experience feels breathable and authoritative.

---

## 2. Colors & Surface Philosophy

The palette is anchored in deep, authoritative Navys and professional Blues, balanced by a sophisticated range of neutral surfaces that replace the need for structural lines.

### The "No-Line" Rule
**Strict Mandate:** 1px solid borders are prohibited for sectioning or grouping. 
Boundaries must be defined solely through background color shifts or subtle tonal transitions. Use `surface-container-low` for a section sitting on a `surface` background to create separation. This produces a modern, "seamless" interface that feels more like an app and less like a website.

### Surface Hierarchy & Nesting
Treat the UI as a series of physical layers—like stacked sheets of fine paper.
- **Level 0 (Base):** `surface` (#fbf9f8)
- **Level 1 (Sections):** `surface_container_low` (#f6f3f2)
- **Level 2 (Cards/Interaction):** `surface_container_lowest` (#ffffff)
- **Level 3 (Prominent Modals):** `surface_bright` (#fbf9f8)

### The "Glass & Gradient" Rule
To elevate CTAs and Floating Action Buttons beyond the "generic," use **Glassmorphism**. Floating elements (like search bars or map filters) should utilize `surface` colors with a 70-80% opacity and a `backdrop-blur` of 12px-20px. 

**Signature Texture:** Use a subtle linear gradient (135°) from `primary` (#002045) to `primary_container` (#1a365d) for hero backgrounds and primary buttons to add depth and "soul" that flat hex codes lack.

---

## 3. Typography: Authority Through Scale

We utilize **Inter** to maintain maximum legibility at high data densities. The hierarchy is designed to feel like a high-end financial journal.

*   **Display Scales (`display-lg` to `display-sm`):** Reserved for market headlines and hero price points. Use these sparingly to create "Moments of Impact" amidst dense data.
*   **Headline & Title:** Used for property addresses and section titles. Pair `headline-sm` with `label-md` (all caps, tracked out +10%) for a sophisticated, editorial categorization.
*   **Body & Labels:** `body-md` is the workhorse for property descriptions. `label-sm` should be used for metadata (sqft, baths, beds) to ensure the hierarchy remains clear even when the screen is information-rich.

---

## 4. Elevation & Depth

We convey importance through **Tonal Layering** rather than traditional drop shadows.

*   **The Layering Principle:** A "Search" card should not have a heavy shadow; it should be `surface_container_lowest` (#ffffff) sitting on a `surface_container` (#f0eded) background. The subtle contrast creates a natural "lift."
*   **Ambient Shadows:** If a floating effect is required (e.g., a mobile navigation bar), use a shadow color tinted with the `on_surface` (#1b1c1c) token at 4% opacity. 
    *   *Spec:* `box-shadow: 0 12px 32px rgba(27, 28, 28, 0.04);`
*   **The "Ghost Border" Fallback:** If a border is required for accessibility (e.g., input fields), use the `outline_variant` token at **20% opacity**. Never use 100% opaque borders.
*   **Glassmorphism:** Use `secondary_container` with 60% opacity for interactive map overlays to allow the map's texture to bleed through, maintaining context.

---

## 5. Components

### Search Bars & Integrated Filters
*   **Style:** Large, pill-shaped (`rounded-full`) containers using `surface_container_lowest`.
*   **Interaction:** On focus, the container should expand slightly using a `surface_bright` tint and a soft ambient shadow. Avoid "Search" buttons; use a minimal magnifying glass icon in `primary`.

### Property Cards
*   **No Dividers:** Forbid the use of divider lines within cards. Separate the price, address, and specs using vertical white space (use the `1.5rem` / `xl` spacing token).
*   **Badges:** Status badges (e.g., "Sold") use `tertiary_container` (#003f23) with `on_tertiary_container` text. Use `rounded-sm` for a sharp, professional "tag" look.
*   **Image:** 16:9 aspect ratio with a subtle `md` (0.75rem) corner radius.

### Buttons
*   **Primary:** Gradient from `primary` to `primary_container`. White text. No border.
*   **Secondary:** `surface_container_high` background with `on_primary_container` text.
*   **Tertiary:** Text-only, using `secondary` (#1960a3). Underline only on hover.

### Interactive Data Visualization
*   **Price Trends:** Use `tertiary_fixed_dim` (#74db9d) for growth lines.
*   **Grid Lines:** Forbid standard black/grey grid lines. Use `surface_container_highest` (#e4e2e1) at 50% opacity for a "barely-there" guide.

---

## 6. Do's and Don'ts

### Do
*   **Do** use asymmetrical layouts (e.g., a left-aligned headline with a right-shifted image) to create a premium feel.
*   **Do** use `on_surface_variant` (#43474e) for secondary text to reduce visual noise in data-heavy tables.
*   **Do** use ample white space. If a layout feels "tight," double the padding.

### Don't
*   **Don't** use 1px dividers to separate list items. Use a background toggle (`surface` to `surface_container_low`) or 24px of white space.
*   **Don't** use pure black (#000000) for text. Use `on_surface` (#1b1c1c) to maintain a soft, high-end editorial tone.
*   **Don't** use standard "Success Green" (#00FF00). Only use the refined `success_green` (#38a169) or `tertiary` tokens provided.
*   **Don't** use "Drop Shadows" on cards. Use tonal elevation.
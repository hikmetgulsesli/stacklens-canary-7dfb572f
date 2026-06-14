---
name: StackLens Canary
colors:
  surface: '#131315'
  surface-dim: '#131315'
  surface-bright: '#39393b'
  surface-container-lowest: '#0e0e10'
  surface-container-low: '#1c1b1d'
  surface-container: '#201f22'
  surface-container-high: '#2a2a2c'
  surface-container-highest: '#353437'
  on-surface: '#e5e1e4'
  on-surface-variant: '#d1c6ab'
  inverse-surface: '#e5e1e4'
  inverse-on-surface: '#313032'
  outline: '#9a9078'
  outline-variant: '#4d4632'
  surface-tint: '#eec200'
  primary: '#ffecb9'
  on-primary: '#3c2f00'
  primary-container: '#facc15'
  on-primary-container: '#6c5700'
  inverse-primary: '#735c00'
  secondary: '#c8c6c9'
  on-secondary: '#303033'
  secondary-container: '#47464a'
  on-secondary-container: '#b6b4b8'
  tertiary: '#eeecf5'
  on-tertiary: '#303037'
  tertiary-container: '#d2d0d9'
  on-tertiary-container: '#595960'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffe083'
  primary-fixed-dim: '#eec200'
  on-primary-fixed: '#231b00'
  on-primary-fixed-variant: '#574500'
  secondary-fixed: '#e4e1e5'
  secondary-fixed-dim: '#c8c6c9'
  on-secondary-fixed: '#1b1b1e'
  on-secondary-fixed-variant: '#47464a'
  tertiary-fixed: '#e3e1ea'
  tertiary-fixed-dim: '#c7c5ce'
  on-tertiary-fixed: '#1b1b21'
  on-tertiary-fixed-variant: '#46464d'
  background: '#131315'
  on-background: '#e5e1e4'
  surface-variant: '#353437'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 30px
    fontWeight: '700'
    lineHeight: 36px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
    letterSpacing: -0.01em
  title-sm:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 24px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Hanken Grotesk
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  code-data:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  code-label:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 14px
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
  container-padding: 1.5rem
  element-gap: 0.75rem
  grid-gutter: 1rem
  stack-compact: 0.25rem
---

## Brand & Style
The design system is engineered for high-stakes operational monitoring and rapid-response technical environments. It adopts an **Industrial Professional** aesthetic, blending the precision of developer tools with the high-visibility requirements of a "Canary" monitoring system.

The personality is authoritative, transparent, and alert. It avoids all decorative ornamentation in favor of information density and functional clarity. The UI should evoke a sense of controlled urgency—providing all necessary data for a "go/no-go" decision at a glance. Visual hierarchy is established through structural borders and status-driven color signaling rather than shadow-based depth.

## Colors
The palette is optimized for long-term monitoring in low-light environments (Dark Mode default).

- **Foundation:** The system uses a Deep Charcoal (`#09090B`) for primary backgrounds to reduce eye strain, with Surface containers utilizing Zinc variants (`#18181B`, `#27272A`) to distinguish modular zones.
- **Accents:** "Canary Yellow" (`#FACC15`) is used sparingly as the primary action color and to highlight active focus states.
- **Semantic Logic:** Status colors are high-chroma to ensure critical alerts are never missed. Success Green, Error Red, and Warning Amber are the primary drivers of the user's attention.
- **Borders:** A consistent "Steel" border (`#3F3F46`) is used to define the high-density grid.

## Typography
This design system utilizes a dual-font strategy to separate UI controls from technical data:

1.  **Hanken Grotesk (UI Sans):** Used for all navigational elements, headers, and descriptive text. It provides a sharp, contemporary professional look that remains legible at small sizes.
2.  **JetBrains Mono (Technical Mono):** Used for all system-generated data, including Module IDs, timestamps, build hashes, and log entries. This ensures character alignment and reinforces the "industrial" nature of the tool.

**Formatting Rules:**
- Use `code-label` for table headers and metadata tags.
- Use `display-lg` exclusively for dashboard overview stats.
- Keep line heights tight to maximize vertical data density.

## Layout & Spacing
The layout follows a **Fixed-Fluid Hybrid** model designed for ultra-wide monitoring displays. 

- **Grid:** A strict 12-column system is used for top-level modules.
- **Density:** We utilize a 4px base unit. Component internal padding is kept to a minimum (8px or 12px) to allow for more data rows per viewport.
- **Breakpoints:**
    - **Desktop (Default):** 1280px+ (Full visibility).
    - **Tablet:** 768px-1279px (Modules stack into 2 columns; side navigation collapses).
    - **Mobile:** Not prioritized for full operations, but functional via single-column linear stack for alert reviewing.
- **Rhythm:** Elements are separated by "Steel" borders rather than whitespace to maintain a tight, structural feeling.

## Elevation & Depth
This design system rejects traditional shadows and blurred depth in favor of **Tonal Layering and Borders**.

- **Z-0 (Background):** `#09090B`. The base canvas.
- **Z-1 (Modules):** `#18181B`. All dashboard cards and data containers.
- **Z-2 (Interactive):** `#27272A`. Input fields, hover states, and dropdown menus.
- **Separation:** Depth is communicated via 1px solid borders (`#3F3F46`). 
- **Focus:** Active states use the Canary Yellow (`#FACC15`) as a 2px inner-border or a high-contrast outline, ensuring no ambiguity about where the cursor is positioned.

## Shapes
The shape language is "Soft-Industrial." We use a very subtle corner radius (4px) to prevent the UI from feeling aggressive while maintaining a rigid, professional structure.

- **Standard Elements:** 4px (Soft) for cards, buttons, and inputs.
- **Status Badges:** 2px or sharp corners to differentiate from interactive buttons.
- **Data Visualizations:** Rectilinear bars; no rounded ends on charts or progress indicators.

## Components
Consistent implementation of these components is vital for maintaining the high-density professional look:

- **Buttons:** 
    - *Primary:* Solid Canary Yellow background, black text, bold weight.
    - *Secondary:* Transparent background, 1px Steel border, white text.
    - *Destructive:* Solid red background, white text.
- **Status Badges:** Compact rectangles with low-opacity background tints and high-opacity text (e.g., Error: 10% Red BG, 100% Red Text). Include a 4px circular dot for immediate color recognition.
- **Data Tables:** No outer padding on the table container. Zebra striping is disabled; use 1px horizontal dividers only. Monospace font for numerical data.
- **Input Fields:** Darker than the card background (`#09090B`). Use JetBrains Mono for text entry to ensure alignment with data display.
- **Canary Monitor Cards:** Top-level containers featuring a "Header Strip" that changes color based on the system health within that module (e.g., a 4px top border in Green, Yellow, or Red).
- **Log Viewer:** A dedicated component using a black background, `code-data` typography, and timestamp-based gutter markers.
---
name: Warung Modern POS
colors:
  surface: '#f9f9ff'
  surface-dim: '#cfdaf2'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f0f3ff'
  surface-container: '#e7eeff'
  surface-container-high: '#dee8ff'
  surface-container-highest: '#d8e3fb'
  on-surface: '#111c2d'
  on-surface-variant: '#4f4632'
  inverse-surface: '#263143'
  inverse-on-surface: '#ecf1ff'
  outline: '#817660'
  outline-variant: '#d3c5ac'
  surface-tint: '#775a00'
  primary: '#775a00'
  on-primary: '#ffffff'
  primary-container: '#ffc61a'
  on-primary-container: '#6e5400'
  inverse-primary: '#f6be0a'
  secondary: '#855300'
  on-secondary: '#ffffff'
  secondary-container: '#fea619'
  on-secondary-container: '#684000'
  tertiary: '#006c49'
  on-tertiary: '#ffffff'
  tertiary-container: '#57e6aa'
  on-tertiary-container: '#006444'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdf98'
  primary-fixed-dim: '#f6be0a'
  on-primary-fixed: '#251a00'
  on-primary-fixed-variant: '#5a4300'
  secondary-fixed: '#ffddb8'
  secondary-fixed-dim: '#ffb95f'
  on-secondary-fixed: '#2a1700'
  on-secondary-fixed-variant: '#653e00'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#f9f9ff'
  on-background: '#111c2d'
  surface-variant: '#d8e3fb'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 3rem
    fontWeight: '700'
    lineHeight: 3.5rem
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 2rem
    fontWeight: '700'
    lineHeight: 2.5rem
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 1.5rem
    fontWeight: '700'
    lineHeight: 2rem
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 1.5rem
    fontWeight: '600'
    lineHeight: 2rem
  headline-sm:
    fontFamily: Space Grotesk
    fontSize: 1.25rem
    fontWeight: '600'
    lineHeight: 1.75rem
  price-xl:
    fontFamily: Inter
    fontSize: 2.25rem
    fontWeight: '700'
    lineHeight: 2.75rem
    letterSpacing: -0.02em
  price-lg:
    fontFamily: Inter
    fontSize: 1.5rem
    fontWeight: '700'
    lineHeight: 2rem
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 1.125rem
    fontWeight: '400'
    lineHeight: 1.75rem
  body-md:
    fontFamily: Inter
    fontSize: 1rem
    fontWeight: '400'
    lineHeight: 1.5rem
  body-sm:
    fontFamily: Inter
    fontSize: 0.875rem
    fontWeight: '400'
    lineHeight: 1.25rem
  label-lg:
    fontFamily: Inter
    fontSize: 1rem
    fontWeight: '600'
    lineHeight: 1.5rem
  label-md:
    fontFamily: Inter
    fontSize: 0.875rem
    fontWeight: '600'
    lineHeight: 1.25rem
  label-sm:
    fontFamily: Inter
    fontSize: 0.75rem
    fontWeight: '600'
    lineHeight: 1rem
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-lg: 1.5rem
  margin: 1rem
  margin-md: 1.5rem
  margin-lg: 2rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2rem
---

## Brand & Style

This design system serves Indonesian micro, small, and medium retail enterprises (warung, kelontong, and quick-service shops) transitioning from paper ledgers to rapid digital commerce. The interface projects reliability, speed, and approachability. 

The aesthetic blends Modern SaaS efficiency with tactile clarity:
- **Approachability:** Warm, inviting accents eliminate tech intimidation for shop owners operating during fast-paced customer rushes.
- **Utilitarian Clarity:** High contrast and prominent currency metrics ensure quick readouts under direct sunlight or dim fluorescent lighting.
- **Tactile Response:** Generous tap targets, clear active states, and physical affordances reassure merchants with every sale, scan, and checkout sequence.

## Colors

The palette balances energetic transaction accents with steady, readable structural tones:

- **Primary (`#FFC61A`):** Applied to primary actions, selected navigation items, and high-priority register buttons. Paired exclusively with dark slate text to maintain WCAG AAA legibility.
- **Secondary (`#F59E0B`):** Reserved for pending payments, cash-drawer adjustments, and secondary alert badges.
- **Tertiary (`#10B981`):** Indicates completed sales, settled QRIS payments, and positive inventory balances.
- **Neutral (`#1E293B`):** Serves as the primary text, structural border, and active icon color.
- **Canvas & Surface:** Built on clean slate tones (`#F8FAFC` for base background, `#FFFFFF` for product grids, transaction drawers, and order summary cards).

### Semantic & Functional Rules
- Never use `#FFC61A` with white typography; it must always pair with `#1E293B`.
- Currency amounts in checkout totals use `#1E293B` or `#10B981` depending on receipt status (unpaid vs. paid).
- Inactive states utilize `#E2E8F0` with `#94A3B8` iconography.

## Typography

The typography system pairs geometric, confident headlines with an analytical, highly legible body face:

- **Headings & Key Metrics:** Space Grotesk offers geometric structure and clear character definition, establishing structure across headers, quick-action tiles, and drawer titles.
- **Data, Prices & Cart Items:** Inter provides neutral clarity with tabular numerals (`tnum`), guaranteeing that Rupiah pricing columns align vertically down the decimal without shifting.

### Rupiah Price Formatting Rules
- All currency labels must prefix `Rp` directly without space or with a non-breaking space before the numerical value (e.g., `Rp15.000` or `Rp 15.000`).
- Always use `font-variant-numeric: tabular-nums` for cart lists, checkout summaries, and cash drawer tallies.

## Layout & Spacing

The layout is built around an asymmetric POS workspace split: an adaptive catalog view paired with a fixed checkout summary drawer.

### Grid & Breakpoints
- **Desktop / Tablet Landscape (≥ 1024px):** 12-column layout. 
  - Left panel (7–8 columns): Category navigation pills, search bar, and 3-to-4 column product SKU card grid.
  - Right panel (4–5 columns): Sticky order tray containing current bill items, discount inputs, payment trigger, and total readout.
- **Tablet Portrait (768px - 1023px):** Collapsible order drawer accessible via a sticky bottom bar displaying aggregate total and quantity count.
- **Mobile Handheld (< 768px):** Single-column stacked layout with full-width product tiles and an expandable sheet bottom drawer for final checkout.

### Touch Targets
- All interactive elements (keypad buttons, item cards, tender selection pills) must maintain a minimum bounding box of 48×48px to accommodate one-handed operation.

## Elevation & Depth

Visual separation relies on crisp border containment complemented by gentle, warm ambient shadowing:

- **Base Canvas:** `#F8FAFC`, flat zero elevation.
- **Card Tier 1 (Product Tiles, Tables):** Solid `#FFFFFF` background with a 1px border (`#E2E8F0`) and an ambient drop shadow: `0 1px 3px rgba(30, 41, 59, 0.04), 0 1px 2px rgba(30, 41, 59, 0.02)`.
- **Card Tier 2 (Cart Summary Drawer, Modal Dialogs):** `#FFFFFF` surface bounded by a subtle border (`#CBD5E1`) and directional elevation: `0 10px 15px -3px rgba(30, 41, 59, 0.08), 0 4px 6px -4px rgba(30, 41, 59, 0.03)`.
- **Active Focus / Selection:** Accent glow using primary yellow (`0 0 0 3px rgba(255, 198, 26, 0.35)`) combined with a solid `#1E293B` outer boundary.

## Shapes

The interface implements a friendly yet controlled corner radius profile:

- **Base Radius (`0.5rem` / `8px`):** Inputs, dropdowns, table cells, and standard buttons.
- **Large Radius (`1rem` / `16px`):** Product SKU cards, summary side panels, and payment modal sheets.
- **Pill Radius (`9999px`):** Category filters, stock indicators, and numeric quantity adjuster buttons inside the cart.

## Components

### Buttons
- **Primary ("Bayar / Selesai"):** Solid `#FFC61A` fill, `#1E293B` bold text, minimum height 52px. Active press scales down slightly (`scale(0.98)`) for physical tactility.
- **Secondary ("Batal / Pending"):** White background with a 1.5px `#E2E8F0` border and `#1E293B` label. Hover shifts border to `#CBD5E1`.
- **Success ("Lunas / Cetak Struk"):** Solid `#10B981` fill with crisp white text.

### Product SKU Cards
- Contained in 16px rounded cards (`#FFFFFF`). Displays an optional thumbnail (top), item name (bold Space Grotesk, 2 lines max), current inventory badge, and tabular Rupiah price anchored at the bottom right.
- Tapping a card triggers an immediate increment in the cart with an instant outline flash (`#FFC61A`).

### Cart & Register Item Rows
- Compact layout with item title, unit price, quantity increment/decrement pill (`-` `qty` `+`), and total row price.
- High-contrast touch steppers with minimum 36px circular click targets.

### Input Fields & Keypads
- **Cash Input:** 56px height, font size `1.5rem` bold tabular Inter, anchored prefix "Rp" in muted slate.
- **Quick Cash Preset Chips:** Rounded pills displaying denomination shortcuts (e.g., `Pas`, `Rp 20.000`, `Rp 50.000`, `Rp 100.000`) for rapid single-tap tender.

### Status Chips & Badges
- **Paid (Lunas):** Light green tint (`#ECFDF5`), `#065F46` label, 4px inner dot.
- **Unpaid / Debt (Kasbon):** Light amber tint (`#FEF3C7`), `#92400E` label.
- **Out of Stock (Habis):** Slate tint (`#F1F5F9`), `#64748B` label.
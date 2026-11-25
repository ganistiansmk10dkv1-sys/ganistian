---
name: Navy Periwinkle Portfolio
colors:
  surface: '#1E266B'
  surface-dim: '#080d3d'
  surface-bright: '#303565'
  surface-container-lowest: '#030638'
  surface-container-low: '#111645'
  surface-container: '#151a49'
  surface-container-high: '#202554'
  surface-container-highest: '#2b3060'
  on-surface: '#dfe0ff'
  on-surface-variant: '#c9c4d6'
  inverse-surface: '#dfe0ff'
  inverse-on-surface: '#272c5b'
  outline: '#928e9f'
  outline-variant: '#474554'
  surface-tint: '#c8bfff'
  primary: '#c8bfff'
  on-primary: '#2d009d'
  primary-container: '#907eff'
  on-primary-container: '#26008b'
  inverse-primary: '#5c47cd'
  secondary: '#bdc2ff'
  on-secondary: '#172186'
  secondary-container: '#313b9d'
  on-secondary-container: '#a8afff'
  tertiary: '#7bd0ff'
  on-tertiary: '#00354a'
  tertiary-container: '#009bd1'
  on-tertiary-container: '#002d40'
  error: '#F87171'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e5deff'
  primary-fixed-dim: '#c8bfff'
  on-primary-fixed: '#190064'
  on-primary-fixed-variant: '#442bb4'
  secondary-fixed: '#e0e0ff'
  secondary-fixed-dim: '#bdc2ff'
  on-secondary-fixed: '#000767'
  on-secondary-fixed-variant: '#313b9d'
  tertiary-fixed: '#c4e7ff'
  tertiary-fixed-dim: '#7bd0ff'
  on-tertiary-fixed: '#001e2c'
  on-tertiary-fixed-variant: '#004c69'
  background: '#080d3d'
  on-background: '#dfe0ff'
  surface-variant: '#2b3060'
  text-primary: '#F3F4F8'
  text-secondary: '#B8BEE0'
  border: '#8E84E8'
  success: '#34D399'
  warning: '#FBBF24'
typography:
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 46px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 30px
    fontWeight: '700'
    lineHeight: 36px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 34px
  headline-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 26px
  title-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 26px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 15px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 20px
  label-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1.5rem
  margin: 1.5rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2rem
---

## Brand & Style

This design system is built for a single-page personal UI/UX portfolio targeting recruiters and product teams. It balances creative personality with scannable structure, evoking a focused, modern, and technically grounded impression.

The visual direction combines **Corporate / Modern** clarity with **Dark-Mode Minimalism**:
- A deep navy canvas overlaid with a subtle technical grid (`40px × 40px`) establishes an architectural, design-oriented atmosphere.
- Periwinkle and violet pill-shaped accents guide attention to interactive actions, active navigation states, and key metrics without visual clutter.
- Pure black (`#000000`) and pure white (`#FFFFFF`) are strictly avoided to prevent harsh glare and maintain cohesive tonal harmony.

## Colors

The palette operates in **dark mode** by default, anchored by deep navy surfaces and high-contrast off-white typography:

- **Background (`#131847`)**: Primary page canvas, paired with a subtle technical grid overlay (`rgba(142, 132, 232, 0.08)` at `40px × 40px`).
- **Surface (`#1E266B`)**: Elevated container background for project showcase frames, cards, and the expertise dock, separating foreground content from the grid canvas.
- **Primary (`#7E6BF1`) & Border (`#8E84E8`)**: Used for active pill outlines, interactive button hover fills, keyboard focus rings, and subtle container borders.
- **Secondary (`#4C56B8`) & Tertiary (`#38BDF8`)**: Used for status badges, statistical pills, and secondary visual highlights.
- **Text Primary (`#F3F4F8`) & Text Secondary (`#B8BEE0`)**: Maintain high contrast (>7:1 to >12:1) for effortless scanning by recruiters without the harshness of pure white.
- **Semantic Colors**: `success` (`#34D399`), `warning` (`#FBBF24`), and `error` (`#F87171`) provide clear feedback states.

## Typography

**Plus Jakarta Sans** is used across all typographic roles for a clean, geometric, and contemporary voice.

- **Headlines**: Use weight `700` (Bold) with tight tracking (`-0.02em` on `headline-lg`) to establish clear section hierarchy. On mobile viewports, `headline-lg` scales down to `headline-lg-mobile` (`30px`).
- **Body**: Uses weights `400`–`500` with a generous `1.6` line-height ratio (`24px` at `15px` `body-md`) to keep profile descriptions, case study summaries, and contact details comfortable to read.
- **Labels**: Use weight `500` for navigation items, pill buttons, and metric badges.

## Layout & Spacing

The layout uses a **fixed-width centered container** (`1120px` maximum width) built on an **8px spacing grid** (`0.5rem` base unit).

- **Asymmetric 2-Column Split**: Sections alternate direction vertically (e.g., text-left / photo-right in the Hero, showcase-left / text-right in the Gallery) to maintain a dynamic yet orderly reading rhythm.
- **Responsive Adaptation**:
  - **Desktop (`>= 1024px`)**: Full 2-column asymmetric split within the `1120px` container, using `1.5rem` (`24px`) gutters and outer margins.
  - **Tablet (`768px – 1023px`)**: Maintains 2-column proportions where space permits, or collapses dense showcase grids while keeping `1.5rem` margins.
  - **Mobile (`< 768px`)**: Stacks into a single-column vertical flow with `1rem`–`1.5rem` outer margins and `2rem` (`space-xl`) vertical section separation.

## Elevation & Depth

Depth is achieved through **tonal layers** and **low-contrast outlines** rather than heavy black drop shadows:

- **Tonal Layering**: Stepping from the `#131847` background canvas to `#1E266B` surface containers clearly separates interactive modules and showcase frames.
- **Low-Contrast Outlines**: `1px solid #8E84E8` borders define container edges, pill buttons, and active navigation states.
- **Ambient Hover Glow**: Interactive elements use a soft periwinkle glow on hover to signal interactivity without breaking the flat, architectural aesthetic.

## Shapes

This design system uses a **Rounded** shape language (`0.5rem` / `8px` base) paired with full-pill accents for interactive controls:

- **Full Pill (`9999px`)**: Applied to action buttons, active navigation indicators, and statistical badges.
- **Large Rounded (`32px` / `2rem`)**: Applied to major container frames such as the project showcase wrapper and the expertise dock.
- **Medium Rounded (`12px` / `0.75rem`)**: Applied to UI/UX thumbnail cards nested inside showcase frames.
- **Small Rounded (`8px` / `0.5rem`)**: Applied to compact inputs and secondary elements.

## Components

All interactive components must maintain a minimum **`44×44px` touch target** and display a clear, high-contrast keyboard focus ring (`#8E84E8` / `#7E6BF1`).

- **Buttons**: Pill-shaped (`9999px` radius) with `10px 24px` padding, transparent background, `#F3F4F8` text, and `1px solid #8E84E8` border. On hover, the background transitions to `#7E6BF1`.
- **Chips & Badges**: Pill-shaped (`9999px` radius) with `6px 16px` padding, `#4C56B8` background, and `#F3F4F8` text for status indicators and skill metrics.
- **Cards**: `#1E266B` surface fill, `1px solid #8E84E8` border, `12px` radius for thumbnail cards, and `32px` radius for outer showcase frames.
- **Lists**: Clean vertical rhythm with `8px`–`16px` (`space-sm` to `space-md`) item gaps and `#B8BEE0` secondary text for supporting metadata.
- **Input Fields**: `#1E266B` surface fill, `1px solid #8E84E8` border, `8px` radius, `#F3F4F8` input text, and `#B8BEE0` placeholder text.
- **Checkboxes & Radio Buttons**: `1px solid #8E84E8` outline on `#1E266B` surface; checked states fill with `#7E6BF1` and `#F3F4F8` indicator marks.
- **Top Navbar**: Single-row navigation with the brand label on the left and section links on the right; the active item is framed with a pill border.
- **Showcase Frame**: Large `32px`-rounded `#1E266B` container grouping 3 aligned UI/UX screen previews with a `- Design Project -` label and click-to-preview modal support.
- **Expertise Dock**: Pill-shaped container housing 4 circular (`64px`) design tool icons alongside an average proficiency badge.
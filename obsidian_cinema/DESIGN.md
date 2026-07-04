---
name: Obsidian Cinema
colors:
  surface: '#17130a'
  surface-dim: '#17130a'
  surface-bright: '#3e382d'
  surface-container-lowest: '#120e05'
  surface-container-low: '#201b11'
  surface-container: '#241f15'
  surface-container-high: '#2f291f'
  surface-container-highest: '#3a3429'
  on-surface: '#ece1d1'
  on-surface-variant: '#d3c5ac'
  inverse-surface: '#ece1d1'
  inverse-on-surface: '#353025'
  outline: '#9b8f79'
  outline-variant: '#4f4633'
  surface-tint: '#f7be1d'
  primary: '#ffd165'
  on-primary: '#3f2e00'
  primary-container: '#eab308'
  on-primary-container: '#604700'
  inverse-primary: '#785a00'
  secondary: '#b7c8e1'
  on-secondary: '#213145'
  secondary-container: '#3a4a5f'
  on-secondary-container: '#a9bad3'
  tertiary: '#adddff'
  on-tertiary: '#00344c'
  tertiary-container: '#60c5ff'
  on-tertiary-container: '#005072'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdf9a'
  primary-fixed-dim: '#f7be1d'
  on-primary-fixed: '#251a00'
  on-primary-fixed-variant: '#5a4300'
  secondary-fixed: '#d3e4fe'
  secondary-fixed-dim: '#b7c8e1'
  on-secondary-fixed: '#0b1c30'
  on-secondary-fixed-variant: '#38485d'
  tertiary-fixed: '#c7e7ff'
  tertiary-fixed-dim: '#83cfff'
  on-tertiary-fixed: '#001e2e'
  on-tertiary-fixed-variant: '#004c6c'
  background: '#17130a'
  on-background: '#ece1d1'
  surface-variant: '#3a3429'
typography:
  display-lg:
    fontFamily: Montserrat
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style

The design system is engineered to evoke the immersive, high-stakes atmosphere of a premium theater. It targets cinephiles and critics who value a sophisticated, "lean-back" digital experience that prioritizes visual storytelling and authoritative critique.

The aesthetic blends **Minimalism** with **Glassmorphism**. By using deep obsidian backgrounds and translucent overlays, the UI recedes into the periphery, allowing high-resolution movie stills and vibrant cinematic content to take center stage. The emotional response is one of exclusivity, focus, and modern elegance.

## Colors

The palette is strictly nocturnal, utilizing varying depths of black to create a natural visual hierarchy.

*   **Primary (Cinematic Gold):** Reserved for high-intent actions, star ratings, and critical highlights. It provides a sharp, prestigious contrast against the dark base.
*   **Neutral (Obsidian & Charcoal):** The foundation. `#0A0A0A` is used for the absolute background, while `#121212` defines the primary surface containers.
*   **Secondary (Slate Gray):** Used for metadata, secondary labels, and icon outlines to ensure they remain legible without competing with the primary content.
*   **Glass Accents:** A semi-transparent surface used for floating navigation and overlay cards, paired with a heavy backdrop blur (20px-30px).

## Typography

This design system uses a dual-font approach to balance personality with utility. 

**Montserrat** is used for headlines and display text. Its geometric precision and bold weights provide the "professional/editorial" feel required for a critique platform. 

**Inter** handles all body copy, metadata, and interface labels. Its high x-height and neutral character ensure maximum readability against dark backgrounds, preventing eye strain during long-form review reading. All labels use uppercase styling with slight tracking to enhance the premium feel.

## Layout & Spacing

The layout follows a **Fluid Grid** model with generous breathing room to mimic a wide-screen cinematic aspect ratio. 

*   **Desktop:** A 12-column grid with 24px gutters. Content is capped at 1280px to maintain readability.
*   **Mobile:** A 4-column grid with 16px margins. Movie posters often switch from horizontal rows to a vertical scroll or a focused 2-column masonry.
*   **Spacing Rhythm:** Based on an 8px scale. Use `stack-lg` for separating distinct sections (e.g., Cast vs. Reviews) and `stack-sm` for internal component grouping (e.g., Title vs. Rating).

## Elevation & Depth

Depth is established primarily through **Glassmorphism** and subtle **Tonal Layering**.

1.  **Level 0 (Base):** Obsidian (`#0A0A0A`) background.
2.  **Level 1 (Cards/Sections):** Charcoal (`#121212`) surfaces with a 1px inner border of `white/0.05` to define edges without using heavy shadows.
3.  **Level 2 (Overlays/Nav):** Semi-transparent glass (`rgba(30, 30, 30, 0.6)`) with a `backdrop-filter: blur(24px)`. 
4.  **Shadows:** Use large, ultra-soft ambient shadows (`0 20px 40px rgba(0,0,0,0.4)`) only for elements that physically float over content, such as modals or dropdown menus.

## Shapes

The shape language is consistently **Rounded (Level 2)**. 

*   **Movie Posters/Cards:** 1rem (16px) corner radius to soften the high-contrast edges of the dark UI.
*   **Buttons & Genre Tags:** Use `rounded-xl` or full pill shapes to create a tactile, "touch-friendly" appearance that contrasts with the architectural grid.
*   **Inputs:** Match the card radius (16px) for a unified form language.

## Components

### Buttons & Actions
Primary buttons are Cinematic Gold (`#EAB308`) with black text. Hover states should include a slight glow effect (box-shadow with primary color at low opacity). Secondary buttons are "Ghost" style with a slate gray border.

### Movie Cards
Cards feature a "Float-up" hover effect: a subtle scale-up (1.02x) and an increase in the glass overlay intensity. Information like "Year" and "Genre" should appear as a glass-morphic tooltip or a bottom-aligned gradient overlay.

### Rating Stars
Use solid Cinematic Gold for filled stars and Slate Gray for empty ones. Include a subtle glow on the active rating to emphasize the "star power."

### Genre Tags
Pill-shaped containers with a semi-transparent background (`white/0.1`) and `label-sm` typography. They should be compact and non-intrusive.

### Sophisticated Navigation Bar
A fixed-top glassmorphic bar. The background should be nearly invisible until the user scrolls, at which point the backdrop-blur increases to maintain legibility over moving content.
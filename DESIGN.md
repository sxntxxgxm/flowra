---
name: Hyper-Focus Nebula
colors:
  surface: '#051424'
  surface-dim: '#051424'
  surface-bright: '#2c3a4c'
  surface-container-lowest: '#010f1f'
  surface-container-low: '#0d1c2d'
  surface-container: '#122131'
  surface-container-high: '#1c2b3c'
  surface-container-highest: '#273647'
  on-surface: '#d4e4fa'
  on-surface-variant: '#ccc3d8'
  inverse-surface: '#d4e4fa'
  inverse-on-surface: '#233143'
  outline: '#958da1'
  outline-variant: '#4a4455'
  surface-tint: '#d2bbff'
  primary: '#d2bbff'
  on-primary: '#3f008e'
  primary-container: '#7c3aed'
  on-primary-container: '#ede0ff'
  inverse-primary: '#732ee4'
  secondary: '#4cd7f6'
  on-secondary: '#003640'
  secondary-container: '#03b5d3'
  on-secondary-container: '#00424e'
  tertiary: '#ddb8ff'
  on-tertiary: '#490081'
  tertiary-container: '#844abe'
  on-tertiary-container: '#f2e0ff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#eaddff'
  primary-fixed-dim: '#d2bbff'
  on-primary-fixed: '#25005a'
  on-primary-fixed-variant: '#5a00c6'
  secondary-fixed: '#acedff'
  secondary-fixed-dim: '#4cd7f6'
  on-secondary-fixed: '#001f26'
  on-secondary-fixed-variant: '#004e5c'
  tertiary-fixed: '#f0dbff'
  tertiary-fixed-dim: '#ddb8ff'
  on-tertiary-fixed: '#2c0051'
  on-tertiary-fixed-variant: '#62259b'
  background: '#051424'
  on-background: '#d4e4fa'
  surface-variant: '#273647'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Space Grotesk
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
  unit: 4px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
  container-max: 1280px
---

## Brand & Style

The design system is engineered to evoke a sense of "deep work" within a high-tech, futuristic environment. It targets high-performing professionals and digital creatives who require a distraction-free yet visually stimulating workspace. 

The visual style is a fusion of **Glassmorphism** and **Vaporwave Futurism**. It utilizes a dark, void-like foundation to eliminate eye strain, contrasted by high-energy neon accents that signify action and progress. The aesthetic is defined by "light-as-material," where elements appear to be powered by internal energy sources, using glows and gradients to guide the user's attention through the productivity flow.

## Colors

The color palette is anchored in deep blacks and navy-greys to create infinite depth. 

- **Primary (Electric Purple):** Used for primary actions and "state of flow" indicators.
- **Secondary (Cyan):** Used for secondary actions, success states, and data visualization.
- **Gradients:** The signature "Flow Gradient" transitions from Electric Purple (#7C3AED) at 0% to Cyan (#06B6D4) at 100%, typically at a 135-degree angle.
- **Neutrals:** A range of cool greys and slates are used for secondary text and borders to maintain high legibility without competing with the neon accents.

## Typography

The typography strategy prioritizes absolute clarity against dark backgrounds. 

**Inter** is the workhorse for this design system, providing a clean, neutral skeleton for complex data. For interactive labels and technical metadata, **Space Grotesk** is introduced to inject a subtle "tech-industrial" feel. 

Headlines should utilize tight letter-spacing to feel "locked-in" and architectural. Body text must maintain a generous line height (1.6) to ensure long-form tasks and notes remain readable in low-light environments.

## Layout & Spacing

This design system employs a **12-column fluid grid** for desktop and a **4-column grid** for mobile. 

A strict 4px base-unit scaling system (4, 8, 12, 16, 24, 32, 48, 64) ensures mathematical harmony. Layouts should emphasize vertical rhythm, using generous whitespace to separate distinct work "zones." 

For productivity dashboards, sidebars are fixed at 280px, while the main content area remains fluid to allow for multi-pane task management. Containers use a "safe area" padding of 24px to prevent content from touching the neon borders of the cards.

## Elevation & Depth

Depth is not communicated through traditional grey shadows, but through **Tonal Layering** and **Luminescence**.

1.  **Level 0 (Deep Space):** `#0D0D0D` - The base canvas.
2.  **Level 1 (Sub-surface):** `#111827` - Cards and panels.
3.  **Level 2 (Interactive):** Glassmorphic overlays with `backdrop-filter: blur(12px)` and 10% white opacity.

**Shadows:** Use "Glow Shadows" instead of black shadows. High-priority elements use a drop shadow with the color of the element (e.g., a purple button gets a blurred #7C3AED shadow at 30% opacity) to simulate a light source emitting from the UI component onto the background.

## Shapes

The design system utilizes a **Rounded (Level 2)** shape language to soften the futuristic aesthetic, making it feel approachable rather than clinical.

- **Standard Elements:** 8px radius (buttons, small inputs).
- **Cards/Containers:** 16px radius.
- **Large Sections/Modals:** 24px radius.
- **Neon Borders:** Borders should be 1px or 1.5px thick. Use a linear gradient for borders that matches the primary brand gradient, creating a "wireframe" effect that glows at the edges.

## Components

### Glowing CTA Buttons
Primary buttons use the full Purple-to-Cyan gradient background with white text. Apply a `box-shadow: 0 0 20px rgba(124, 58, 237, 0.4)` to create the glowing effect. On hover, the intensity of the glow increases.

### Neon-Bordered Cards
Cards use the `#111827` background. The border is a 1px gradient stroke. To enhance the "neon" feel, apply a subtle inner-glow (`box-shadow: inset 0 0 8px rgba(6, 182, 212, 0.1)`).

### Tabular Pricing
Pricing tables should be border-collapsed with "Ghost Rows." The active/recommended plan card is elevated with a full-neon border and a backdrop blur. Use **Space Grotesk** for currency and numerical data to emphasize the technical nature of the app.

### Input Fields
Inputs are dark (`#0D0D0D`) with a 1px slate border. Upon focus, the border transitions to the Electric Purple gradient and a subtle outer glow activates.

### Progress Indicators
Progress bars use a "Pulse" animation, where a highlight light-streak travels across the Cyan gradient bar from left to right every 3 seconds.
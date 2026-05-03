---
name: Cosmic Cinematic
colors:
  surface: '#111415'
  surface-dim: '#111415'
  surface-bright: '#373a3b'
  surface-container-lowest: '#0c0f10'
  surface-container-low: '#191c1d'
  surface-container: '#1d2021'
  surface-container-high: '#282a2b'
  surface-container-highest: '#323536'
  on-surface: '#e1e3e4'
  on-surface-variant: '#d4c0d7'
  inverse-surface: '#e1e3e4'
  inverse-on-surface: '#2e3132'
  outline: '#9d8ba0'
  outline-variant: '#514255'
  surface-tint: '#ecb2ff'
  primary: '#ecb2ff'
  on-primary: '#520071'
  primary-container: '#bd00ff'
  on-primary-container: '#ffffff'
  inverse-primary: '#9900cf'
  secondary: '#fface8'
  on-secondary: '#5e0053'
  secondary-container: '#ff24e4'
  on-secondary-container: '#520049'
  tertiary: '#c8c6c8'
  on-tertiary: '#313032'
  tertiary-container: '#777578'
  on-tertiary-container: '#fffeff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#f8d8ff'
  primary-fixed-dim: '#ecb2ff'
  on-primary-fixed: '#320047'
  on-primary-fixed-variant: '#74009f'
  secondary-fixed: '#ffd7f0'
  secondary-fixed-dim: '#fface8'
  on-secondary-fixed: '#3a0033'
  on-secondary-fixed-variant: '#840076'
  tertiary-fixed: '#e5e1e4'
  tertiary-fixed-dim: '#c8c6c8'
  on-tertiary-fixed: '#1c1b1d'
  on-tertiary-fixed-variant: '#474649'
  background: '#111415'
  on-background: '#e1e3e4'
  surface-variant: '#323536'
typography:
  display-xl:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '300'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '300'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '400'
    lineHeight: '1.3'
    letterSpacing: normal
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '300'
    lineHeight: '1.6'
    letterSpacing: 0.01em
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: normal
  label-sm:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1440px
  gutter: 24px
  margin-edge: 64px
  section-gap: 160px
---

## Brand & Style

This design system is built to evoke the vastness and mystery of the deep cosmos. The brand personality is awe-inspiring, quiet, and high-fidelity, targeting an audience that values immersion and cinematic storytelling. 

The aesthetic is a sophisticated blend of **Glassmorphism** and **Minimalism**. It relies on high-transparency layers to simulate the thinness of gas clouds and the clarity of a vacuum. Every interaction should feel like a soft ripple in a gravitational field, prioritizing smooth, eased transitions over abrupt state changes. The UI does not sit on top of the content; it floats within it.

## Colors

The palette is anchored in the "Infinite Deep"—a base layer of near-black that serves as the canvas for celestial light. 

- **Primary (Cosmic Purple):** Used for interactive highlights and focal points that draw the eye through the "void."
- **Secondary (Nebula Pink):** Reserved for energetic accents, status indicators, or subtle glow effects behind primary elements.
- **Surface Neutrals:** A range of ultra-low-opacity whites and grays used to define structure without obstructing the background nebula gradients.
- **Accents:** Subtle gradient washes (0-15% opacity) should be used in the background to simulate gas clouds, moving slowly as the user scrolls.

## Typography

The typography is ethereal and structured. **Space Grotesk** provides a technical, futuristic edge for large displays, while **Manrope** ensures high-fidelity readability for body text. 

Weights should remain predominantly light (300-400) to maintain an airy, weightless feel. For headlines, negative letter spacing is used to create a "gravitational pull" between characters, while labels use expanded tracking to feel like distant constellations.

## Layout & Spacing

This design system utilizes a **fluid grid** with generous internal breathing room to reinforce the sense of space. Sections are separated by large vertical gaps to allow the background nebula accents to take center stage during the scroll.

The layout philosophy emphasizes "float." Content should rarely feel "boxed in." Instead, use wide margins and varying offsets to create a sense of three-dimensional depth as the user traverses the page.

## Elevation & Depth

Depth is achieved through **Glassmorphism** and light-based hierarchy rather than traditional shadows. 

1.  **The Void (Level 0):** The base black background with moving nebula gradients.
2.  **Atmospheric Layers (Level 1):** Large containers using a subtle `backdrop-filter: blur(20px)` and a 5% white fill.
3.  **Celestial Objects (Level 2):** Active elements and cards with a 1px "stellar" border—a linear gradient border from transparent to cosmic purple.
4.  **Luminance (Interaction):** Hover states should trigger a soft outer glow (`box-shadow` with high blur, 0px spread) using the primary cosmic purple.

## Shapes

The shape language is organic yet controlled. Standard UI elements use a **rounded** (0.5rem) base to feel approachable and smooth. For larger immersive containers, use `rounded-xl` (1.5rem) to mimic the soft curvature of planetary horizons. Avoid sharp 90-degree angles to maintain the fluid, cinematic flow of the interface.

## Components

### Buttons
Buttons are the centerpiece of the interaction model. They feature a transparent background with a thin, iridescent border. On hover, the button container remains static, but the **text inside performs a fluid animation**: characters should slightly shift or "shimmer" with a color-cycle effect from Cosmic Purple to Nebula Pink, simulating flowing energy.

### Cards
Cards use a high-blur glassmorphic effect. Content inside should appear to float. Ensure the background nebula accents are visible through the cards to maintain environmental immersion.

### Input Fields
Inputs are minimalist, defined only by a bottom border that glows when focused. The placeholder text should be a dimmed neutral-400, appearing like distant starlight.

### Scroll Progress Indicator
A custom vertical line on the far right of the viewport, using a gradient mask to show the user's "trajectory" through the cosmic space.

### Chips & Tags
Small, pill-shaped elements with a faint purple glow. They should appear "self-lit," as if they are small LEDs floating in the dark.
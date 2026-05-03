---
name: Nocturne Editorial
colors:
  surface: '#121316'
  surface-dim: '#121316'
  surface-bright: '#38393c'
  surface-container-lowest: '#0d0e10'
  surface-container-low: '#1a1c1e'
  surface-container: '#1e2022'
  surface-container-high: '#292a2c'
  surface-container-highest: '#333537'
  on-surface: '#e3e2e5'
  on-surface-variant: '#c2c7ce'
  inverse-surface: '#e3e2e5'
  inverse-on-surface: '#2f3033'
  outline: '#8c9198'
  outline-variant: '#42474d'
  surface-tint: '#a8caed'
  primary: '#a8caed'
  on-primary: '#0c334f'
  primary-container: '#89aacc'
  on-primary-container: '#1b3f5c'
  inverse-primary: '#406180'
  secondary: '#9ecaff'
  on-secondary: '#003258'
  secondary-container: '#004e84'
  on-secondary-container: '#8ac0fd'
  tertiary: '#edbe84'
  on-tertiary: '#462a00'
  tertiary-container: '#cb9f68'
  on-tertiary-container: '#543607'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#cee5ff'
  primary-fixed-dim: '#a8caed'
  on-primary-fixed: '#001d33'
  on-primary-fixed-variant: '#274967'
  secondary-fixed: '#d1e4ff'
  secondary-fixed-dim: '#9ecaff'
  on-secondary-fixed: '#001d36'
  on-secondary-fixed-variant: '#00497d'
  tertiary-fixed: '#ffddb6'
  tertiary-fixed-dim: '#edbe84'
  on-tertiary-fixed: '#2a1800'
  on-tertiary-fixed-variant: '#604012'
  background: '#121316'
  on-background: '#e3e2e5'
  surface-variant: '#333537'
typography:
  display-xl:
    fontFamily: Instrument Serif
    fontSize: 84px
    fontWeight: '400'
    lineHeight: '1.0'
  display-lg:
    fontFamily: Instrument Serif
    fontSize: 64px
    fontWeight: '400'
    lineHeight: '1.1'
  headline-md:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '300'
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
    lineHeight: '1.0'
    letterSpacing: 0.05em
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  unit: 4px
  container-max: 1200px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 64px
  section-gap: 160px
---

## Brand & Style

The design system is a high-fidelity, dark-themed framework tailored for a sophisticated professional portfolio. It draws heavily from **Minimalism** and **Glassmorphism**, merging the raw authority of editorial print with the fluid interactivity of modern digital interfaces. 

The aesthetic is defined by high-contrast compositions where deep blacks provide a void-like backdrop for crisp, white typography and ethereal blue accents. The emotional response is one of quiet confidence, technical precision, and premium artistry. Visual interest is generated through the juxtaposition of utilitarian sans-serifs against expressive, italicized serifs, alongside subtle motion found in animated gradient strokes.

## Colors

This design system utilizes a restricted, monochromatic base to ensure the content remains the focal point. The background uses a near-pure black to achieve maximum contrast with the primary text. 

The **Accent Gradient** is reserved for high-impact moments: interactive states, progress indicators, and thin-gauge animated borders. Surface colors are used sparingly to create containerized depth without breaking the dark-mode immersion. All strokes are kept at a low-light value (#1f1f1f) to maintain a seamless transition between surfaces and backgrounds.

## Typography

The typography strategy relies on a dramatic scale shift. **Instrument Serif** (always in its italic state) is used for large-scale display titles to inject personality and an editorial feel. 

**Inter** serves as the functional workhorse, providing extreme legibility across body copy and interface labels. Use `light` (300) weights for long-form reading to maintain the minimalist aesthetic, and `semibold` (600) for UI labels and subheadings to ensure structural clarity. Headlines should lean into tight line-heights and negative letter-spacing for a modern, compact look.

## Layout & Spacing

This design system follows a **Fixed Grid** philosophy for desktop, centered within the viewport to create generous negative space on the periphery. A 12-column grid is utilized with 24px gutters.

The spacing rhythm is intentional and "airy," using a 4px base unit. Section-to-section gaps are intentionally large (160px+) to allow the display typography to breathe and to signal clear transitions in the portfolio narrative. Bento-style layouts within the grid should use consistent internal padding (40px) to maintain a sense of luxury and order.

## Elevation & Depth

Hierarchy is established through **Glassmorphism** and **Tonal Layering** rather than traditional shadows. 

1.  **Level 0 (Background):** #0a0a0a. The base canvas.
2.  **Level 1 (Bento Cards):** #141414 with a 1px stroke of #1f1f1f.
3.  **Level 2 (Floating UI):** Navigation bars and floating action buttons utilize a 20px-40px backdrop-blur with a semi-transparent surface (#141414 at 70% opacity).
4.  **Level 3 (Interactive Modals):** High-opacity surfaces with a subtle outer glow using the primary accent color at 10% opacity to simulate light emission.

Depth is communicated via the clarity of the blur; elements closer to the user feature less transparency and more pronounced "frosted" effects.

## Shapes

The shape language is a mix of geometric extremes. 
- **Pill-shapes (Full Rounding):** Used for interactive elements like buttons, tags, and the primary navigation dock. This creates a soft, approachable touchpoint for the user.
- **Large Radius (24px - 32px):** Used for "Bento Cards" and image containers, providing a sophisticated, modern framing for project work.
- **Strict Square:** Reserved exclusively for small-scale icons or utility grid lines to provide a rhythmic counterpoint to the rounded containers.

## Components

### Buttons
Primary buttons are pill-shaped with a background matching the Accent Gradient. Text is dark (#0a0a0a) to ensure legibility. Secondary buttons use a ghost style: a 1px #1f1f1f stroke that transforms into an animated gradient stroke on hover.

### Bento Cards
Large containers with a 32px corner radius. These should feature a subtle 1px stroke (#1f1f1f). Internal content should have a minimum padding of 40px. Cards may feature "glass" overlays for metadata.

### Navigation (The Dock)
A floating, pill-shaped navbar positioned at the bottom or top center. It utilizes `backdrop-blur: 24px` and a semi-transparent surface. Active states are indicated by a small, 4px glowing dot using the primary accent color.

### Progress Indicators & Borders
Progress bars and specific container borders utilize the **Animated Gradient**. The gradient should slowly shift along the X-axis (linear-gradient movement) to provide a "living" feel to the interface without being distracting.

### Input Fields
Minimalist underlines or subtle #141414 blocks with rounded-sm (4px) corners. Focus states activate the blue accent stroke.
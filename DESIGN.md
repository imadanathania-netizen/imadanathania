---
name: Neon Nights
colors:
  surface: '#0b1323'
  surface-dim: '#0b1323'
  surface-bright: '#31394a'
  surface-container-lowest: '#060e1d'
  surface-container-low: '#131c2b'
  surface-container: '#18202f'
  surface-container-high: '#222a3a'
  surface-container-highest: '#2d3546'
  on-surface: '#dbe2f8'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#dbe2f8'
  inverse-on-surface: '#283041'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe9'
  primary: '#dbfcff'
  on-primary: '#00363a'
  primary-container: '#00f0ff'
  on-primary-container: '#006970'
  inverse-primary: '#006970'
  secondary: '#fface8'
  on-secondary: '#5e0053'
  secondary-container: '#ff24e4'
  on-secondary-container: '#520049'
  tertiary: '#e1ffd1'
  on-tertiary: '#053900'
  tertiary-container: '#33fb0a'
  on-tertiary-container: '#106e00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#7df4ff'
  primary-fixed-dim: '#00dbe9'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#ffd7f0'
  secondary-fixed-dim: '#fface8'
  on-secondary-fixed: '#3a0033'
  on-secondary-fixed-variant: '#840076'
  tertiary-fixed: '#79ff5b'
  tertiary-fixed-dim: '#2ae500'
  on-tertiary-fixed: '#022100'
  on-tertiary-fixed-variant: '#095300'
  background: '#0b1323'
  on-background: '#dbe2f8'
  surface-variant: '#2d3546'
typography:
  display-lg:
    fontFamily: Montserrat
    fontSize: 72px
    fontWeight: '900'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '800'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style
The design system is engineered for a high-energy, futuristic music festival experience. It captures the "Neon Nights" theme by blending **Cyberpunk-lite** aesthetics with modern **Glassmorphism**. 

The brand personality is electric, immersive, and nocturnal. It targets a digitally-native audience that craves sensory-rich environments. Visual hierarchy is established through high-contrast interactions where dark, deep-space backgrounds meet vibrant, self-illuminated UI elements. The interface should feel like a premium digital cockpit—functional yet visually spectacular.

## Colors
The palette is rooted in a **Deep Midnight** base to allow neon accents to "pop" with maximum luminance.

- **Primary (Electric Cyan):** Used for primary actions, active states, and core branding.
- **Secondary (Magenta Shock):** Used for secondary highlights, "Live" indicators, and artist categories.
- **Tertiary (Lime Green):** Reserved for success states and financial/ticket-related calls to action.
- **Accent (Bright Yellow):** Used sparingly for urgent alerts or special "VIP" tagging.
- **Neutral:** A range of deep navy-blacks (#020817) and slate greys to provide depth without pure black flatness.

Apply a 20px background blur to any surface using the `surface_glass` token to maintain legibility over vibrant festival photography.

## Typography
The typography system balances aggressive, geometric impact with technical precision. 

**Montserrat** is the voice of the festival, used in heavy weights for headlines to convey power and excitement. **Hanken Grotesk** provides a clean, neutral counterpoint for long-form content and artist bios, ensuring high legibility against dark backgrounds. **Space Grotesk** is used for utility labels and technical data (like set times and stage names), reinforcing the futuristic aesthetic.

All display text should utilize tight letter-spacing to feel more cohesive and "logo-like."

## Layout & Spacing
The layout follows a **Fluid Grid** model with a 12-column structure for desktop and a 4-column structure for mobile. 

We utilize a generous spacing rhythm to allow the "glow" of elements to breathe. Content cards should be grouped using 32px or 48px gaps to prevent the UI from feeling cluttered. Navigation is handled via a fixed-top "Glass" bar that stays visible, ensuring the user always has access to the Lineup and Tickets.

- **Mobile:** Elements stack vertically; margins are reduced to 16px to maximize screen real estate for imagery.
- **Desktop:** Wide margins (64px) create a cinematic, widescreen feel.

## Elevation & Depth
Depth is conveyed through **Light Emission** rather than traditional physical shadows. 

1.  **Level 0 (Base):** The deep midnight background.
2.  **Level 1 (Cards/Sections):** Semi-transparent glass containers with a subtle 1px border (`rgba(255,255,255,0.1)`).
3.  **Level 2 (Interactive):** Elements that emit a "Neon Glow." Use diffused outer glows (drop-shadows with 15-30px blur) using the primary or secondary accent colors at 30% opacity.
4.  **Level 3 (Overlays):** Modals and high-priority alerts use a darker backdrop dimming (80% opacity) with a vibrant, 2px neon border.

## Shapes
This design system utilizes **Soft** geometry. While the vibe is futuristic, overly sharp corners feel aggressive; the 0.25rem (4px) base roundedness provides a technical, "machined" look while remaining accessible. 

Interactive elements like buttons and chips may use a slightly higher roundedness (up to 8px) to distinguish them from structural layout containers.

## Components
- **Buttons:** Primary buttons feature a diagonal linear gradient (Cyan to Blue) with a white "inner glow" border. On hover, the button should scale 2% and increase its outer neon glow intensity.
- **Glass Cards:** Used for Artist profiles. Feature a `backdrop-filter: blur(20px)` and a subtle gradient stroke. The artist's name should use the `headline-md` style.
- **Neon Chips:** Small, pill-shaped tags for "Genre" or "Stage." These have a transparent fill and a solid neon border corresponding to the category.
- **Input Fields:** Dark backgrounds with a 1px bottom-border only. On focus, the border animates to a full neon cyan box-shadow.
- **Navigation Bar:** A sleek, top-anchored bar with 60% opacity. Navigation links use `label-caps` and glow slightly when hovered.
- **Schedule List:** Use high-contrast dividers and `Space Grotesk` for time-stamps to ensure the schedule is readable in low-light environments.
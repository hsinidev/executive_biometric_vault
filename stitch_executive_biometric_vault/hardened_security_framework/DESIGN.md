---
name: Hardened Security Framework
colors:
  surface: '#141313'
  surface-dim: '#141313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a29'
  surface-container-highest: '#353434'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c4c7c4'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8e918e'
  outline-variant: '#444845'
  surface-tint: '#c7c6c4'
  primary: '#ffffff'
  on-primary: '#303130'
  primary-container: '#e3e2e0'
  on-primary-container: '#646463'
  inverse-primary: '#5e5e5d'
  secondary: '#afc8f0'
  on-secondary: '#163152'
  secondary-container: '#2f486a'
  on-secondary-container: '#9eb7de'
  tertiary: '#ffffff'
  on-tertiary: '#313030'
  tertiary-container: '#e5e2e1'
  on-tertiary-container: '#656464'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e3e2e0'
  primary-fixed-dim: '#c7c6c4'
  on-primary-fixed: '#1b1c1b'
  on-primary-fixed-variant: '#464746'
  secondary-fixed: '#d4e3ff'
  secondary-fixed-dim: '#afc8f0'
  on-secondary-fixed: '#001c3a'
  on-secondary-fixed-variant: '#2f486a'
  tertiary-fixed: '#e5e2e1'
  tertiary-fixed-dim: '#c9c6c5'
  on-tertiary-fixed: '#1c1b1b'
  on-tertiary-fixed-variant: '#474646'
  background: '#141313'
  on-background: '#e5e2e1'
  surface-variant: '#353434'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  body-base:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  mono-label:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.1em
spacing:
  unit: 8px
  gutter: 24px
  margin: 40px
  border-thick: 3px
  border-thin: 1px
---

## Brand & Style

This design system is engineered to evoke the psychological profile of a high-clearance physical vault. It prioritizes the perception of **permanence, fortification, and absolute integrity**. The target audience includes high-net-worth individuals and security administrators who require a visual guarantee that their digital assets are as safe as physical bullion.

The visual style is a fusion of **Industrial Brutalism** and **Modern Tactile** design. It rejects the "lightness" of modern SaaS in favor of heavy structural elements, thick borders, and metallic textures. The interface should feel "milled" rather than "rendered," utilizing high-contrast transitions and monochromatic depth to signal technical sophistication and impenetrable security. Every interaction must feel intentional, heavy, and mechanical.

## Colors

The palette is strictly limited to metallic and deep oceanic tones to maintain a serious, high-stakes atmosphere.

*   **Platinum Silver (#E5E4E2):** Used for primary text, active states, and "brushed metal" surfaces. It serves as the high-contrast light source against the dark void.
*   **Deep Navy (#001F3F):** Acts as the secondary structural layer, used for "armored" containers and recessed areas to provide depth without resorting to pure black.
*   **Deep Black (#000000 / #0A0A0A):** The foundation. It represents the "void" of the vault interior, used for main backgrounds to make the platinum elements pop.
*   **Functional Accents:** Status colors are high-chroma (Matrix Green for access granted, Alert Red for security breaches) to ensure immediate cognitive recognition amidst the monochromatic scheme.

Apply metallic linear gradients (45-degree angle) using transitions from `#E5E4E2` to a slightly darker `#BDBAB7` to simulate light reflecting off steel.

## Typography

Typography in this design system is treated as technical data. We use **Hanken Grotesk** for headlines to provide a sharp, contemporary, and authoritative presence. Its geometric precision mirrors the engineering of a vault door.

**Geist** is employed for body copy to provide a developer-centric, high-tech aesthetic that remains highly legible during data-heavy tasks. For technical readouts, serial numbers, and biometric data, **JetBrains Mono** is used in all-caps to reinforce the industrial, machine-readable nature of the platform. All type should maintain high contrast—predominantly Platinum Silver on Deep Black.

## Layout & Spacing

The layout follows a **Rigid Fixed Grid** model. Elements do not "float"; they are locked into heavy structural containers. A 12-column grid is used for desktop, but with significantly larger gutters (24px) to emphasize the separation of "secure compartments."

Spacing is strictly based on an 8px base-unit. Use generous internal padding within components (minimum 24px) to convey a sense of heavy-duty construction. Alignment should be mathematical and precise; any asymmetry is considered a design failure. Containers should feel like modular blocks stacked or bolted together.

## Elevation & Depth

This design system eschews soft, ambient shadows. Depth is instead communicated through **Physical Extrusion and Recess**:

1.  **Beveled Edges:** Use 1px inner highlights (Platinum at 20% opacity) on the top/left edges and 1px inner shadows (Black at 50% opacity) on the bottom/right edges to create a "milled metal" effect.
2.  **Tonal Stacking:** The background is Deep Black. The primary containers are Deep Navy. Interactive elements are Platinum. This clear hierarchy creates a "layering of armor."
3.  **Inset States:** Input fields and inactive zones should appear "etched" into the surface using inner shadows, making them look like physical slots in a console.
4.  **Glass Secondary Layers:** For non-critical information overlays, use a heavy backdrop blur (20px) with a Deep Navy tint to maintain the sense of looking through thick, reinforced glass.

## Shapes

The shape language is **Aggressively Linear**. We use a `roundedness` of **0 (Sharp)** for all primary containers, buttons, and structural elements to emphasize hardness and industrial strength. 

Small UI elements like status "LEDs" or biometric sensors may use a 2px chamfer (angled corner) rather than a radius to maintain the machined aesthetic. Avoid circles unless they represent specific hardware components (like a vault dial or a camera lens).

## Components

*   **Buttons:** Must feel like physical switches. Use a 3px solid border of Platinum Silver. On hover, the button should fill with a metallic gradient and the text should invert to Deep Black.
*   **Input Fields:** Recessed styling. Use a Deep Black background with a 1px Deep Navy border. The cursor and active border should be a glowing "Security Green" or "Platinum."
*   **Cards/Containers:** These are "Vault Modules." They must feature a visible "header bar" in Deep Navy with a technical label in JetBrains Mono.
*   **Progress Bars:** Should resemble industrial gauges. Use segmented blocks rather than a smooth continuous fill to indicate "loading" or "scanning."
*   **Biometric Scanners:** Use thin, horizontal scanning lines that animate vertically. The framing should be heavy and industrial, with "Locked" and "Unlocked" states clearly differentiated by high-contrast color shifts.
*   **Icons:** Icons must be "Wireframe Industrial"—no rounded terminals, consistent 2px stroke weight, and sharp 90-degree angles. Use technical iconography (bolts, shields, keys, circuit paths).
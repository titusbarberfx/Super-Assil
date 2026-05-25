---
name: Mediterranean Orientalism
colors:
  surface: '#fbf9f9'
  surface-dim: '#dbdad9'
  surface-bright: '#fbf9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f5f3f3'
  surface-container: '#efeded'
  surface-container-high: '#e9e8e7'
  surface-container-highest: '#e3e2e2'
  on-surface: '#1b1c1c'
  on-surface-variant: '#444748'
  inverse-surface: '#303031'
  inverse-on-surface: '#f2f0f0'
  outline: '#747878'
  outline-variant: '#c4c7c7'
  surface-tint: '#5f5e5e'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1c1b1b'
  on-primary-container: '#858383'
  inverse-primary: '#c8c6c5'
  secondary: '#79591d'
  on-secondary: '#ffffff'
  secondary-container: '#fdd089'
  on-secondary-container: '#78581c'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#1b1c1a'
  on-tertiary-container: '#848481'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e5e2e1'
  primary-fixed-dim: '#c8c6c5'
  on-primary-fixed: '#1c1b1b'
  on-primary-fixed-variant: '#474746'
  secondary-fixed: '#ffdeac'
  secondary-fixed-dim: '#ebc07a'
  on-secondary-fixed: '#281900'
  on-secondary-fixed-variant: '#5f4105'
  tertiary-fixed: '#e4e2de'
  tertiary-fixed-dim: '#c8c6c3'
  on-tertiary-fixed: '#1b1c1a'
  on-tertiary-fixed-variant: '#474744'
  background: '#fbf9f9'
  on-background: '#1b1c1c'
  surface-variant: '#e3e2e2'
typography:
  headline-xl:
    fontFamily: Libre Caslon Text
    fontSize: 48px
    fontWeight: '400'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Libre Caslon Text
    fontSize: 32px
    fontWeight: '400'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Libre Caslon Text
    fontSize: 24px
    fontWeight: '400'
    lineHeight: '1.3'
  headline-xl-mobile:
    fontFamily: Libre Caslon Text
    fontSize: 36px
    fontWeight: '400'
    lineHeight: '1.1'
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
  label-sm:
    fontFamily: Hanken Grotesk
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.1em
spacing:
  base: 8px
  section-gap-desktop: 120px
  section-gap-mobile: 64px
  gutter: 24px
  container-max: 1280px
---

## Brand & Style

This design system embodies the intersection of Cartagena’s Mediterranean light and the rich heritage of Arabian perfumery. The aesthetic is rooted in **Minimalism** with a **Tactile** edge, prioritizing clarity, breathing room, and high-end material textures.

The target audience is the discerning traveler and local connoisseur looking for an artisanal, luxury experience. The UI must evoke a sense of calm, timelessness, and olfactory "space." By utilizing generous whitespace and a restricted, high-contrast palette, the design shifts focus entirely to the product photography and the "narrative" of the scents.

## Colors

The palette is anchored by **Off-white (#FDFBF7)**, which serves as the canvas, replicating the look of high-quality parchment or sun-bleached stone. 

- **Primary (Deep Charcoal):** Used for all critical communication, navigation, and typography to ensure grounded authority.
- **Secondary (Subtle Gold):** Reserved for high-intent actions, accents, and luxury markers. It should be used sparingly to maintain its value.
- **Neutrals:** Used for secondary labels and dividers to maintain a soft hierarchy without breaking the minimalist flow.

## Typography

The typography strategy balances the literary, authoritative weight of **Libre Caslon Text** for editorial storytelling with the clinical precision of **Hanken Grotesk**. 

Headlines should be treated as architectural elements—centered and spacious. Body text requires increased line-height (1.6) to prevent the "clutter" often found in retail interfaces. Labels utilize uppercase tracking (letter-spacing) to signify technical details or product categories, mimicking the labels on artisanal perfume bottles.

## Layout & Spacing

The design system employs a **Fixed Grid** on desktop (12 columns) and a **Fluid Grid** on mobile (4 columns). 

Layouts are characterized by "The Gallery View"—large margins and asymmetric placements that force the eye to move intentionally through the content. Avoid "crowding" at all costs; if a section feels full, increase the vertical padding. 

- **Desktop:** 120px vertical padding between major sections.
- **Mobile:** 64px vertical padding; margins should be 20px to maximize the visual impact of product imagery on small screens.

## Elevation & Depth

This design system avoids traditional drop shadows to maintain its high-end minimalist profile. Instead, it uses **Tonal Layers** and **Hard-Edge Depth**:

1.  **Surfaces:** Elements sit flush with the background. Separation is achieved through subtle shifts in tone (e.g., a slightly warmer cream for a card background) or ultra-thin 0.5px borders in #B89150.
2.  **Overlays:** When modals or menus are required, use a full-screen #FDFBF7 wash with high opacity (95%) to obscure the background, rather than a floating shadow box. This maintains the "physical room" feel.

## Shapes

The shape language is strictly **Sharp (0)**. 

Sharp corners evoke the precision of cut glass and the architectural lines of upscale boutiques. Rectilinear containers provide a framework that allows the organic, fluid shapes of perfume bottles and ingredients within the photography to stand out. This lack of rounding reinforces the "Professional" and "High-End" attributes of the system.

## Components

- **Buttons:** Primary buttons are solid Charcoal (#1A1A1A) with white Hanken Grotesk text, uppercase. Secondary buttons use a "Ghost" style: 1px Charcoal border, no fill, with a subtle hover state that transitions the background to the Gold/Bronze accent (#B89150).
- **Inputs:** Minimalist bottom-border only (1px Charcoal). Labels sit above the line in Label-SM typography. Error states are indicated by a thin Gold line rather than a harsh Red, to keep the luxury vibe intact.
- **Cards:** No borders, no shadows. The image takes up 100% of the card width, with typography left-aligned or centered beneath. 
- **Chips/Tags:** Small, rectangular boxes with a 0.5px Gold border. Used for "Scent Profiles" (e.g., *Oud*, *Jasmine*, *Musk*).
- **Navigation:** A centered logo with a transparent background. Links should have a subtle underline on hover, using the Gold accent.
- **Product Tiles:** Focus on high-resolution photography with a "hover-zoom" effect to show bottle details and texture.
---
name: Royal Taste Design Identity
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#d0c5af'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#99907c'
  outline-variant: '#4d4635'
  surface-tint: '#e9c349'
  primary: '#f2ca50'
  on-primary: '#3c2f00'
  primary-container: '#d4af37'
  on-primary-container: '#554300'
  inverse-primary: '#735c00'
  secondary: '#fff9ef'
  on-secondary: '#3a3000'
  secondary-container: '#ffdb3c'
  on-secondary-container: '#725f00'
  tertiary: '#d0cdcd'
  on-tertiary: '#313030'
  tertiary-container: '#b4b2b2'
  on-tertiary-container: '#454544'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffe088'
  primary-fixed-dim: '#e9c349'
  on-primary-fixed: '#241a00'
  on-primary-fixed-variant: '#574500'
  secondary-fixed: '#ffe16d'
  secondary-fixed-dim: '#e9c400'
  on-secondary-fixed: '#221b00'
  on-secondary-fixed-variant: '#544600'
  tertiary-fixed: '#e5e2e1'
  tertiary-fixed-dim: '#c8c6c5'
  on-tertiary-fixed: '#1c1b1b'
  on-tertiary-fixed-variant: '#474746'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-xl:
    fontFamily: Playfair Display
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '500'
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
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.15em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 20px
  section-gap: 80px
  element-gap: 16px
---

## Brand & Style

The design system is engineered to evoke a sense of exclusive, high-end culinary artistry. It targets a discerning audience that values both Gastronomy and Technology. The brand personality is "The Modern Aristocrat"—sophisticated and traditional in quality, yet ultra-modern and seamless in delivery.

The aesthetic utilizes **Glassmorphism** as its core structural driver, creating layers of depth that mimic high-end restaurant glassware and polished obsidian surfaces. The interface should feel expansive, utilizing significant whitespace (or "dark space") to let high-fidelity food photography serve as the primary visual anchor. Interactions must be fluid and rhythmic, emphasizing a "concierge-level" digital experience.

## Colors

This design system employs a deep, monochromatic base to provide a high-contrast stage for gold accents. 

- **Primary & Secondary:** Gold (#D4AF37) and Amber (#FFD700) are used sparingly for calls-to-action, branding elements, and active states to signify premium value.
- **Backgrounds:** The foundation is Obsidian (#0B0B0B), with Deep Charcoal (#1A1A1A) used for elevated surface containers.
- **Gradients:** Use subtle, linear gradients (e.g., Deep Charcoal to Obsidian) to prevent flat surfaces and add a metallic, brushed texture feel.
- **Interactive Accents:** Gold should be used for critical path elements, while Amber provides a warmer, "candlelit" glow for hover states and highlights.

## Typography

The typographic scale relies on the tension between the classic elegance of **Playfair Display** and the clinical precision of **Inter**.

- **Headlines:** Always use Playfair Display. For hero sections, use high-contrast weights to mimic luxury editorial layouts.
- **Body:** Inter is the workhorse for all descriptive text, menu items, and pricing, ensuring high legibility against dark backgrounds.
- **Micro-copy:** Use "label-caps" (Inter, Uppercase with wide tracking) for categories, small headers, and overlines to create a sense of organized, high-end cataloging.
- **Hierarchy:** Ensure a clear distinction between the "Editorial" voice (Serif) and the "Functional" voice (Sans-Serif).

## Layout & Spacing

The layout philosophy is rooted in **spaciousness**. In this design system, density is the enemy of luxury. 

- **Grid:** A 12-column fluid grid for desktop and a 4-column grid for mobile.
- **Rhythm:** Use an 8px base unit. Section gaps should be aggressive (80px+) to allow the eye to rest and focus on one signature dish at a time.
- **Margins:** Implement wide horizontal margins to create a "centered, boutique" feel, even on wider displays.
- **Photography:** Food imagery should often break the grid or occupy large, full-bleed containers to emphasize the "Royal" scale of the brand.

## Elevation & Depth

Elevation is achieved through optical transparency and light refraction rather than heavy shadows.

- **Glassmorphism:** Use `backdrop-filter: blur(20px)` on all primary containers. These "glass" sheets should have a very subtle 1px border using the `glass_stroke` token to define their edges against the dark background.
- **Shadows:** Use extremely soft, diffused shadows (Blur: 40px, Opacity: 0.3) with a slight gold tint (#D4AF37) for floating elements like the "Add to Cart" fab or featured menu cards.
- **Layering:** Level 0 is the Obsidian background. Level 1 is a Charcoal surface. Level 2 is the Glassmorphic container. Level 3 is the interactive element (buttons/badges).

## Shapes

The shape language combines architectural rigidity with soft touchpoints.

- **Containers:** Main cards and glass panels use `rounded-lg` (1rem) to feel approachable yet structured.
- **Interactive Elements:** Buttons and input fields should utilize `rounded-xl` (1.5rem) or full pill shapes to contrast against the more rectangular layout of the grid.
- **Imagery:** Food photography should feature either sharp, clean edges or be contained within sophisticated, organic mask shapes (like soft ovals) to reinforce the premium aesthetic.

## Components

- **Primary Buttons:** High-gloss gold gradient backgrounds with dark Inter SemiBold text. Include a subtle "shimmer" animation on hover.
- **Secondary Buttons:** Ghost style with a 1px gold border and `backdrop-filter` blur.
- **Glass Cards:** These are the primary containers for menu items. They feature a subtle inner glow and top-weighted gold border (0.5px).
- **Inputs:** Minimalist bottom-border only, or fully enclosed glass fields. The cursor and label-focus should transition to Gold (#D4AF37).
- **Interactive Menu Items:** On hover, cards should slightly scale up (1.02x) and the background blur intensity should increase.
- **Badges/Chips:** Use Amber (#FFD700) for "Chef's Special" or "Limited Edition" tags, using small, high-tracking uppercase Inter text.
- **Food Display:** Use "Ken Burns" style slow-zoom animations for hero photography to maintain a cinematic quality.
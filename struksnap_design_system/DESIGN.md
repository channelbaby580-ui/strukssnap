---
name: StrukSnap Design System
colors:
  surface: '#f8f9fa'
  surface-dim: '#d9dadb'
  surface-bright: '#f8f9fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f4f5'
  surface-container: '#edeeef'
  surface-container-high: '#e7e8e9'
  surface-container-highest: '#e1e3e4'
  on-surface: '#191c1d'
  on-surface-variant: '#41484d'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#71787e'
  outline-variant: '#c1c7ce'
  surface-tint: '#2e6385'
  primary: '#2e6385'
  on-primary: '#ffffff'
  primary-container: '#a5d8ff'
  on-primary-container: '#285f80'
  inverse-primary: '#9accf3'
  secondary: '#2f6a3f'
  on-secondary: '#ffffff'
  secondary-container: '#b2f2bb'
  on-secondary-container: '#357044'
  tertiary: '#7d5718'
  on-tertiary: '#ffffff'
  tertiary-container: '#fdc97f'
  on-tertiary-container: '#785313'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#c9e6ff'
  primary-fixed-dim: '#9accf3'
  on-primary-fixed: '#001e2f'
  on-primary-fixed-variant: '#0c4b6c'
  secondary-fixed: '#b2f2bb'
  secondary-fixed-dim: '#96d5a0'
  on-secondary-fixed: '#00210b'
  on-secondary-fixed-variant: '#145129'
  tertiary-fixed: '#ffddb2'
  tertiary-fixed-dim: '#f1be75'
  on-tertiary-fixed: '#291800'
  on-tertiary-fixed-variant: '#624000'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.6'
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '500'
    lineHeight: '1.2'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 20px
  lg: 32px
  xl: 48px
  container-padding: 20px
  gutter: 16px
---

## Brand & Style
The brand personality is efficient, friendly, and approachable, designed to transform the mundane task of receipt scanning into a delightful, stress-free experience. The design system leverages **Minimalism** with a subtle **Kawaii** influence—characterized by generous whitespace, soft rounded forms, and a gentle color palette. 

The target audience consists of everyday consumers and small business owners who value speed and clarity. The UI should evoke an emotional response of "calm productivity." Elements should feel light, almost floating, avoiding any industrial or "heavy" aesthetic. Any mascot or illustrative elements should follow a "squish" logic—plump, rounded, and endearing—to maintain the professional yet approachable balance.

## Colors
The palette is intentionally restrained to maintain a "crisp" and "airy" feel. 
- **Primary (#A5D8FF):** A soft Sky Blue used for primary actions, progress indicators, and key focus states.
- **Secondary (#B2F2BB):** A Mint Green used for success states, "Scan Complete" confirmations, and positive financial trends.
- **Neutral (#F8F9FA):** Used for large surface areas, background fills, and subtle grouping containers to differentiate from the pure white base.
- **Background (#FFFFFF):** The foundation of the UI, ensuring the PWA feels native and clean.
- **Text (#212529):** A deep charcoal (rather than pure black) to maintain readability while softening the contrast against the light background.

## Typography
**Inter** is selected for its exceptional legibility on mobile screens and its neutral, modern character that doesn't distract from content. 

- **Headlines:** Use tighter letter spacing and bold weights to create a strong hierarchy against the minimalist background.
- **Body:** Aim for generous line height (1.6) to enhance the "airy" feel and prevent text-heavy receipt data from feeling cluttered.
- **Labels:** Used for metadata (dates, categories), these utilize semi-bold weights at smaller sizes to remain legible.

## Layout & Spacing
The layout follows a **fluid grid** model tailored for PWA usage across mobile and desktop. 

- **Margins:** A consistent 20px (md) safe area on mobile devices.
- **Rhythm:** An 8px linear scale. Vertical spacing between card elements should be generous (20px to 32px) to emphasize the minimalist aesthetic.
- **Mobile First:** On mobile, components like the "Scan" button should be floating or anchored to the bottom using safe-area insets.
- **Desktop Reflow:** Content should center-align in a maximum 768px container to maintain the focused "utility app" feel.

## Elevation & Depth
Depth is created through **Ambient Shadows** and **Tonal Layers**. 

- **Surface Tiers:** The base layer is pure white (#FFFFFF). Cards and secondary sections sit on top using a very soft shadow (0px 4px 20px rgba(0,0,0,0.04)) or a subtle light grey background (#F8F9FA).
- **Shadow Character:** Shadows must be extremely diffused and low-opacity. Avoid hard edges. The goal is to make elements look like they are gently resting on a soft surface.
- **Interactive Depth:** On press/tap, buttons should not have a "down" state shadow, but rather a slight scale reduction (98%) to feel tactile and "squishy."

## Shapes
In line with the friendly/Kawaii aesthetic, shapes are highly rounded. 
- **Standard Radius:** 0.5rem (8px) for small inputs.
- **Large Radius (2xl/3xl):** 1rem (16px) to 1.5rem (24px) for cards, modals, and primary action buttons.
- **Full Radius:** Use pill-shaped (999px) for tags, chips, and the floating action button to reinforce the "soft" brand identity.

## Components
- **Buttons:** Primary buttons use a 1.5rem (24px) radius. They should be filled with the Primary Blue (#A5D8FF) with white text. No borders.
- **Cards:** Cards are the primary vessel for receipt data. They use a 1.5rem radius, white background, and the ambient shadow defined in Elevation.
- **Input Fields:** Use the Neutral Grey (#F8F9FA) as a fill with a 0.5rem radius. When focused, the border changes to Primary Blue with a soft glow.
- **Chips:** Small, pill-shaped elements for categorizing receipts (e.g., "Food," "Travel"). Use low-saturation background tints of the primary/secondary colors.
- **The "Snap" Button:** A large, circular floating action button (FAB) at the bottom center. It should be the most prominent element, potentially using a subtle gradient or a mascot icon.
- **Checkboxes/Radios:** Highly rounded corners (almost circular for checkboxes) to maintain the soft shape language.
- **Progress Bars:** Thick, rounded tracks with the Secondary Mint Green (#B2F2BB) indicating completion.
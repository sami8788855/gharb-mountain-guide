---
name: Jabal Al-Gharbi Service Portal
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
  on-surface-variant: '#434655'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#747686'
  outline-variant: '#c4c5d7'
  surface-tint: '#2151da'
  primary: '#0037b0'
  on-primary: '#ffffff'
  primary-container: '#1d4ed8'
  on-primary-container: '#cad3ff'
  inverse-primary: '#b7c4ff'
  secondary: '#7b5731'
  on-secondary: '#ffffff'
  secondary-container: '#ffce9f'
  on-secondary-container: '#795630'
  tertiary: '#005021'
  on-tertiary: '#ffffff'
  tertiary-container: '#006b2e'
  on-tertiary-container: '#65ef88'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dce1ff'
  primary-fixed-dim: '#b7c4ff'
  on-primary-fixed: '#001551'
  on-primary-fixed-variant: '#0039b5'
  secondary-fixed: '#ffdcbc'
  secondary-fixed-dim: '#edbe8f'
  on-secondary-fixed: '#2c1700'
  on-secondary-fixed-variant: '#60401c'
  tertiary-fixed: '#74fd94'
  tertiary-fixed-dim: '#55e07b'
  on-tertiary-fixed: '#002109'
  on-tertiary-fixed-variant: '#005322'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  headline-xl:
    fontFamily: IBM Plex Sans
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: IBM Plex Sans
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: IBM Plex Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: IBM Plex Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: IBM Plex Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-bold:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
  label-sm:
    fontFamily: IBM Plex Sans
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
  headline-lg-mobile:
    fontFamily: IBM Plex Sans
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  container-margin: 24px
  gutter: 16px
  card-padding: 20px
  section-gap: 48px
---

## Brand & Style

The brand personality is rooted in reliability, civic duty, and regional pride. It serves as a digital utility for the Nafusa Mountains community, prioritizing clarity and trust over aesthetic flair. The design style follows a **Corporate / Modern** approach with **High-Contrast** elements to ensure the platform remains usable in the bright, high-glare outdoor environments typical of the region.

The UI avoids decorative clutter, focusing instead on high-information density and immediate recognition. The emotional response should be one of "assured assistance"—knowing that the status of a fuel station in Nalut or an ATM in Gharyan is accurate and accessible at a glance.

## Colors

The palette is balanced between professional service and geographic identity.
- **Primary (Service Blue):** Used for navigation, primary actions, and institutional branding. It signifies the "Service" aspect of the platform.
- **Tertiary (Libyan Green):** Integrated as a secondary brand mark and for "Operational" status indicators, linking the service to the national identity.
- **Secondary (Mountain Earth):** A muted sand and stone palette used for backgrounds and subtle borders, grounding the digital tool in the physical landscape of the Nafusa range.
- **Status Colors:** These are high-chroma and strictly enforced for utility updates (e.g., fuel availability). Accessibility is prioritized with high contrast against the light neutral background.

## Typography

The design system utilizes **IBM Plex Sans** (with the Arabic companion) to ensure technical precision and high legibility across both Latin and Arabic scripts.

- **Headlines:** Set in bold weights to anchor the card-based layout.
- **Body:** Standardized for readability in long-form service descriptions or community news.
- **Status Labels:** High-weight, smaller font sizes are used for badges to maximize space while remaining readable at a glance on mobile devices.
- **Map Labels:** Use `label-sm` with a light halo effect for clarity against varied map backgrounds.

## Layout & Spacing

The layout follows a **Fluid Grid** model designed for mobile-first utility.
- **Desktop:** 12-column grid with 24px gutters. Content is typically housed in cards spanning 3 or 4 columns.
- **Mobile:** 4-column grid with 16px margins. Cards stack vertically to ensure large touch targets.
- **Spacing Rhythm:** Based on an 8px scale. Padding within service cards is generous (20px) to prevent visual crowding when multiple status icons are present.
- **Navigation:** A sticky top bar or bottom navigation (mobile) ensures the "Report" and "Search" functions are always within thumb's reach.

## Elevation & Depth

This design system uses **Tonal Layers** and **Low-Contrast Outlines** to define hierarchy. 

1.  **Level 0 (Background):** Solid Neutral (#F8F9FA) or a very light Sand tint.
2.  **Level 1 (Cards):** White background with a 1px border in a muted Stone tone (#E7E5E4). No shadow is used for Level 1 to maintain a clean, "tool-like" feel.
3.  **Level 2 (Active/Hover):** A subtle, diffused ambient shadow (10% opacity Primary Blue) to indicate interactable elements or filtered results.
4.  **Level 3 (Modals/Overlays):** Stronger elevation with a 15% opacity neutral shadow to pull critical information (like emergency alerts) to the foreground.

## Shapes

The shape language is **Soft (0.25rem)**. This provides a professional and modern look that is more approachable than sharp corners but avoids the "playful" connotations of fully rounded or pill-shaped designs. 

- **Primary Buttons:** Soft corners with consistent internal padding.
- **Service Cards:** `rounded-lg` (0.5rem) to create a distinct containerized feel for information.
- **Status Badges:** `rounded-xl` (0.75rem) to create a "capsule" look that differentiates metadata from main content.

## Components

- **Service Status Cards:** The core component. Includes a Service Icon (top left), Status Badge (top right), Location Title (headline-md), and "Last Updated" timestamp (label-sm).
- **Status Badges:** Color-coded based on the Status palette (Green = Working, Red = Out of Service, Yellow = Limited). Use high-contrast text (white on dark green/red/blue).
- **Primary Buttons:** Solid Primary Blue with white text. High-contrast for outdoor visibility.
- **Service Icons:** Linear, 24px icons with a 2px stroke. Use distinct metaphors for Fuel (Pump), Gas (Cylinder), ATM (Banknote), and Towing (Hook).
- **Input Fields:** Large tap targets (minimum 48px height) with 1px Stone borders that turn Primary Blue on focus.
- **Community Feed List:** Simple, horizontally-ruled list items for quick updates and news, utilizing `body-md` for content.
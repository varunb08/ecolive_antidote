# JalDOOT Website Design Specifications

## Overview
The JalDOOT website UI is built specifically around the context of water harvesting and ecological restoration in rural India. The design is modern but grounded, utilizing nature-inspired color palettes and a clean, accessible layout driven by Tailwind CSS.

## Typography
- **Headlines (`h1`, `h2`, `h3`)**: **Plus Jakarta Sans** (Weights: 400, 500, 600, 700, 800)
  - Used for large, bold, and modern headings that capture attention.
- **Body & Labels (`p`, `span`, `a`)**: **Be Vietnam Pro** (Weights: 300, 400, 500, 600)
  - Highly legible, modern sans-serif. Used for readable body copy and UI elements.

## Color Palette
The colors are derived from a Material You (M3) inspired theme:
- **Primary Base**: `#004f56` (Deep Teal / Water-inspired)
- **Secondary Base**: `#006e1c` (Forest Green / Flora-inspired)
- **Background**: `#f5fced` (Very light, warm green-tinted off-white)
- **Surface Enhancements**:
  - `primary-fixed`: `#a1eff9`
  - `liquid-gradient`: `linear-gradient(135deg, #004f56 0%, #006972 100%)`
  - `surface-container-low/highest`: Used to differentiate sections (e.g. `#eff6e7`, `#dee5d6`).

## Core Components
1. **Glassmorphism Navigation (`.glass-nav`)**
   - Translucent headers (`bg-[#f5fced]/70 backdrop-blur-xl`) with sleek bottom shadows, maintaining readability while scrolling over images.
2. **Bento Grid Layouts**
   - Used heavily for stats and impact sections where cards have heavily rounded corners (`rounded-[2.5rem]`).
3. **Pill-shaped Call to Actions (CTAs)**
   - Fully rounded buttons (`rounded-full`) that often incorporate the `.liquid-gradient` class or light/dark contrast inversions.
4. **Mobile Bottom Navigation**
   - Fixed to the bottom on mobile devices with high border-radius (`rounded-t-[2rem]`) containing icons and text labels.
5. **Contextual Floating Action Buttons (FAB)**
   - Rounded square/squircle items (`rounded-2xl`) sitting above the layout for primary actions like "Start a Project".

## Visual Assets & Icons
- Edge-to-edge nature and community-focused photography acting as subtle background textures with opacity/gradient overlays.
- Google Material Symbols utilized extensively (Filled and Outlined variants) for UI iconography like water drops, people, and community icons.

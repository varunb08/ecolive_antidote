# Design System Strategy: Organic Precision
(Project: ESG & Impact Dashboard Concept)

## 1. Overview & Creative North Star
The "Modern Eco-Corporate" aesthetic is not about adding a leaf icon to a corporate template. It is about **Organic Precision**. Our Creative North Star for this design system is **"The Living Document."**

We aim to bridge the gap between high-end editorial print (think *Monocle* or *Architectural Digest*) and cutting-edge digital interfaces. This system rejects the rigid, boxy constraints of traditional SaaS platforms. Instead, it utilizes intentional asymmetry, overlapping elements, and vast expanses of "breathing room" to create an experience that feels as much like an environmental sanctuary as it does a professional tool. We prioritize tonal depth over structural lines, creating a UI that feels grown, not just built.

---

## 2. Colors: The Tonal Ecosystem
This system moves away from flat color blocks. We treat color as light and atmosphere.

### The Palette
- **Primary Architecture:** `#00261b` (Primary) and `#0b3d2e` (Primary Container). These are our "Deep Forest" anchors, used for moments of absolute authority.
- **Vibrant Growth:** `#006e09` (Secondary) and `#97fa85` (Secondary Fixed). Use these to draw the eye to growth metrics and primary calls to action.
- **The Elements:** `#c2e8ff` (Tertiary Fixed/Sky Blue) for wellness and `#e0e3e1` (Surface Variant/Sand) for grounding organic elements.

### The "No-Line" Rule
**Explicit Instruction:** Designers are prohibited from using 1px solid borders to define sections. Boundaries must be defined through background color shifts. A `surface_container_low` section sitting on a `surface` background is the only way we define space. We do not "fence in" our content; we let it inhabit its own space.

### Surface Hierarchy & Nesting
Treat the UI as a series of physical layers.
- **Level 0 (Base):** `#f7faf8`
- **Level 1 (Sections):** `#f1f4f2`
- **Level 2 (Cards/Interaction):** `#ffffff`
By nesting a "lowest" white card inside a "low" grey-green section, we achieve a soft, natural lift that mimics sunlight hitting a surface.

### The "Glass & Gradient" Rule
To elevate the "Tech-Eco" feel, use **Glassmorphism** for floating headers or navigation. Use `#f7faf8` at 70% opacity with a `20px` backdrop blur. For primary CTAs, do not use flat colors; use a subtle linear gradient from `primary` to `primary_container` at a 135-degree angle to give the element "soul" and weight.

---

## 3. Typography: Editorial Authority
We use **Manrope** across the board. Its geometric foundation provides the "Corporate" stability, while its wide apertures and rounded terminals provide the "Eco" warmth.

- **Display & Headlines:** Use `display-lg` and `headline-lg` to create a sense of scale. Headlines should be "Heavy" or "Bold" and use tight tracking (-0.02em) to feel like a high-end masthead.
- **Body & Readability:** Body text (`body-lg`) must utilize generous leading. For a 1rem font size, we aim for a 1.7rem line height to ensure the "Happy" and "Approachable" feel is maintained even in data-heavy sections.
- **The Tonal Shift:** Headlines should utilize the `on_surface` color, while secondary labels use `on_surface_variant`. This contrast creates hierarchy without the need for varying font weights.

---

## 4. Elevation & Depth: Tonal Layering
We do not use shadows to create "pop." We use them to create "atmosphere."

- **The Layering Principle:** Depth is achieved by stacking `surface-container` tiers. If a card needs to feel interactive, transition its state from `#ffffff` to `#f7faf8` on hover.
- **Ambient Shadows:** When a "floating" effect is required (e.g., a modal), shadows must be extra-diffused. Use a blur of 40px and a 4% opacity. The shadow color must be a tinted version of `on_surface` (a very dark green-grey, `#181c1b`) to mimic natural light filtered through a forest canopy.
- **The "Ghost Border" Fallback:** If accessibility requires a stroke (e.g., in a high-contrast mode or specific input field), use `#c0c8c3` (outline_variant) at 20% opacity. 100% opaque borders are forbidden.

---

## 5. Components: Refined Primitives

### Buttons
- **Primary:** Full rounded (`rounded-full`). Gradient of `#00261b` to `#0b3d2e`. Typography in `#ffffff`.
- **Secondary:** Transparent background with a "Ghost Border" (`#c0c8c3` at 20%). On hover, fill with `#e6e9e7`.
- **Tertiary:** No border, no background. Use `#006e09` for text to signal a "Growth" action.

### Cards & Layouts
- **Constraint:** Forbid the use of divider lines. 
- **Method:** Use `spacing.8` (2.75rem) to separate content chunks. Use `#ffffff` for the card body. 
- **Imagery:** Cards should often feature "Bleed Imagery"—high-quality nature photography that hits the top and side edges of the card, transitioning into the content via a subtle white fade.

### Data Visualization
- **Eco-Charts:** Use `#006e09` for growth and `#c2e8ff` for baseline/water metrics. 
- **Rounded Data:** All bar charts and progress indicators must use `rounded-full` caps. Sharp 90-degree corners do not exist in this system.

### Inputs & Fields
- **Style:** Subtle glassmorphism. Use `#f1f4f2` with a 1px `ghost border`. 
- **Focus State:** Transition the border to `#006e09` (Vibrant Leaf Green) to symbolize an "active/living" state.

---

## 6. Do’s and Don’ts

### Do:
- **Use Asymmetry:** Place a large `display-lg` headline on the left with a small `body-md` paragraph offset to the right. 
- **Embrace White Space:** If a section feels "crowded," double the padding. This is a premium experience; we are not afraid of empty space.
- **Use Macro Photography:** Use high-resolution, close-up textures of leaves, water ripples, or sand to fill large background areas at low opacity.

### Don't:
- **Don't use 1px dividers.** Use color shifts or white space.
- **Don't use standard Grey shadows.** Always tint shadows with a hint of forest green (#181c1b).
- **Don't use "Default" Inter/Roboto styles.** Ensure the Manrope letter-spacing and line-heights are strictly followed to maintain the editorial feel.
- **Don't use sharp corners.** Every element must have at least `rounded-DEFAULT` (0.5rem) to maintain the "Happy" organizational personality.

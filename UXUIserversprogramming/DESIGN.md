```markdown
# Design System Document: High-Tech Cyber-Editorial

## 1. Overview & Creative North Star
**Creative North Star: "The Kinetic Monolith"**

This design system moves beyond the "standard dark mode" template. We are building an interface that feels like a living, breathing piece of high-performance hardware. By leveraging **Space Grotesk’s** geometric quirks alongside a high-energy Neon Green palette, we create a "Kinetic Monolith"—an experience that is structurally rigid and brutalist, yet vibrating with digital energy.

To achieve a signature high-end feel, we move away from traditional "boxed" layouts. We utilize **intentional asymmetry**, massive typography scales, and tonal layering to create depth. The interface shouldn't feel like a website; it should feel like a tactical heads-up display (HUD) for an advanced financial or synthetic ecosystem.

---

## 2. Colors & Surface Architecture

The palette is anchored in deep obsidian greens and energized by a "Radioactive" Neon Primary. 

### The "No-Line" Rule
**Borders are a design failure.** We prohibit the use of 1px solid borders for sectioning or containment. Boundaries must be defined through:
*   **Background Shifts:** Using `surface-container-low` against a `surface` background.
*   **Tonal Transitions:** Defining edges through subtle contrast rather than lines.
*   **Negative Space:** Using the typography grid to create invisible boundaries.

### Surface Hierarchy & Nesting
Treat the UI as a series of physical layers. We use the Material surface tiers to "carve" into the dark background:
*   **Base Layer:** `surface` (#001204) — The infinite void.
*   **Sectional Layer:** `surface-container-low` (#001806) — Sub-regions of the screen.
*   **Active Layer:** `surface-container-high` (#00260c) — Interaction zones and modals.
*   **Floating Layer:** `surface-container-highest` (#002d0f) — The "Glass" layer.

### The "Glass & Gradient" Rule
To inject "soul" into the futuristic aesthetic, use **Glassmorphism**. Floating cards should utilize semi-transparent `surface-variant` colors with a `backdrop-filter: blur(20px)`. 
*   **Signature Texture:** For primary CTAs or high-impact headers, use a linear gradient: `primary` (#8eff71) to `primary-container` (#2ff801) at a 135-degree angle. This provides a "liquid light" effect.

---

## 3. Typography: Geometric Brutalism

We use **Space Grotesk** exclusively. Its monospaced-adjacent feel provides the "high-tech" look without sacrificing legibility.

*   **Display (Display-LG 3.5rem):** Use for hero moments and data-heavy "Statement" numbers. Tracking should be set to -0.02em for a tighter, more aggressive stance.
*   **Headline (Headline-LG 2rem):** Used for section titles. Implement **Intentional Asymmetry**: try left-aligning headlines while right-aligning the corresponding body text to create a dynamic, editorial flow.
*   **Body (Body-LG 1rem):** High readability for technical documentation. Use `on-surface-variant` (#8cb58f) for secondary body text to reduce eye strain.
*   **Labels (Label-MD 0.75rem):** Always uppercase with +0.05em letter spacing. This mimics technical blueprints.

---

## 4. Elevation & Depth: Tonal Layering

Traditional drop shadows are forbidden. We achieve lift through **The Layering Principle**.

*   **Ambient Shadows:** When an element must float (e.g., a modal), use a diffused glow rather than a shadow. The shadow color should be a tinted `primary` (opacity 4%) with a blur value of 40px+. This mimics the neon light reflecting off a dark surface.
*   **The "Ghost Border" Fallback:** If accessibility requires a stroke, use a "Ghost Border": `outline-variant` (#2b5031) at **15% opacity**. It should be felt, not seen.
*   **Interactive Depth:** On hover, a container should not just change color; it should "ascend" from `surface-container-low` to `surface-container-high`, creating a tactile sense of movement.

---

## 5. Components

### Buttons: The Power Cells
*   **Primary:** High-energy. Background: `primary` (#8eff71). Text: `on-primary` (#0d6100). No border. On hover, apply a `box-shadow` glow using the `primary` color at 20% opacity.
*   **Secondary:** The "Outlined" feel. Background: transparent. Border: Ghost Border (20% `primary`). Text: `primary`.
*   **Tertiary:** Text-only. `label-md` styling. 

### Cards & Lists: The "Invisible Grid"
*   **Forbid Dividers:** Do not use lines to separate list items. Use a 12px vertical gap and a subtle background shift (`surface-container-lowest`) on hover to define the row.
*   **Card Styling:** Use `md` (0.375rem) corner radius. Large radius values feel too "soft" for a high-tech system; sharper corners feel faster and more precise.

### Input Fields: Tactical Entry
*   **Default State:** Background: `surface-container-highest`. No border. Bottom-only accent line using `outline-variant`.
*   **Focus State:** The bottom accent line transforms into a 2px `primary` glow. The label should shift to `primary` color.

### Custom Component: The "Data Pulse"
*   For status indicators or live data feeds, use a small 4px circle of `primary` with a CSS "ripple" animation to signify a living connection.

---

## 6. Do's and Don'ts

### Do:
*   **Embrace the Dark:** Allow large areas of the screen to remain `surface` (#001204). High-end design thrives on "the luxury of space."
*   **Use Neon Spreads:** Use the `primary` color sparingly but powerfully. A single Neon Green button on a deep black screen is more energetic than a screen full of green.
*   **Monospace Numbers:** Ensure all numerical data uses tabular lining to maintain the "High-Tech" alignment.

### Don't:
*   **Don't use Pure White:** Use `on-surface` (#d1fcd2) for text. Pure #FFFFFF is too jarring against the dark green-black background and feels "default."
*   **Don't use 1px Gray Lines:** This is the quickest way to make a high-end system look like a generic dashboard. Use color shifts instead.
*   **Don't Round Everything:** Avoid the `full` (pill) radius for anything other than chips. Over-rounding makes the system feel "bubbly" rather than "futuristic." Use `sm` or `md` for a technical edge.

---
**Director's Note:**
Remember, we are designing for speed and precision. Every pixel of the Neon Green primary should feel like it's providing power to the interface. Keep the layouts breathable, the type bold, and the surfaces deep.```
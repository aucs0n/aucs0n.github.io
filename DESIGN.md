```markdown
# Design System Document: The Eternal Hero Aesthetic

## 1. Overview & Creative North Star
The **Creative North Star** for this design system is **"The Nostalgic Monolith."** 

This system is designed to evoke the feeling of a cherished memory—heroic yet humble, grand yet intimate. We are moving away from the rigid, boxy constraints of traditional SaaS UI and toward a "High-End Editorial" experience. The layout should feel like a curated gallery or a beautifully typeset memoir. We achieve this through intentional asymmetry, generous whitespace (breathing room), and "Ethereal Layering" where elements feel as though they are floating in a soft, morning mist.

### The Editorial Shift
*   **Asymmetry:** Avoid perfectly centered grids. Offset text blocks against large, evocative imagery.
*   **The Hero’s Path:** Use "Blue Rose" filigree motifs as subtle directional cues, guiding the eye through the narrative flow of the page.
*   **Atmosphere over Structure:** Focus on the "vibe" of selfless heroism—clean, bright, and hopeful.

---

## 2. Colors & Tonal Depth
The palette is a study in atmospheric blues and warm, human accents. It prioritizes light-mode clarity with a romantic, nostalgic undertone.

### Surface Hierarchy & Nesting
To achieve a premium look, we prohibit the use of 1px solid borders for sectioning. 
*   **The "No-Line" Rule:** Boundaries are defined by shifting between `surface` (#F1FBFF), `surface-container-low` (#E2F7FF), and `surface-container-highest` (#C5E8F5).
*   **Layering:** Treat the UI as stacked sheets of fine parchment. A card (`surface-container-lowest` / #FFFFFF) should sit atop a `surface-container-low` section to create a natural, soft lift.

### Signature Textures & Glassmorphism
*   **The "Glass & Gradient" Rule:** Floating navigation or modal elements must use Glassmorphism. Utilize `surface` colors at 70% opacity with a `24px` backdrop-blur to allow the "Sky High Blue" (#A1C6EA) backgrounds to bleed through softly.
*   **Heroic Gradients:** For primary CTAs or Hero sections, use a subtle linear gradient from `primary_container` (#A1C6EA) to `primary` (#3D6281) at a 135-degree angle. This adds "soul" and depth that flat hex codes cannot provide.

---

## 3. Typography
The typography is the voice of the system: a dialogue between the legendary past and the clear-eyed present.

*   **Display & Headlines (Noto Serif):** These are your "Nostalgic" anchors. Use `display-lg` for moments of high emotional impact. The serif should feel authoritative but elegant, like an inscription on a hero's monument.
*   **Body & UI (Plus Jakarta Sans):** This provides the "Airy" modern balance. It ensures that even within a romantic aesthetic, the functional data remains highly readable and professional.
*   **Visual Hierarchy:** Pair a `headline-lg` (Serif) with a `title-sm` (Sans-Serif) in `secondary` (#406279) for a sophisticated, editorial sub-header look.

---

## 4. Elevation & Depth
In this system, depth is organic, not mechanical.

*   **The Layering Principle:** Depth is achieved by "stacking" the surface-container tiers. Never use a shadow where a color shift can work.
*   **Ambient Shadows:** If an element must float (like a FAB or a Hover Card), use an extra-diffused shadow: `box-shadow: 0 12px 40px rgba(85, 122, 149, 0.08);`. Note the use of `smoke-blue` for the shadow tint rather than pure black—this mimics natural light passing through a blue sky.
*   **The "Ghost Border" Fallback:** If a container requires a boundary for accessibility, use `outline_variant` at 15% opacity. It should be felt, not seen.

---

## 5. Components
All components follow the `ROUND_EIGHT` (0.5rem) corner radius for a soft, approachable feel.

*   **Buttons:** 
    *   *Primary:* Gradient fill (A1C6EA to 7395AE) with `on_primary` text. No border.
    *   *Tertiary:* `Warm Beige` (#F1E3D3) text with a 0px background. Use for "Low-Priority" or "Selfless" actions.
*   **Cards:** Forbid divider lines. Use `surface_container_low` for the card body and `surface_container_highest` for the header area to create separation.
*   **Chips:** Pill-shaped (`full` roundness). Use `tertiary_fixed` (#EEE0D0) for a subtle "cloak-accent" feel that stands out against the blue-heavy UI.
*   **Input Fields:** Ghost-style inputs. Use a `surface_variant` background with a `primary` bottom-only focus stroke (2px).
*   **Filigree Dividers:** Instead of horizontal rules (`<hr>`), use a centered, low-opacity "Blue Rose" or filigree vector to separate major content sections.

---

## 6. Do’s and Don’ts

### Do:
*   **Do** use `Warm Beige` (#F1E3D3) sparingly as a "human" accent—it represents the hero's cloak and adds warmth to the cold blues.
*   **Do** embrace negative space. If a layout feels "full," remove elements until only the "Hero" content remains.
*   **Do** use Noto Serif for any text that is meant to be read with "emotion."

### Don’t:
*   **Don’t** use pure black (#000000) for text. Use `on_surface` (#001F27) to maintain the deep-sea/sky tonal consistency.
*   **Don’t** use hard shadows or 1px borders. They shatter the "ethereal" illusion of the system.
*   **Don’t** crowd components. Each element should feel like a statue in a park—given its own dedicated space to be admired.

---

## 7. Signature Motif: The Blue Rose Effect
To truly capture the inspiration, incorporate a "Light Leak" or "Ethereal Glow" on large landing pages. This is a large, soft radial gradient of `primary_container` (#A1C6EA) at 20% opacity, positioned in the top-right corner of the viewport, simulating sunlight filtering through a blue sky. This is the final touch in creating a UI that feels less like a tool and more like a journey.```
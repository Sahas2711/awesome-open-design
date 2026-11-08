---
name: cafe-menu
en_name: "Café Menu"
description: "A café menu rendered as an A4 printed menu (210 × 297 mm) and an Instagram Story canvas (1080 × 1920 px), sharing one warm brown-and-cream visual identity. Suitable for small businesses wanting a print-ready menu plus a social story from one design."
en_description: "A café menu rendered as an A4 printed menu (210 × 297 mm) and an Instagram Story canvas (1080 × 1920 px), sharing one warm brown-and-cream visual identity. Suitable for small businesses wanting a print-ready menu plus a social story from one design."
category: hospitality
tags: ["café", "menu", "food", "hospitality", "print", "social-media"]
od:
  mode: prototype
  surface: web
  preview:
    type: html
    entry: example.html
  design_system:
    requires: false
  example_prompt: "Make me a café menu with an A4 printed version and an Instagram Story version. Include the café name, address and opening hours, a drink menu, a breakfast menu and a dessert menu, with sample prices."
---

# Café Menu

A café menu example showing an A4 printed menu and an Instagram Story in one file, with a shared warm brown-and-cream visual identity.

## Files

- `example.html`: the A4 printed menu (210 × 297 mm) followed by an Instagram Story canvas (1080 × 1920 px), sharing colors, type and spacing.
- `open-design.json`: the starter prompt for reproducing the design.

## Reproducing with the Open Design kit

Open Design does not ship a dedicated "menu" recipe, so reproduce this with the poster workflow (`/open-design-poster`), which handles print sizes with bleed and exports PNG/PDF:

1. **Ask.** In Copilot Chat, run `/open-design-poster` with a brief such as:
   > An A4 café menu with breakfast, lunch and drinks sections, sample prices, and an Instagram Story version, warm brown and cream palette, serif headings.
2. **The kit asks about size.** Choose print (A4, 210 × 297 mm) for the menu and screen (1080 × 1920 px) for the story; the agent sets bleed and safe area for print.
3. **The kit writes the files** under `.open-design/<name>/` and registers them as an artifact.
4. **Check and export.** `check_open_design_artifact` renders the design; the agent fixes clipped text or contrast. `export_open_design_artifact` writes the A4 print PDF/PNG and the story image.

## Output formats

- **A4 Menu:** 210 × 297 mm portrait, print-ready with margins, exported as PDF or PNG.
- **Instagram Story:** 1080 × 1920 px vertical canvas, exported as PNG.

## Notes

- Prices and menu items in `example.html` are illustrative **sample prices** and are labeled as such; they are not real café pricing.
- Where your café has real values (name, address, hours, prices, menu items), replace the sample text before printing. Never present invented prices as real.

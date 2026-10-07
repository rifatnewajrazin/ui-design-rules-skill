---
name: ui-design-rules
description: Rules for building web and app interfaces: 4px spacing scale, Material Design 3 tokens, button hierarchy and placement, icon sizing and naming, Open Graph image specs, and a pre-delivery QA checklist. Use when generating or reviewing HTML, CSS, React, Vue, Svelte or Tailwind UI, or when asked for a layout, a component or a link preview image.
---

# UI Design Rules

Apply these whenever you build or review an interface. Load the reference file for the area you are working in.

## Core rules

1. **Spacing.** Every margin, padding, gap and size is a multiple of 4px. No `7px`, `11px`, `13px`. Define tokens once and use them. See `references/spacing-4pt.md`. If the project uses Material Design 3, use its 8dp system instead: `references/spacing-material-3.md`.
2. **Proximity.** Related things sit closer than unrelated things. A label is nearer to its input than to the next field.
3. **Buttons.** One primary button per screen. Buttons do things, links go places. Labels say what happens. See `references/buttons.md`.
4. **Touch targets.** At least 44 by 44 px, 48 by 48 where possible, even if the visible icon is smaller.
5. **Icons.** One library, one or two sizes, sized to the text line height, named by the object, inherit colour. See `references/icons.md`.
6. **Contrast.** Text meets WCAG AA, 4.5 to 1.
7. **Consistency.** No page-specific component variants. Change the system, not one screen.
8. **Share images.** 1200 by 630, everything important inside the centre 630 by 630, under 300 KB. See `references/og-images.md`.

## How to work

- Only change what was asked. If you see something else worth fixing, list it and ask.
- Do not add visual elements nobody requested.
- Before saying a UI change is done, run `references/qa-checklist.md` and show full-size screenshots at desktop width and phone width.
- Optical adjustments are allowed when the maths looks wrong to the eye (a play icon, a rounded badge). Say so when you do it.
- If a rule conflicts with the project's existing design system, follow the design system and mention the conflict.

## When in doubt

Pick the more conservative option, keep the spacing on the grid, and ask.

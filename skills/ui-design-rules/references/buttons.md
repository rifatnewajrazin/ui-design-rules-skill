# Buttons

## Look and hierarchy

- A button must look clickable: a fill or a clear border, real padding, rounded corners, and visible hover, focus and active states.
- **Primary:** the one main action ("Save changes"). Strongest colour. Only one per screen. Two competing primaries make people stall.
- **Secondary:** outline or neutral fill ("Cancel", "Back").
- **Tertiary:** a plain text link or an icon with no border.
- **Buttons act, links navigate.** Submitting, saving, opening a dialog: button. Going to another page or section: link.

## Placement

- Put the main action where the task ends: bottom right of a dialog, the end of a form, the last step of a flow.
- Keep a button close to the thing it controls. Do not leave it floating in a far corner.
- On phones and long forms, a sticky bottom button helps. Make sure it does not cover content.

## Words

- One to three words. Start with a verb: "Create file", "Save draft", "Download report".
- Say what will happen. Avoid "Submit", "OK" and "Click here".
- Match the moment on screen, not a goal three steps away.
- Destructive actions name the outcome: "Delete account", not "Confirm". For serious deletes, ask for typed confirmation or offer an undo.
- Use the user's words, not internal jargon.

## Size and spacing

- Touch area at least 44 by 44 px.
- Padding about 12 to 16 px sideways and 8 to 12 px vertically.
- At least 8 to 12 px between neighbouring buttons.

## Colour

| Role | Colour guidance |
| --- | --- |
| Primary | Main brand colour, high contrast |
| Secondary | Neutral grey, slate or outline |
| Destructive | A clear red |
| Disabled | Muted grey, lower opacity, `cursor: not-allowed` |

Text on a button meets WCAG AA (4.5 to 1) in every state.

## Details that help

- **Glow on dark backgrounds.** Take the glow colour from the button's own fill, not plain white. Keep it close and soft, around 22 to 26 px blur at 35 to 45 percent opacity, so it looks like the button is giving off light and not like a game menu.
- **Corner radius.** 6px is a good default. Sharp corners feel like a spreadsheet. Full pills feel like a consumer app. Change it only if the brand calls for it.
- **One spec.** Same radius, font, weight, padding and elevation on every screen. Do not invent a special button for one page. Update the system instead.

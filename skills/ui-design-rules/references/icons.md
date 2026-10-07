# Icons

## Library

- Choose one library at the start, with enough icons and a few weights (regular, bold, duotone).
- Match the product's personality: soft and rounded for playful apps, thin geometric strokes for sleek professional tools.
- Do not draw your own icons or bend the geometry of a standard one.
- Good options: Phosphor, Iconoir, Google Material Symbols.

## Size

- Use one or two sizes across the whole app, for example 20 and 24 px.
- Keep sizes on the 4px grid: 16, 20, 24, 28, 32.
- Size the icon to the text line height. 14px text with 20px line height gets a 20px icon. 16px text with 24px line height gets a 24px icon. Then a button or list row keeps the same height whether the icon is there, hidden or swapped.

## Hit area

A 20 or 24 px icon is too small to tap. Wrap it in an invisible area of at least 44 by 44, ideally 48 by 48.

## Naming

Name icons for what they are, not what they do.

| Avoid | Prefer |
| --- | --- |
| `Icon/Settings` | `Icon/Gear` |
| `Icon/Help` | `Icon/QuestionMark` |
| `Icon/Search` | `Icon/MagnifyingGlass` |

An object name can be reused for a tooltip, a button or a nav item without a meaning clash. In design files, keep the layer structure identical (`icon-name` then `vector`) so colour overrides survive when you swap an icon.

## Code

- Use optimised SVG. Never PNG or JPG for interface icons.
- Use `fill: currentColor` or `stroke: currentColor` so the icon follows the text colour, including hover and theme changes.
- Decorative icon next to text: `aria-hidden="true"`.
- Icon-only button: give it an `aria-label` that describes the action.

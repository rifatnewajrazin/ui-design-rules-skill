# 4-Point Spacing

Base unit: 4px. Every spacing value and element size is a multiple of it.

## Scale

| Token | Value | Typical use |
| --- | --- | --- |
| `--space-1` | 4px | Icon-to-text gap, badge padding |
| `--space-2` | 8px | Compact padding, button vertical padding |
| `--space-3` | 12px | Dense card padding, input vertical padding |
| `--space-4` | 16px | Standard container padding, form gaps, button horizontal padding |
| `--space-6` | 24px | Roomy card padding, section gaps |
| `--space-8` | 32px | Large margins, grid gaps |
| `--space-12` | 48px | Major section breaks |
| `--space-16` | 64px | Page-level margins |
| `--space-24` | 96px | Hero padding on desktop |

The scale skips some numbers on purpose. Fewer choices means more consistency.

## Micro and macro

- **Micro spacing** is inside a component: button padding, input padding, icon gaps. Use 4, 8, 12, 16.
- **Macro spacing** is between components and regions: card gaps, section breaks, page padding. Use 24, 32, 48, 64, 96.

## Why it works

- **Proximity.** People read things that sit close together as a group. The gap between a label and its field (4 or 8) should be smaller than the gap between two form groups (16 or 24).
- **Rhythm.** Repeated steps feel orderly and make a page easy to scan.
- **Sharp rendering.** Multiples of 4 land on whole pixels at 1x, 2x and 3x screens, so edges stay crisp.
- **Optical exception.** If a shape looks off despite correct maths, adjust by eye by a pixel or two.

## In code

```css
:root {
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-6: 24px;
  --space-8: 32px;
  --space-12: 48px;
  --space-16: 64px;
  --space-24: 96px;
}
```

- Tailwind already uses a 4px scale: `p-1` is 4px, `p-2` is 8px, `p-4` is 16px. Do not write arbitrary values like `p-[13px]`.
- Line heights and fixed heights are multiples of 4 as well.

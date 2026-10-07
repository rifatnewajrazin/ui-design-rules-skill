# Material Design 3 Spacing

Use this when a project follows Material Design 3. The baseline is 8dp, with 2dp and 4dp steps for small parts.

## Tokens

| Token | Value | Use |
| --- | --- | --- |
| `space000` | 0 | Flush |
| `space025` | 2 | Hairline offsets |
| `space050` | 4 | Icon-to-text gap |
| `space075` | 6 | Chip vertical padding |
| `space100` | 8 | Baseline gap, button padding |
| `space150` | 12 | Input vertical padding, dense cards |
| `space200` | 16 | Container padding, list gaps, phone page margin |
| `space300` | 24 | Card padding, tablet gutters |
| `space400` | 32 | Sub-section breaks, desktop margins |
| `space500` | 40 | Header margins |
| `space600` | 48 | Major sections, hero padding |
| `space700` | 56 | Navigation rail width |
| `space800` | 64 | Large layout gaps |

Full token names look like `md.sys.spacing.space100`.

## Window sizes

| Class | Width | Margin | Gutter |
| --- | --- | --- | --- |
| Compact (phone) | under 600 | 16 | 16 |
| Medium (tablet) | 600 to 840 | 24 | 24 |
| Expanded (desktop) | 840 to 1200 | 24 to 32 | 24 |
| Extra large | over 1200 | 32 to 48 | 32 |

## Naming and direction

- System tokens (`md.sys.*`) are global choices. Component tokens (`md.comp.*`) point at system tokens, so a theme change flows through.
- Use `leading` and `trailing` instead of left and right. In CSS, prefer `padding-inline-start` and `padding-inline-end` so right-to-left languages work without extra code.

## Touch targets

Every tappable thing is at least 48 by 48dp, whatever its visible size.

## In code

```css
:root {
  --md-sys-spacing-space050: 4px;
  --md-sys-spacing-space100: 8px;
  --md-sys-spacing-space150: 12px;
  --md-sys-spacing-space200: 16px;
  --md-sys-spacing-space300: 24px;
  --md-sys-spacing-space400: 32px;
  --md-sys-spacing-space600: 48px;
}

.button {
  padding-inline: var(--md-sys-spacing-space200);
  padding-block: var(--md-sys-spacing-space100);
  gap: var(--md-sys-spacing-space100);
  min-height: var(--md-sys-spacing-space600);
}
```

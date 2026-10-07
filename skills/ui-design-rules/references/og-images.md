# Social Share Images (Open Graph)

The picture that shows up when someone shares your link in a chat or on a social site.

## Specs

| Item | Rule |
| --- | --- |
| Canvas | 1200 x 630 px (ratio 1.91 to 1) |
| Safe zone | Logo, product graphic and all text inside the centre 630 x 630 square (x from 285 to 915) |
| Why | Chat apps such as WhatsApp and Messenger crop to a square thumbnail. Anything outside the centre gets cut. |
| File size | Under 300 KB, or some apps fail to fetch the preview |
| Format | WebP (preferred) or progressive JPEG, sRGB, 72 DPI |
| File name | Lowercase, hyphenated, descriptive |

## File name pattern

`brand-core-product-role-country.webp`

Example: `acme-industrial-valves-manufacturer-bangladesh.webp`

## Workflow

1. Leave a clear space in the middle for the logo.
2. Let background and atmosphere run into the outer 285 px on each side, but put nothing important there.
3. Resize to exactly 1200 x 630, compress under 300 KB, rename.
4. Add the tags:

```html
<meta property="og:image" content="https://example.com/og/acme-industrial-valves-manufacturer-bangladesh.webp">
<meta property="og:image:width" content="1200">
<meta property="og:image:height" content="630">
<meta name="twitter:card" content="summary_large_image">
```

5. Test the link in a real chat app, not only a preview tool.

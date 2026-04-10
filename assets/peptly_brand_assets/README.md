# peptly — brand asset files

Logo files for the peptly brand. All files are production-ready.

## Vector files (SVG)

These are the master files. SVG scales infinitely without losing quality. Use these whenever possible — for the website, social media headers, print materials, and as the source for any future format conversion.

| File | Use |
|---|---|
| `peptly_wordmark.svg` | Primary wordmark in deep forest (#1F3A2E). Use on light backgrounds. This is your default logo. |
| `peptly_wordmark_bone.svg` | Wordmark in bone (#F5F1EA). Use on dark or photographic backgrounds. |
| `peptly_icon.svg` | Icon mark — lowercase "p" in bone on a deep forest rounded square. Use for favicons, social profile pictures, and app icons. |

The text in these files has been converted to outlined paths, which means the files are fully self-contained and don't depend on the Inter font being installed on the viewer's machine. This is the correct way to ship logo files.

## PNG exports (raster)

Use these only when SVG isn't supported (some email clients, older systems, certain social media uploads).

### Wordmark PNGs

| File | Width | Use |
|---|---|---|
| `peptly_wordmark_400.png` | 400px | Email signatures, small web use |
| `peptly_wordmark_800.png` | 800px | Standard web use, blog headers |
| `peptly_wordmark_1600.png` | 1600px | High-resolution, retina displays, print |
| `peptly_wordmark_bone_800.png` | 800px | Wordmark on dark backgrounds |

### Icon PNGs

| File | Size | Use |
|---|---|---|
| `peptly_icon_16.png` | 16x16 | Browser tab favicon (standard) |
| `peptly_icon_32.png` | 32x32 | Browser tab favicon (retina) |
| `peptly_icon_64.png` | 64x64 | Small UI elements |
| `peptly_icon_192.png` | 192x192 | Android home screen, web app manifest |
| `peptly_icon_512.png` | 512x512 | PWA icon, social profile pictures (Instagram, X, TikTok, YouTube), app stores |
| `peptly_icon_1024.png` | 1024x1024 | iOS app icon, high-resolution master |

### Favicon

| File | Use |
|---|---|
| `favicon.ico` | Multi-resolution ICO file containing 16x16, 32x32, and 48x48 versions. Drop this in your website root directory. Browsers will automatically detect it. |

## Brand colors (reference)

| Color | Hex | Use |
|---|---|---|
| Deep forest | `#1F3A2E` | Primary brand color, wordmark on light backgrounds |
| Bone | `#F5F1EA` | Primary background color, wordmark on dark backgrounds |
| Ink | `#1A1A1A` | Body text |
| Copper | `#B8743E` | Accent (use sparingly) |
| Mist | `#D4D9D2` | Secondary text, borders, dividers |

## Quick implementation guide

**Website favicon:** Upload `favicon.ico` to your website root directory (e.g., `peptly.org/favicon.ico`). Most platforms (Shopify, Webflow, WordPress) have a favicon upload field — use the .ico file there. For modern setups, also add this to your HTML head:

```html
<link rel="icon" type="image/svg+xml" href="/peptly_icon.svg">
<link rel="icon" type="image/png" sizes="32x32" href="/peptly_icon_32.png">
<link rel="icon" type="image/png" sizes="192x192" href="/peptly_icon_192.png">
<link rel="apple-touch-icon" sizes="180x180" href="/peptly_icon_192.png">
```

**Shopify logo upload:** Upload `peptly_wordmark_800.png` in your theme's logo settings. Shopify will scale it appropriately.

**Instagram/TikTok/X/YouTube profile picture:** Upload `peptly_icon_512.png`. The icon mark is designed for circular crops — the rounded square will be visible in feed contexts and the centered "p" will read clearly when cropped to a circle.

**Email signature:** Use `peptly_wordmark_400.png`. Most email clients render PNG reliably; SVG support is inconsistent.

**Print materials (business cards, packaging):** Always use the SVG files. Send `peptly_wordmark.svg` to any designer or printer — they'll know what to do with it.

## Logo usage rules

These rules come from your brand style guide. Do not break them.

- **Never modify the wordmark.** Don't stretch, recolor, rotate, add effects, or change letter spacing. Use the files as-is.
- **Always lowercase.** The wordmark is "peptly" — never PEPTLY, never Peptly, never PEPTly.
- **Maintain clear space.** Leave space around the wordmark equal to the height of the letter "p" — no other text, logos, or graphics should encroach.
- **Minimum size.** Don't use the wordmark smaller than 80 pixels wide on screen or 0.75 inches in print. Below that, use the icon mark instead.
- **Contrast.** Use the deep forest version on light/bone backgrounds. Use the bone version on dark/forest backgrounds. Never use the deep forest version on a dark background or the bone version on a light background.

## Need to make changes?

These files are final and shouldn't be edited. If you need a variant that doesn't exist (different color, different layout, with tagline added), commission a designer on Fiverr and send them the SVG files as the source of truth. The files are clean, well-structured, and ready to be the foundation for any extended brand work.

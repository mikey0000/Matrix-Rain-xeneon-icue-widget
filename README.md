# Matrix Rain — iCUE Widget

Animated Matrix digital rain for CORSAIR LCD screens. Supports all Xeneon Edge sizes, Pump LCD, and Keyboard LCD.

## Supported Devices

| Device | Resolution |
|--------|------------|
| Xeneon Edge (S horizontal) | 840×344 |
| Xeneon Edge (S vertical) | 696×416 |
| Xeneon Edge (M horizontal) | 840×696 |
| Xeneon Edge (M vertical) | 696×840 |
| Xeneon Edge (L horizontal) | 1688×696 |
| Xeneon Edge (L vertical) | 696×1688 |
| Xeneon Edge (XL horizontal) | 2536×696 |
| Xeneon Edge (XL vertical) | 696×2536 |
| Pump LCD | 480×480 |
| Keyboard LCD | 320×170 |

## Installation

[![Download latest release](https://img.shields.io/github/v/release/mikey0000/Matrix-Rain-xeneon-icue-widget?label=Download&style=for-the-badge)](https://github.com/mikey0000/Matrix-Rain-xeneon-icue-widget/releases/latest)

Download the `.icuewidget` file from the [latest release](https://github.com/mikey0000/Matrix-Rain-xeneon-icue-widget/releases/latest), then double-click it to install or drag it into the iCUE widget panel.

## Configuration

### Matrix Rain

| Property | Type | Description | Default |
|----------|------|-------------|---------|
| Character Set | Dropdown | The character set used for the rain: **Katakana**, **Latin**, **Binary**, or **Mix** | Katakana |
| Fall Speed | Slider 1–10 | How fast the columns fall. Higher = faster. | 5 |
| Column Density | Slider 1–10 | Controls how quickly columns restart after reaching the bottom. Higher = more active columns at once. | 5 |
| Font Size | Slider 8–28 px | Size of each character in pixels. Smaller values produce more columns. | 14 px |
| Tail Length | Slider 3–40 | Number of characters in each column's trail. | 15 |

### Widget Personalization

| Property | Type | Description | Default |
|----------|------|-------------|---------|
| Text Color | Color | Color of the trail characters. | `#00ff41` (Matrix green) |
| Accent Color | Color | Color of the leading head character at the tip of each column. | `#80ff80` (bright green) |
| Background Color | Color | Solid background color shown behind the rain. | `#000000` (black) |
| Background Image | Media selector | Optional background image or video displayed behind the rain. Supports PNG, JPG, JPEG, WEBP, MP4, WEBM. | — |
| Glass Blur | Slider 0–30 | Blur applied to the background image. | 0 |
| Background Transparency | Slider 0–100 | Opacity of the background layer (color + image). At 0% the background is fully transparent. | 100 |

## Character Sets

| Value | Characters |
|-------|-----------|
| Katakana | Half-width katakana (ｦ–ﾝ) |
| Latin | A–Z, 0–9, and common symbols |
| Binary | 0 and 1 only |
| Mix | Katakana + Latin + digits |

## Notes

- Each column falls at its own randomized speed (1–3× the base interval) for an organic look.
- Each column has a slightly randomized tail length (±40% of the Tail Length setting).
- Character changes follow the original film's timing: glyphs hold for ~3 animation steps before being eligible to change, with ~2% of cells refreshing per eligible step.
- The canvas is transparent — the background image shows through the gaps in the rain at all times.

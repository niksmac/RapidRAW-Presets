# RapidRAW Presets

Sony-optimized [RapidRAW](https://www.getrapidraw.com) presets for nature, wildlife, landscape, and portrait photography.

## Presets

| File | Best for | Style |
|------|----------|-------|
| `Natural` | All-purpose | Clean baseline, Sony color calibration, subtle s-curve |
| `Natural-Portrait` | People | Warm skin tones, desaturated backgrounds, soft clarity |
| `Cinematic` | Storytelling | Teal shadows / orange midtones, glow, halation |
| `Bright-Airy` | Lifestyle, pastels | High-key, lifted blacks, soft desaturated |
| `Warm-Golden-Hour` | Sunset, golden light | +14 temp, boosted oranges/yellows, grain |
| `Landscape-Vibrant` | Scenery | Rich greens/blues, dehaze, vibrance 25 |
| `Wildlife-Detail` | Animals, birds | Sharpness 30, clarity 25, structure 15 |
| `Moody-Nature` | Forest, overcast | Deep shadows, desaturated, grain + vignette |

## Sony Tuning (A6400)

- **Color Calibration**: RGB primary shifts to counter Sony's cool baseline and green shadow cast
- **Temp +3 to +14, Tint +2 to +8** for natural warmth
- **Luma + chroma NR** on every preset for shadow noise at higher ISOs
- **Conservative sharpness** (max 30) — Sony JPEGs already sharpen in-camera
- **Vibrance over saturation** to protect skin tones

Designed for Sony 70-350mm F4.5-6.3 G OSS, 50mm F1.8, and 18-105mm F4 G OSS.

## Installation

Copy `presets/` and `manifest.json` into your RapidRAW presets directory, or open any `.rrpreset` file directly from the files app.

## Credits

Inspired by [CyberTimon/RapidRAW-Presets](https://github.com/CyberTimon/RapidRAW-Presets).

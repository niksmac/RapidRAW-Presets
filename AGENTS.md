# AGENTS.md

## What this repo is

Static RapidRAW (`.rrpreset`) presets tuned for Sony cameras (A6400, 70-350mm, 50mm f/1.8, 18-105mm). No build, test, or CI tooling.

## Structure

```
v1/                  # Original presets (bright, saturated, punchy)
  manifest.json      # All 8 preset definitions
  presets/*.rrpreset # Individual preset files
v2/                  # Wildlife-focused presets (muted, natural)
  manifest.json
  presets/*.rrpreset
```

## Key files

- `v{1,2}/manifest.json` — single source of truth per version (JSON array of `{name, creator, adjustments}`)
- `v{1,2}/presets/*.rrpreset` — individual preset files, each wraps a single preset with UUID
- `README.md` — preset descriptions and Sony tuning rationale

## Conventions

- Preset filenames use kebab-case and match `name` in `manifest.json` (spaces → hyphens)
- Every preset includes `colorNoiseReduction` + `lumaNoiseReduction` for Sony high-ISO noise
- `vibrance` is preferred over `saturation` to protect skin tones
- Conservative sharpness (max 30) — Sony JPEGs already sharpen in-camera
- `filmBaseColor` is `#ff8800` across all presets
- Each `.rrpreset` file requires a unique UUID in the `id` field

## Adding a new preset

1. Add entry to `v{1,2}/manifest.json` with full `adjustments` object
2. Create matching `v{1,2}/presets/<Name>.rrpreset` file with a unique UUID
3. Add row to the Presets table in `README.md`

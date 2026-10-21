# Flagifier

Make any flag image flutter. A single self-contained HTML file, no build step and no dependencies.

Open `index.html` in a browser. Drop in a PNG, WebP or SVG, adjust the motion, camera and lighting, then export.

## Export formats

| Format | Transparency |
| --- | --- |
| Animated GIF | on or off per pixel |
| Animated PNG | full alpha |
| PNG sequence (ZIP) | full alpha |
| Single frame PNG | full alpha |
| MP4 (H.264) | none, laid over a background colour |

## Requirements

WebGL 2 for the preview and all exports. MP4 also needs WebCodecs in a secure context, so serve the file over localhost if it is unavailable from `file://`:

```bash
python -m http.server 8765
```

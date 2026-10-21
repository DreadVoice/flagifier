# Flagifier

Make any flag image flutter. A single self-contained HTML file, no build step and no dependencies.

**[Try Flagifier](https://flagifier.pages.dev/)**

Open `index.html` in a browser. Drop in a PNG, WebP or SVG, adjust the motion, camera and lighting, then export.

## Export formats

| Format | Transparency |
| --- | --- |
| Animated GIF | On or off per pixel |
| Animated PNG | Full alpha |
| PNG sequence (ZIP) | Full alpha |
| Single frame PNG | Full alpha |
| MP4 (H.264) | None, laid over a background colour |

## Requirements

WebGL 2 for the preview and all exports. MP4 also needs WebCodecs in a secure context, so serve the file over localhost if it is unavailable from `file://`:

```bash
python -m http.server 8765
```

# 🎨 Aseprite Pixel Assets

A curated set of **Aseprite** assets (tiles & sprites): dirt, bush, grass, trees, water, clouds, a bonsai, a landscape scene, a small sci-fi set, and a “Ni no Kuni”–inspired study.

> Source files are `.aseprite` to keep layers, frames, palettes, tags and slices intact.

## 📁 Index
- 01-Dirt.aseprite
- 02-Dirt.aseprite
- 03-Bush.aseprite
- 04-Grass.aseprite
- 05-Tree.aseprite
- 06-Water.aseprite
- 07-SciFi.aseprite
- 08-LandScape.aseprite
- 09-Bonsai.aseprite
- 10-NinoKuni.aseprite
- 11-Clouds.aseprite
- 12-Clouds.aseprite
- 13-Clouds.aseprite

## 📤 Exports
Use Aseprite GUI (**File → Export / Export Sprite Sheet**) or the CLI:

```bash
# single PNG
aseprite -b 05-Tree.aseprite --save-as exports/05-Tree.png

# spritesheet + JSON (example options)
aseprite -b 07-SciFi.aseprite \
  --sheet exports/07-SciFi.png \
  --data  exports/07-SciFi.json \
  --sheet-type rows --filename-format {tag}_{frame} \
  --split-tags --trim

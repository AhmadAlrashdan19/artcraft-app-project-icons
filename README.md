# ArtCraft File Format Icons

Icon set for the file formats used by ArtCraft (e.g. `.pcraft` project files).
Created as a contribution proposal for the project.

<p align="center">
  <img src="png/512x512/512-PhotoCraft-Project.png" width="384" alt="Project file icon preview">
</p>

## Design

- **Shape:** a document sheet with a folded top-right corner, identical across all icons.
- **Emblem:** the ArtCraft logo in the center. Only the color and a small badge change between file types; each type uses the color of its related ArtCraft application.
- **Grid:** 1024×1024 canvas, sheet size 704×928 (3:4 ratio), built on multiples of 32 px so it scales cleanly.
- **Text:** the format name is converted to outlines, so it renders the same on every system.
- **Colors:** taken from the existing ArtCraft application icons to keep the visual identity consistent. The values are written directly in each SVG, so the palette is easy to change if the maintainers prefer different colors.

## Icons

| Icon | Format | Description |
|------|--------|-------------|
| <img src="png/512x512/512-PhotoCraft-Project.png" width="48"> | `.pcraft` | PhotoCraft project file |
| <img src="png/512x512/512-VectorCraft-Project.png" width="48"> | `.vectorcraft` | VectorCraft project file |
| <img src="png/512x512/512-FilmCraft-Project.png" width="48"> | `.fcproj` | FilmCraft project file |
| <img src="png/512x512/512-EffectCraft-Project.png" width="48"> | `.ecproj` | EffectCraft project file |
| <img src="png/512x512/512-PdfCraft.png" width="48"> | `.pdf` | PDF file |
| <img src="png/512x512/512-DesignCraft-Project.png" width="48"> | `.designcraft` | DesignCraft project file |
| <img src="png/512x512/512-AniCraft-Project.png" width="48"> | `.anicraft` | AniCraft project file |
| <img src="png/512x512/512-SoundCraft-Project.png" width="48"> | `.scraft` | SoundCraft project file |
| <img src="png/512x512/512-FigCraft-Project.png" width="48"> | `.figcraft` | FigCraft project file |

## Files

```
icons/
├── svg/      # Editable sources (text converted to outlines)
├── png/      # Exports: 16, 32, 48, 64, 128, 256, 512, 1024
├── source/   # Original .vectorcraft files (optional)
└── README.md
```

- **SVG** is the source of truth. Please edit it, not the PNGs.
- **PNG** files are exported from the SVG, with a transparent background.
- `.ico` / `.icns` are not included; they can be generated from the SVG or the 1024 px PNG.

## Naming convention

Lowercase with hyphens:

- `<type>-project.svg` (full version)
- `<size>-<type>-project.png`

Example: `photocraft-project.svg`, `512-photocraft-project.png`.

## Export settings

Exported from VectorCraft.

- **SVG:** SVG 1.1, text converted to outlines, `viewBox="0 0 1024 1024"`, not minified.
- **PNG:** transparent background, art-optimized anti-aliasing, not interlaced.

## Usage

Feel free to use these icons in ArtCraft and its related tools.
Feedback is welcome through issues or pull requests: colors, sizes, naming, or additional file types.

## License

[Choose one: CC BY 4.0 / CC0 1.0 / same license as ArtCraft]

## Author

Designed by **Ahmad Alrashdan** ([@AhmadAlrashdan19](https://github.com/AhmadAlrashdan19)).

Copyright (c) 2026 Ahmad Alrashdan. The icon designs are available under the
license above.

## Credits

The ArtCraft name and logo belong to the ArtCraft project and its authors.
They are used here only to propose icons for the project's file formats.
This repository is not an official ArtCraft release unless the maintainers
state otherwise.

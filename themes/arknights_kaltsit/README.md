# kal'tsit_(arknights)

- **Character:** 凯尔希
- **Source:** 明日方舟 / Arknights
- **Alias:** `Kal'tsit` (EN), `ケルシー` (JP)
- **Reference:** [Donmai Wiki](<https://donmai.moe/wiki_pages/arknights_kaltsit>), [PRTS](https://prts.wiki/w/%E5%87%AF%E5%B0%94%E5%B8%8C)
- **Index:** `#4`

---

> `kal'tsit_(arknights)` is the 4th character in this project. With this theme, I introduced JSON files and automation scripts, making it one of the most successful palettes compared to the first three.
>
> The JSON structure design, contrast results, semantic color fine-tuning... it wasn't until this character that a workflow was formed.
>
> Interestingly, while this theme is arguably more refined, [Mon3tr](../arknights_mon3tr/README.md)was conceived to be its semantic dark mode counterpart.

## Palette Files

| File                                                            | Purpose                                         |
| --------------------------------------------------------------- | ----------------------------------------------- |
| [`palette.json`](./palette.json)                                | Full color data                                 |
| [`palette-whiskers.json`](./palette-whiskers.json)              | Catppuccin “color_overrides” ready for Whiskers |

### Contrast Matrix

| File                                             | Description                  |
| ------------------------------------------------ | ---------------------------- |
| [`contrast-matrix.json`](./contrast-matrix.json) | All-vs-all contrast ratios   |
| [`contrast-base.json`](./contrast-base.json)     | Each swatch against **Base** |
| [`contrast-report.md`](./contrast-report.md)     | Human-readable summary       |

## Reference Artwork
 
A picture (or two) used for color sampling.
 
![sample](./assets/sample.png)

## Porting How-Tos
 
<details>
<summary>Neovim example (Catppuccin latte)</summary>

```lua
require("catppuccin").setup {
    color_overrides = {
        latte = {
        rosewater= "#B58F8F",
        flamingo = "#C28483",
        pink     = "#C180A9",
        mauve    = "#AA84DA",
        red      = "#D35B5B",
        maroon   = "#B24444",
        peach    = "#C38E66",
        yellow   = "#9C9E2F",
        green    = "#77A05E",
        sky      = "#5D9DB8",
        sapphire = "#359FBD",
        blue     = "#4F83E3",
        lavender = "#8D91E5",
        text     = "#4C4B50",
        subtext0 = "#6C6B6C",
        subtext1 = "#5C5B5E",
        base     = "#F5F4E5",
        mantle   = "#ECECDF",
        crust    = "#E2E3D8",
        surface0 = "#D2D3CA",
        surface1 = "#C2C3BC",
        surface2 = "#B2B3AE",
        overlay0 = "#A2A3A0",
        overlay1 = "#929291",
        overlay2 = "#828283",
        },
    }
}```

</details>

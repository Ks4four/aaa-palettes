# suzuran_(arknights)

- **Character:** 铃兰
- **Source:** 明日方舟 / Arknights
- **Alias:** `丽萨` (Real Name), `Suzuran`, `Lisa` (EN), `スズラン`, `リサ` (JP)
- **Reference:** [Safebooru Wiki](<https://safebooru.donmai.us/wiki_pages/suzuran_(arknights)>), [PRTS](https://prts.wiki/w/%E9%93%83%E5%85%B0)
- **Index:** `#2`

---

> `suzuran_(arknights)` is the 3rd character in this project.
>
> For this palette, I wanted to create a light theme, and Suzuran—often called "everyone's light"—felt like the perfect choice.

## Palette Files

| File                                                            | Purpose                                         |
| --------------------------------------------------------------- | ----------------------------------------------- |
| [`palette.json`](./palette.json)                                | Full color data                                 |
| [`palette-whiskers.json`](./palette-whiskers.json) | Catppuccin “color_overrides” ready for Whiskers |

### Contrast Matrix

| File                                                         | Description                  |
| ------------------------------------------------------------ | ---------------------------- |
| [`contrast-matrix.json`](./contrast/contrast-matrix.json) | All-vs-all contrast ratios   |
| [`contrast-base.json`](./contrast/contrast-base.json)     | Each swatch against **Base** |
| [`contrast-report.md`](./contrast/contrast-report.md)     | Human-readable summary       |

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
        rosewater= "#8F4E4C",
        flamingo = "#874542",
        pink     = "#8E4561",
        mauve    = "#6B4A7F",
        red      = "#b43842",
        maroon   = "#a34246",
        peach    = "#8F5524",
        yellow   = "#6E5715",
        green    = "#0C6B51",
        teal     = "#18685A",
        sky      = "#255B74",
        sapphire = "#066ca2",
        blue     = "#386a8f",
        lavender = "#715894",
        text     = "#111115",
        subtext0 = "#2b2e34",
        subtext1 = "#1e1f24",
        base     = "#E7DCB4",
        mantle   = "#DED2A6",
        crust    = "#D6C897",
        surface0 = "#C5B57B",
        surface1 = "#B5A25E",
        surface2 = "#A48F3F",
        overlay0 = "#947C16",
        overlay1 = "#806B12",
        overlay2 = "#6C5A0D",
        },
    }
}
```
</details>

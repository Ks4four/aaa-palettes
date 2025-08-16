# mon3tr_(arknights)

- **Character:** Mon3tr
- **Source:** 明日方舟 / Arknights
- **Alias:** Read as `Monster`
- **Reference:** [Safebooru Wiki](<https://safebooru>), [PRTS](https://prts.wiki/w/Mon3tr)
- **Index:** `#2`

---

> `mon3tr_(arknights)` is the 2nd character in this project.
>
> I don't have a particular preference for green characters. I chose Mon3tr simply because its green-dominant palette provided a great opportunity to test my process against a different base color than Nozomi's. I needed to see how robust the methodology was for generating a green-based theme.

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
<summary>Neovim example (Catppuccin mocha)</summary>

```lua
require("catppuccin").setup {
    color_overrides = {
        mocha = {
        rosewater= "#f5e5e0",
        flamingo = "#f2c9c0",
        pink     = "#ffb0c9",
        mauve    = "#b8a4ff",
        red      = "#FF442E",
        maroon   = "#B03A33",
        peach    = "#f7bd8f",
        yellow   = "#fcd912",
        green    = "#5ad641",
        teal     = "#5fb8a8",
        sky      = "#96d8d0",
        sapphire = "#4d9fd0",
        blue     = "#3c8dd9",
        lavender = "#a1c1ff",
        text     = "#e8e1cf",
        subtext0 = "#cdbe97",
        subtext1 = "#dacfb3",
        base     = "#1f2722",
        mantle   = "#181e1a",
        crust    = "#111513",
        surface0 = "#313d35",
        surface1 = "#435449",
        surface2 = "#556b5d",
        overlay0 = "#678171",
        overlay1 = "#7b9685",
        overlay2 = "#92a89a",
        },
    }
}
```

</details>

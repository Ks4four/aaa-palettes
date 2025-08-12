# nozomi_(blue_archive)

- **Character:** 橘ノゾミ (たちばなのぞみ)
- **Source:** ブルーアーカイブ / Blue Archive
- **Alias:** `Tachibana Nozomi` (EN), `橘望`, `橘希望` (CN)
- **Reference:** [Safebooru Donmai Wiki](<https://safebooru.donmai.us/wiki_pages/nozomi_(blue_archive)>), [Pixiv Encyclopedia](https://dic.pixiv.net/a/%E6%A9%98%E3%83%8E%E3%82%BE%E3%83%9F)
- **Index:** `#1`

---

> `nozomi_(blue_archive)` is the 1st character in this project.
> 
> Her only specialty is that she was the first.
> Unlike the importance of Catppuccin to Neovim, nozomi was simply the first.
> Because of this, if she had not existed, another character would have been the first.

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
<summary>Neovim example (Catppuccin frappe)</summary>

```lua
require("catppuccin").setup {
    color_overrides = {
        frappe = {
        rosewater= "#F5E0DC",
        flamingo = "#F2CDCD",
        pink     = "#F5C2E7",
        mauve    = "#CBA6F7",
        red      = "#F38BA8",
        maroon   = "#EBA0AC",
        peach    = "#FAB387",
        yellow   = "#F9E2AF",
        green    = "#A6E3A1",
        teal     = "#94E2D5",
        sky      = "#89DCEB",
        sapphire = "#74C7EC",
        blue     = "#89B4FA",
        lavender = "#B4BEFE",
        text     = "#F4F9E3",
        subtext0 = "#CCD2BD",
        subtext1 = "#E0E6D0",
        base     = "#292A3C",
        mantle   = "#303143",
        crust    = "#38394C",
        surface0 = "#47495C",
        surface1 = "#58596D",
        surface2 = "#686A7F",
        overlay0 = "#7A7B91",
        overlay1 = "#8C8DA3",
        overlay2 = "#9EA0B6",
        },
    }
}
```

</details>

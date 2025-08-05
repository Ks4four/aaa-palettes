# rosmontis_(arknights)

- **Character:** 迷迭香
- **Source:** 明日方舟 / Arknights
- **Alias:** `纳西莎` (Real name), `Rosmontis`, `Narcissa` (EN), `ロスモンティス`, `ナルシッサ` (JP)
- **Reference:** [Donmai Wiki](<https://donmai.moe/wiki_pages/rosmontis_(arknights)>), [PRTS](https://prts.wiki/w/%E8%BF%B7%E8%BF%AD%E9%A6%99)
- **Index:** `#10`

---

> `rosmontis_(arknights)` is the 10th character in this project.

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
			rosewater = "#d76787",
			flamingo = "#dd608d",
			pink = "#d96489",
			mauve = "#6c699f",
			red = "#d65b91",
			maroon = "#b84681",
			peach = "#d1732f",
			yellow = "#b3821f",
			green = "#469b60",
			teal = "#5a9591",
			sky = "#7d8da2",
			sapphire = "#4c6c94",
			blue = "#5e81ac",
			lavender = "#7c79a9",
			text = "#3b4251",
			subtext1 = "#4a5161",
			subtext0 = "#5a616f",
			overlay2 = "#636986",
			overlay1 = "#727896",
			overlay0 = "#838aa4",
			surface2 = "#939bb2",
			surface1 = "#a4abc1",
			surface0 = "#b5bcce",
			base = "#d8dee8",
			mantle = "#ced5e3",
			crust = "#c5cddd",
		},
	}
}
```

</details>

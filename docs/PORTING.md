# Porting a Palette

All palettes in this repository follow the Catppuccin schema. There are two primary methods for porting them: direct color overrides and theme generation with Whiskers.

## Direct Color Overrides

The fastest way to apply a palette is by overriding the default colors directly in the target application's settings.

For specific instructions, refer to the "Override palette colors" section in the documentation for the Catppuccin port you are using.

### Example — VS Code

To apply a palette in VS Code, add a `catppuccin.colorOverrides` object to the user `settings.json`:

```jsonc
{
  // ...other settings...
  "catppuccin.colorOverrides": {
    // Make text red for all flavors
    "all": {
      "text": "#ff0000",
    },
    // Make Mocha "OLEDppuccin"
    "mocha": {
      "base": "#000000",
      "mantle": "#010101",
      "crust": "#020202",
    },
  },
}
```

## Generating Themes with Whiskers

For a more comprehensive or replicable port, use [**Whiskers**](https://github.com/catppuccin/whiskers), Catppuccin’s official command-line tool. It generates complete theme files from a template, offering fine-grained control over the final output.

### Prerequisites

- [Whiskers](https://github.com/catppuccin/whiskers)
- A `palette-whiskers.json` file for the theme you want to port
- A Whiskers template for the target application (e.g., `nvim.tera` for Neovim)

### Basic Command

```bash
whiskers -f <flavor> --color-overrides <palette-whiskers.json> <template>
```

- `<flavor>`: `latte`, `frappe`, `macchiato`, or `mocha` (choose **one**)
- `<palette-whiskers.json>`: Path to the palette file
- `<template>`: Whiskers template, e.g. `nvim.tera`

### Example — Kal'tsit to Neovim

```bash
whiskers \
  -f latte \
  --color-overrides themes/arknights_kaltsit/palette-whiskers.json \
  nvim.tera
```

Whiskers will write the output to `lua/catppuccin/palettes/latte.lua`:

```lua
return {
  rosewater = "#b58f8f",
  flamingo  = "#c28483",
  -- …snip…
  crust     = "#e2e3d8",
}
```

From there, follow Catppuccin’s Neovim setup guide to enable the palette.

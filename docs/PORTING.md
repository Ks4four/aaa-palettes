# Porting a Palette with Whiskers

All palettes in this repo follow the Catppuccin schema, so the fastest way to port them is Catppuccin’s official tool [**Whiskers**](https://github.com/catppuccin/whiskers).

## Prerequisites

- [Whiskers](https://github.com/catppuccin/whiskers)
- A `palette-whiskers.json` file for the character you want to port
- A Whiskers template for your target application (e.g., `nvim.tera` for Neovim)

## Basic Command

```bash
whiskers -f <flavor> --color-overrides <palette-whiskers.json> <template>
```

- `<flavor>`: `latte`, `frappe`, `macchiato`, or `mocha` (choose **one**)
- `<palette-whiskers.json>`: path to the palette file
- `<template>`: Whiskers template, e.g. `nvim.tera`

## Example — Kal'tsit to Neovim

```bash
whiskers \
  -f latte \
  --color-overrides themes/arknights_kaltsit/palette-whiskers.json \
  nvim.tera
```

Whiskers writes the result to `lua/catppuccin/palettes/latte.lua`:

```lua
return {
  rosewater = "#b58f8f",
  flamingo  = "#c28483",
  -- …snip…
  crust     = "#e2e3d8",
}
```

From there, follow Catppuccin’s Neovim setup guide to enable the palette.

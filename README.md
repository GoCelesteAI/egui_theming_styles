# egui Theming and Styles — Theme Editor

**Learn egui in Neovim — Episode 26**

Build a Theme Editor with live style controls using egui's `Visuals` and `Style` systems. Features a side panel with dark/light mode toggle, accent color picker, rounding and spacing sliders, and a reset button — with a central panel that previews all changes in real time.

## What You'll Build

A theme editor with:
- Dark/light mode toggle using `egui::Visuals::dark()` / `light()`
- Accent color picker with `color_edit_button_rgb`
- Corner rounding slider (0–20px) via `CornerRadius::same()`
- Widget spacing slider applied through `Style`
- Reset button to restore default values
- Live preview panel with sample widgets

## Prerequisites

- Rust installed ([rustup.rs](https://rustup.rs))
- Basic Rust knowledge (structs, enums, closures)

## Run

```bash
cargo run
```

## Key Concepts

- `egui::Visuals::dark()` / `light()` — preset color themes
- `visuals.selection.bg_fill` — accent color for selections and active widgets
- `egui::Color32::from_rgb()` — custom color from RGB values
- `egui::CornerRadius::same()` — uniform corner rounding for all widgets
- `style.spacing.item_spacing` — global widget spacing
- `ctx.set_style()` — apply style changes each frame
- `color_edit_button_rgb()` — interactive color picker widget
- `egui::Slider` with `.suffix()` — formatted slider display

## Series

This is part of the [Learn egui in Neovim](https://www.youtube.com/@GoCelesteAI) series — 36 episodes teaching Rust GUI development with egui, coded entirely in Neovim.

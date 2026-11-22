# Glowing Blocks for Horizon

A minimal **content mod** for [Horizon](https://github.com/horizon-rust/horizon), the Rust
rewrite of Minecraft Java Edition 26.3. It adds one block (`glowing_amethyst`) using only
data and asset files вЂ” no Java code and no Fabric loader.

This project was generated with `cargo horizon-mod new` from Horizon's own mod tooling and
built with `cargo-horizon-mod`, then packaged as a `.hmod` without requiring the launcher.

## Install

1. Copy `glowing_blocks-0.1.0+mc26.3.hmod` into your Horizon game folder's `horizon-mods/`.
2. Add `mod.glowing_blocks:true` to `horizon-mods.txt` in the same folder.
3. Start a 26.3 instance; craft the block from an amethyst block and glowstone dust.

## Build

Requires Rust 1.95+ and the Horizon tool:

```sh
cargo install --locked --git https://github.com/horizon-rust/horizon cargo-horizon-mod
cargo horizon-mod build
```

The result is `target/horizon-mod/glowing_blocks.hmod`.

## Attribution and license

* Based on the official [Horizon native mod template](https://github.com/horizon-rust/horizon-native-mod-template)
  and Horizon's content-mod generator. Credit goes to the **Horizon Team**, founded by
  Ludovic Marie, and all contributors.
* Horizon's original project work is licensed **LGPL-3.0-or-later**; older merged code is MIT.
  This generated content mod is provided under the **MIT** license (see `LICENSE`), matching
  the template it was generated from. This is not an official Mojang/Microsoft product.
* **LLM disclosure:** the repository scaffolding, build scripts, packaging and documentation
  were prepared with LLM assistance (OpenCode agent) and reviewed before upload. No upstream
  Horizon source was submitted as a pull request from this work.

## Version

`0.1.0+mc26.3` вЂ” targets Horizon's pinned Minecraft Java Edition 26.3.
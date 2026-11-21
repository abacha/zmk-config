# zmk-config

ZMK firmware for a Corne 42 (nice!nano v2, nice!oled).
Derived from KeebMaker/zmk-config (MIT).

## The repository is the source of truth

`config/corne.keymap` defines the keymap.
Anything that exists only in ZMK Studio is lost on the next settings reset or reflash.
To keep a change, make it in this repository.

## Editing the keymap

- Web editor: [nickcoutsos.github.io/keymap-editor](https://nickcoutsos.github.io/keymap-editor/) with GitHub access to this private repo; saving commits to `main`.
- Or edit `config/corne.keymap` directly and push.

## Firmware

Every push to `main` builds the left half, the right half and `settings_reset`.
Download the `.uf2` files from the artifact of the latest run in the Actions tab.
Flashing the keyboard is manual: double-tap reset on a half and copy its `.uf2` to the mounted drive.

## Layer cheatsheet

The `draw` workflow renders `keymap-drawer/corne.svg` from the keymap on every change to it.

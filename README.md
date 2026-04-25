# ZMK Config for Sofle (MTZ)

This repository contains a custom ZMK (Zephyr Mechanical Keyboard) configuration for the Sofle keyboard, tailored for the "eyelash_sofle" variant. It provides all necessary files and settings to build and customize your own Sofle keyboard firmware using ZMK.

## Hardware Overview

**Board Name:** Eyelash Sofle

- **MCU:** ARM (nRF52840)
- **RAM:** 40 KB
- **Supported Features:**
	- ADC, USB Device, BLE, IEEE802154, PWM, Watchdog, GPIO, I2C, SPI
- **Matrix:** 5 rows × 14 columns (split)
- **Rotary Encoder:** Alps EC11 (left side, 40 steps, configurable)
- **Underglow & Backlight:** Supported
- **Physical Layout:** Custom Sofle ergonomic layout

## Features
- Custom keymap and layout for Sofle (MTZ)
- Board and shield definitions for the eyelash_sofle variant (based on nano!view)
- Ready-to-use configuration files for ZMK
- Easily modifiable YAML and DTS files for advanced customization

## Directory Structure
- `boards/arm/eyelash_sofle/` — Board definitions, device trees, matrix/encoder/backlight configuration, and keymap files
- `config/` — Main configuration, keymap, and west manifest
- `keymap-drawer/` — YAML files for visualizing and editing keymaps
- `zephyr/` — Zephyr module configuration

## Getting Started
1. **Clone this repository**
2. **Install ZMK build environment** ([ZMK setup guide](https://zmk.dev/docs/development/setup/))
3. **Build your firmware** using the provided configuration files and board definitions
4. **Flash your Sofle keyboard** with the generated firmware

## Customization
- Edit the keymap files in `config/` or `boards/arm/eyelash_sofle/` to suit your preferences
- Use the `keymap-drawer` YAML files for visual keymap editing
- Adjust hardware features (matrix, encoder, underglow, backlight) in the device tree files (`.dts`, `.dtsi`)

## Credits
This repository is inspired and based on [a741725193/zmk-sofle](https://github.com/a741725193/zmk-sofle). Many thanks to the original author and the ZMK community for their contributions!

## License
This project is open source and available under the MIT License.

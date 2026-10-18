# Scarab

## Overview
Scarab is a custom input device that combines keyboard and trackball functionality into a single unit. It is designed for gaming and productivity use cases, with an emphasis on input control rather than traditional coding workflows. The device functions as a unified interface for both mouse and keyboard inputs, enabling gameplay in various environments.

> **Keyboard Maintainer**: [soundsewcrazy](https://github.com/soundsewcrazy)
> **Hardware Supported**: Pro Micro or clone hardware
> **Availability**: [GitHub releases](https://github.com/soundsewcrazy/Scarab/releases)

## Target Use Cases
- Gaming environments (RTS, MOBAs, FPS)
- Desktop workstations
- Portable use scenarios

The device is intended for users who require combined input methods in a single unit.

## 3D Files & Printing
- **Files Available**: STL files for all keyboard components are included in the repository for download and printing.
- **Recommended Printer**: ELEGOO Neptune 3 Plus (or compatible FDM printer).
- **Print Settings**: Use a 0.6mm nozzle with PETG filament.
- **Post-Processing**: Minor cleaning after printing is required to achieve proper fit with hardware and PCBs.
- **Model Tolerances**: Clearances are optimized for standard printers using a 0.6mm nozzle, resulting in a relatively tight fit.
- **Retention Mechanism**: Heat set inserts are used to secure components and hardware.
- **Keycap Requirement**: Regular keycaps will not fit due to the 16.5mm key spacing. Specific keycap models designed for this pitch must be used.

## PCB Information & Manufacture
- **Files Available**: PCB gerb files and original KiCad source are located in the `production` subfolder.
- **Manufacturing**: Initial runs were produced via JLCPCB (small quantities).
- **Switch Configuration**: Standard panels use regular Cherry MX switches. Akko Blue and Silver Speed switches are featured in documentation.
- **Switch Recommendations**: Linear switches are highly recommended for thumb clusters for easy actuation. Tactile or clicky switches may be used on hand panels if preferred.

## QMK Firmware & Keymapping
- **Firmware Tool**: QMK is required to compile firmware from source or flash precompiled HEX files.
- **Usage Methods**: 
  - Flash precompiled HEX files included in the repository.
  - Compile firmware directly from uncompiled source using QMK software.
- **Keymap Location**: Default keybindings are defined in the `keymaps` directory.
- **Customization Process**: 
  1. Edit keymap files within the `keymaps/` folder.
  2. Re-compile the firmware using QMK.
  3. Flash the updated HEX file to the device.

## Installation & Setup
- Clone the project from [GitHub](https://github.com/soundsewcrazy/Scarab).
- Install and configure QMK software on your machine.
- Select a firmware method (precompiled HEX or source compilation) based on technical preference.
- Initial configuration may require reference to variant documentation for keymap implementation.

## Variants
### Dynastinae — Thumb Support Model
The Dynastinae variant adds dedicated thumb panels to the standard trackball/keyboard hybrid. This configuration supports right-handed use as default, with left-handed assembly requiring component mirroring.

**Configuration:**
- Thumb Panels: 8 keys per cluster
- Hand Panels: Standard keyboard layout (30 keys, 5 rows of 6 columns)
- Left-Handed Assembly: Mirror body components to swap left/right panels

Additional variants are planned.

## Contributing & Community
Contributions through project forks are welcome

Support is community-driven; formal support is not guaranteed.
---
*This documentation reflects current information as of 2026-10-18.*
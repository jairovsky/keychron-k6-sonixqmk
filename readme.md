### SonixQMK configuration for Keychron K6 (RGB ANSI)

This is a working copy of https://github.com/SonixQMK/qmk_firmware/pull/367

The critical configuration (rgb_matrix and pin mappings) is the same from the PR above.

You should clone the most recent version of SonixQMK/qmk_firmware, and then clone this repo inside the `keyboards` directory.

What's changed:
- mapped the lightbulb key do Delete (hooray! it's now a useful key).
    - fn2 + lightbulb: cycle through RGB animation modes
- fn2 + P: Print Screen key
- fn2 + B: reboot the keyboard into bootloader mode (no need to disassemble and short the pins behind the board anymore)

Note that all RGB animation modes are disabled by default. Just enable the ones you prefer before compiling.

Working environment
- Ubuntu 24.04
- Compiled against SonixQMK/qmk_firmware (commit id 6657474b400d54e93f3eaef9a72f91cb314b2ffb)
- Flashed with SonixQMK/SonixFlasherC 2.0.8

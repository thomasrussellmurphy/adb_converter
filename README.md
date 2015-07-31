# adb_converter

A subset of [tmk_keyboard][keyboard] with just the Apple Desktop Bus
functionality.

This is the firmware for circuit boards that I designed and built. To give me
ease of isolation from the upstream development, I created this repository with
the correct configurations for both boards.

The manufacturing files for these boards is available at [adb-to-usb][boards].
The information may be incomplete and some revisions of the boards have severe
errors, but they were coaxed into functioning.

To use, select the correct branch (master or enclosed-aek-converter-config).
Then:

```bash
cd converter/adb_usb
make
# Connect board in reset mode for DFU programming
make dfu
```

[keyboard]: https://github.com/tmk/tmk_keyboard
[boards]: https://github.com/thomasrussellmurphy/adb-to-usb

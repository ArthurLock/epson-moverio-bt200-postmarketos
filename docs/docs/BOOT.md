# Boot Guide — Epson Moverio BT-200

This document covers booting postmarketOS on the Epson Moverio BT-200 (EMBT2WS).

## Important

The BT-200 uses a device-specific bootloader. Writing an operating system image to a microSD card does not, by itself, guarantee that the device will boot from that card.

The boot procedure must be verified against the exact device configuration and image being used.

## Before attempting to boot

1. Confirm that the disk image was written successfully.
2. Verify the image SHA-256 checksum.
3. Make sure the microSD card is inserted correctly.
4. Ensure the device has sufficient battery charge.
5. Read the official device documentation.

Device wiki:

https://wiki.postmarketos.org/wiki/Epson_Moverio_BT-200_(epson-embt2ws)

## Bootloader behavior

The BT-200 bootloader has device-specific boot logic, including checks involving `sdboot.scr`.

The order in which boot sources are checked can affect whether an operating system on microSD starts.

Do not assume that the device will automatically boot from microSD simply because the card contains a valid image.

## If the device does not boot

Record the following information:

- Whether the display turns on.
- Whether any startup logo appears.
- Whether the device's LEDs indicate activity.
- Whether the behavior changes with or without the microSD card.
- Whether the device can still start its original operating system.

These observations help distinguish a boot-selection issue from an image, kernel or hardware problem.

## Bootloader modifications

Do not flash a bootloader or modify internal storage based on generic instructions for other devices.

Before changing boot settings, make sure the procedure is appropriate for the BT-200 and that a recovery method is available.

## Verification status

The precise boot procedure for the published image must be documented after it has been verified on physical hardware.

This guide will be updated with tested, step-by-step instructions as results become available.

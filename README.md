# Epson Moverio BT-200 — postmarketOS

A community project to bring postmarketOS Linux to the Epson Moverio BT-200 smart glasses (model EMBT2WS).

The goal is simple: make Linux on the Moverio BT-200 accessible to everyone, without requiring users to build the operating system from scratch.

## Project status

A postmarketOS-based disk image has been built for the Epson Moverio BT-200.

**Important:** The image has been built, but successful boot and hardware functionality must be verified on the physical device before this release can be described as fully tested.

## Device information

- **Device:** Epson Moverio BT-200
- **Device model:** EMBT2WS
- **Platform:** Texas Instruments OMAP4460
- **Architecture:** ARMv7
- **Operating system:** postmarketOS / Nura edge
- **Intended installation media:** microSD card

## Download

A prebuilt disk image is intended to be provided through the GitHub Releases section.

**Releases:**  
https://github.com/ArthurLock/epson-moverio-bt200-postmarketos/releases

If no release is available yet, the image has not been published. Please do not use an unrelated image.

## Image verification

The original image filename is:

`epson-embt2ws-postmarketOS.img`

Original image size: 1,949,302,784 bytes.

SHA-256 checksum of the original image:

`0d5d9f7abaf949bf5a2f6423a8f1a3af48e9fb316e4ab4675195f61b6b04f862`

Always verify the downloaded image against the checksum published with the corresponding release. A compressed download will have a different checksum from the uncompressed image.

## Installation overview

The intended process is:

1. Download the image from GitHub Releases.
2. Verify its SHA-256 checksum.
3. Write the image to a suitable microSD card using a disk imaging tool.
4. Safely eject the card and insert it into the Moverio BT-200.
5. Follow the device-specific boot instructions.

**Warning:** Writing a disk image overwrites the selected target device and destroys existing data on it. Double-check the selected drive before writing.

## Boot instructions

The BT-200 uses a bootloader with device-specific boot behavior. Simply writing an image to a microSD card may not be sufficient to make the device boot from it.

Please consult the device documentation before attempting bootloader changes:

https://wiki.postmarketos.org/wiki/Epson_Moverio_BT-200_(epson-embt2ws)

Boot instructions for this project's specific image will be documented here as they are verified.

## Hardware compatibility

Hardware functionality must be tested on the actual device. Do not assume that every component works just because the operating system image builds successfully.

Testing and documentation should cover:

- Display and graphical interface
- Wi-Fi and networking
- Audio output
- Buttons and input
- Battery status and power management
- Suspend and resume
- microSD boot behavior

Known limitations and verified results will be documented as testing progresses.

## Building from source

This project uses postmarketOS and pmbootstrap.

Official project resources:

- postmarketOS: https://postmarketos.org/
- pmbootstrap: https://gitlab.postmarketos.org/postmarketOS/pmbootstrap
- Device wiki: https://wiki.postmarketos.org/wiki/Epson_Moverio_BT-200_(epson-embt2ws)

Reproducible build instructions, device configuration, kernel information and any project-specific patches will be added as they are collected and verified.

## Contributing

Owners of the Epson Moverio BT-200 are welcome to share test results, installation experiences, hardware compatibility information and improvements to the documentation.

Please include the exact device model and relevant logs when reporting a problem.

## Disclaimer

This is a community project and is not affiliated with or endorsed by Epson.

Use the image at your own risk. Back up important data before making changes to storage or boot configuration. Do not modify the device's bootloader unless you understand the risks and have a recovery plan.

The software is provided without any guarantee of functionality or fitness for a particular purpose.

## License

Licensing information for project-specific documentation, configuration and patches will be added after their origins and applicable licenses have been reviewed.

Third-party software remains subject to its respective license terms.

# Troubleshooting — Epson Moverio BT-200

This page collects troubleshooting advice for postmarketOS on the Epson Moverio BT-200 (EMBT2WS).

## 1. The device does not boot from microSD

Possible causes include bootloader behavior, an incorrectly written image, an incompatible card or an image that has not been verified on physical hardware.

Try the following:

1. Verify the SHA-256 checksum of the downloaded image.
2. Confirm that the image was written as a disk image, not copied as a regular file.
3. Check that the microSD card is inserted correctly.
4. Charge the device before testing again.
5. Consult the device-specific boot guide.

Device wiki:

https://wiki.postmarketos.org/wiki/Epson_Moverio_BT-200_(epson-embt2ws)

Do not modify the bootloader or internal storage without a verified procedure and a recovery plan.

## 2. The display remains black

A black screen alone does not establish the cause of a boot failure.

Record whether the device shows a startup logo, whether LEDs indicate activity and whether the original operating system still starts.

## 3. Wi-Fi or networking does not work

Networking functionality may depend on the device configuration, drivers and userspace services.

Record the observed behavior and any available system logs. Do not assume that every network interface is configured automatically.

## 4. Audio does not work

Check the volume, audio output selection and available audio services after confirming that the operating system has booted.

If audio is unavailable, include relevant system logs and describe whether the problem affects all audio or only a particular application.

## 5. Battery status appears incorrect

Battery reporting and power management may have limitations on this device. An incorrect battery indicator does not necessarily mean that the operating system has failed to boot.

## 6. Reporting a problem

When opening an issue, include:

- Exact device model: Epson Moverio BT-200 / EMBT2WS.
- The release version and image filename.
- Whether the image checksum matches.
- The microSD card capacity and writing tool.
- A description of the startup behavior.
- Any available logs or error messages.

Avoid publishing personal information in logs.

## 7. Testing status

This project distinguishes between a successful image build and verified operation on physical hardware.

Hardware compatibility claims will be updated as actual test results become available.

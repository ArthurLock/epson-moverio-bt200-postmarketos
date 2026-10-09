# Installation Guide — Epson Moverio BT-200

This guide is for the Epson Moverio BT-200 (EMBT2WS) and the postmarketOS image provided by this project.

## 1. Before you start

You will need:

- An Epson Moverio BT-200 (EMBT2WS).
- A microSD card with sufficient capacity for the disk image.
- A Windows or Linux computer.
- A disk imaging tool.
- A backup of any important data on the target microSD card.

**Warning:** Writing a disk image erases existing data on the selected target drive. Carefully verify the selected drive before writing.

## 2. Download the image

Visit the project's Releases page:

https://github.com/ArthurLock/epson-moverio-bt200-postmarketos/releases

Download the disk image if a release is available.

The original image filename is:

`epson-embt2ws-postmarketOS.img`

If no release asset is available, the image has not yet been published.

## 3. Verify the image

The original, uncompressed image has the following SHA-256 checksum:

`0d5d9f7abaf949bf5a2f6423a8f1a3af48e9fb316e4ab4675195f61b6b04f862`

On Windows, open PowerShell in the download directory and run:

```powershell
Get-FileHash .\epson-embt2ws-postmarketOS.img -Algorithm SHA256
```

On Linux, run:

```bash
sha256sum epson-embt2ws-postmarketOS.img
```

Compare the resulting hash with the checksum published for the release. Do not use the image if the checksum does not match.

## 4. Write the image to microSD

Use a disk imaging tool that supports writing raw `.img` files, such as balenaEtcher.

1. Select the downloaded image.
2. Select the intended microSD card as the target.
3. Double-check the target device.
4. Start writing and wait for the process to finish.
5. Safely eject the card.

**Important:** Do not select your computer's system drive. Writing an image to the wrong drive can destroy its data.

## 5. Booting the Moverio

The BT-200 has device-specific bootloader behavior. Writing the image to microSD does not guarantee that the glasses will boot from it.

Read the device-specific documentation first:

https://wiki.postmarketos.org/wiki/Epson_Moverio_BT-200_(epson-embt2ws)

Follow boot instructions verified for this project's image. Do not change bootloader settings or flash internal storage without a documented procedure and a recovery plan.

## 6. Troubleshooting

If the device does not boot:

- Verify the image checksum.
- Confirm that the image was written to the microSD card, not copied as an ordinary file.
- Check that the card is readable and correctly inserted.
- Record any LED activity, screen behavior or boot messages.
- Consult the device wiki and report the exact symptoms.

Do not assume that a black screen necessarily means the image was written incorrectly.

## 7. Current testing status

The image has been built, but successful boot and hardware functionality on a physical BT-200 must be confirmed before compatibility can be considered fully verified.

Test results and device-specific boot instructions will be updated as they become available.

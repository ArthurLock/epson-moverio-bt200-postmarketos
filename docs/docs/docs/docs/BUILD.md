# Build Guide — Epson Moverio BT-200

This guide introduces the tools and information needed to build postmarketOS for the Epson Moverio BT-200 (EMBT2WS).

A prebuilt image is the recommended starting point for users who do not want to build the operating system themselves.

## 1. Requirements

You will need:

- A Linux build environment.
- Git and the dependencies required by pmbootstrap.
- An internet connection to access source repositories and package mirrors.
- Sufficient free disk space for downloaded packages, build artifacts and the resulting image.

A virtual machine can be used, provided that it has sufficient resources and working network access.

## 2. Official resources

- postmarketOS: https://postmarketos.org/
- pmbootstrap source: https://gitlab.postmarketos.org/postmarketOS/pmbootstrap
- Epson Moverio BT-200 device wiki: https://wiki.postmarketos.org/wiki/Epson_Moverio_BT-200_(epson-embt2ws)
- postmarketOS package ports: https://gitlab.postmarketos.org/postmarketOS/pmaports

Consult the device-specific documentation before choosing a device package, kernel or installation method.

## 3. Obtain pmbootstrap

Follow the current official pmbootstrap installation instructions:

https://wiki.postmarketos.org/wiki/Pmbootstrap

Use the documented installation method appropriate for your Linux distribution.

## 4. Select the device configuration

The target device is:

`epson-embt2ws`

Verify that the corresponding device configuration and kernel package are available in the package repository version you intend to use.

Device packages, kernel versions and build instructions can change over time. Do not assume that instructions written for an older revision will work unchanged with current sources.

## 5. Build the image

Follow the current pmbootstrap documentation and the device-specific instructions to configure the target and generate an image.

The exact build commands and configuration used to produce this project's published image will be documented after the original build environment and package revisions have been recorded.

## 6. Reproducibility

For a reproducible build, record at least:

- The pmbootstrap Git commit.
- The pmaports revision used.
- The device package version.
- The kernel package version and patches.
- The selected operating system channel and architecture.
- The image-generation configuration.
- Any local changes required to complete the build.

Local patches should be documented and reviewed before being published.

## 7. Network and mirror issues

Build environments may encounter DNS, proxy, TLS or package-mirror failures.

Check the current official Alpine Linux and postmarketOS mirror configuration before changing repository URLs. Avoid permanently modifying build scripts just to work around a temporary network problem.

If a proxy is required, configure it according to the documentation for your environment and verify that package downloads work.

## 8. Contributing build improvements

When submitting build fixes, include the affected package, the source revision, the reason for the change and the results of testing.

Do not publish credentials, private proxy settings or other sensitive configuration.

## 9. Current limitations

The complete, independently reproducible build procedure for the published image is still being documented.

The prebuilt image and its published checksum should be used to identify the specific release being tested.

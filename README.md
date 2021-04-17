# custom-freebsd-13

Create a custom FreeBSD ISO that will install unattended. Based on [mi-freebsd-10](https://github.com/joyent/mi-freebsd-10) by Joyent.

## Requirements

This must be run on a FreeBSD host as user root.

## Setup

Before using this you need to install the following packages:

```
pkg install -y zsh rsync cdrtools git
```

## Usage

To build a custom ISO, run the `build_freebsd_iso` script:


```
./build_freebsd_iso
```

This will download an ISO, created a customized layout with installerconfig, then build the custom ISO.


## Customizing
You can modify the following if you'd prefer a different ISO, architexture, or FreeBSD mirror:

```
MIRROR="ftp.uk.freebsd.org"
MIRROR_PATH="pub/FreeBSD/releases/amd64/ISO-IMAGES"
ISO="FreeBSD-13.0-RELEASE-amd64-disc1.iso"
CUSTOM_ISO_FILENAME="freebsd-13-custom.iso"
```

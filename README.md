# MCC Interim Linux Modern Guide

This repository documents the process of installing and booting MCC Interim Linux with Linux kernel 1.0.4 using the Bochs emulator on modern hardware.

The goal of this project is historical preservation, experimentation, and making early Linux easier to explore for modern users.

## What is included

* Working Bochs configuration
* Bootable Linux 1.0.4 hard disk image
* Original floppy disk images
* Installation walkthrough
* Troubleshooting notes
* Screenshots

## Why Bochs instead of QEMU?

QEMU repeatedly froze during the installation and boot process. Bochs emulates older hardware more accurately for very early Linux versions and worked reliably for MCC Interim Linux.

## System information

```bash
uname -a
Linux linux 1.0.4 #1 Wed Mar 30 23:49:33 GMT 1994 i686
```

## Notes

This software is preserved for historical and educational purposes.

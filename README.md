# MCC Interim Linux on modern hardware

A preservation and systems-learning project documenting an installation of MCC Interim Linux with Linux kernel 1.0.4 under Bochs. It includes the emulator configuration, disk images, installation notes, and screenshots of the recorded boot process.

## Included artifacts

- `disks/mcc-hdd.img`: prepared hard-disk image.
- `disks/nocdboot` and `disks/root`: installation floppy images.
- `configs/mcc-bochs.txt`: example Bochs configuration.
- `mcc_interim_linux_guide.pdf`: walkthrough and troubleshooting notes.
- `OG-mcc-User-manual.pdf`: historical reference manual.
- `Screenshots/`: partitioning, installation, errors, and successful boot captures.

The [v1.0 release](https://github.com/aminewe898/mcc-interim-linux-modern-guide/releases/tag/v1.0) packages the principal images, configuration, and guide.

## Reproduce the setup

Clone or download the repository. Install Bochs, review the guide, and edit a local copy of `configs/mcc-bochs.txt` to point to your BIOS/VGA BIOS and the supplied files. Paths are now relative to the repository root; start Bochs with that root as the working directory.

```sh
bochs -f configs/mcc-bochs.txt
```

Keep the source disk image unchanged: use a working copy when experimenting, and update the local configuration to refer to that copy. Bochs can write to its configured disk.

## Technical focus

Early Linux installation, disk geometry and partitioning, floppy-based bootstrap, emulator compatibility, and documenting failure/recovery steps. Bochs worked for the recorded installation after QEMU attempts froze; this is experience from this setup, not a universal emulator benchmark.

## Status and boundaries

The repository records a successful installation and has a published release. A fresh boot was not repeated during portfolio curation. This obsolete OS is for isolated historical exploration, not exposure to an untrusted network or use as a modern server.

## Licensing

The repository's [LICENSE](LICENSE) covers material where applicable. Historical Linux distributions, disk contents, manuals, and emulator dependencies retain their respective licenses; the repository license does not relicense third-party software.

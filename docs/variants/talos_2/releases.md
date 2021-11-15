# Raptor Computing Systems Talos II Dasharo Release Notes

Following Release Notes describe status of Open Source Firmware development for
Raptor Computing Systems Talos II

For details about our release process please read
[Dasharo Standard Release Process](../../dev-proc/standard-release-process.md).

[Subscribe to Raptor Computing Systems Talos II Dasharo Release Newsletter]( https://newsletter.3mdeb.com/subscription/w2Y2G4Rrj){ .md-button .md-button--primary .center }

## v0.4.0 - 2021-10-29

### Added
  - OCC support
  - XIVE support
  - PCIe initialization
  - IPMI block transfer interface
  - Non-constant nodes in Device Tree are generated programmatically

### Known issues
  - [Only one CPU is started](https://github.com/Dasharo/dasharo-issues/issues/30)
  - [SPDs are not exposed in sysfs automatically](https://github.com/Dasharo/dasharo-issues/issues/31)
  - [Missing parts of Device Tree describing specific unit (VPD, serial numbers)](https://github.com/Dasharo/dasharo-issues/issues/32)
  - [Watchdog times out](https://github.com/Dasharo/dasharo-issues/issues/29)

### Binaries

[dasharo_talos_2_bootblock_v0.4.0.signed.ecc](https://cloud.3mdeb.com/index.php/s/54MDtRgBNEmyKo6){ .md-button }
[sha256](https://cloud.3mdeb.com/index.php/s/DwpWdgfZyD9StBW){ .md-button }
[sha256.sig](https://cloud.3mdeb.com/index.php/s/5xawXEissBZN6rT){ .md-button }

[dasharo_talos_2_coreboot.rom.signed.ecc](https://cloud.3mdeb.com/index.php/s/5Pbw5EtmNimrdrj){ .md-button }
[sha256](https://cloud.3mdeb.com/index.php/s/TNcLAz3CZo4QzeD){ .md-button }
[sha256.sig](https://cloud.3mdeb.com/index.php/s/9Fr6Kn57mP2bbwS){ .md-button }

[zImage_v0.4.0.bundled](https://cloud.3mdeb.com/index.php/s/o5RE7oj4r9kFXS2){ .md-button }
[sha256](https://cloud.3mdeb.com/index.php/s/FgeHfa4LzcZK6Pj){ .md-button }
[sha256.sig](https://cloud.3mdeb.com/index.php/s/awNSefJrN4d2tAD){ .md-button }

### SBOM (Software Bill of Materials):

- [coreboot based on 5621a1e revision b535763b](https://github.com/Dasharo/coreboot/tree/raptor-cs_talos-2_v0.4.0)
- [skiboot based on 04-16-2019 revision 98581863](https://git.raptorcs.com/git/talos-skiboot/)
- [heads based on 21e50681 revision 34c77951](https://git.raptorcs.com/git/talos-skiboot/commit/?id=9858186353f2203fe477f316964e03609d12fd1d)
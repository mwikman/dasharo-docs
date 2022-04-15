# Dasharo compatible with MSI PRO Z690-A WIFI DDR4 Release Notes

Following Release Notes describe status of Open Source Firmware development for
MSI PRO Z690-A WIFI DDR4

For details about our release process please read
[Dasharo Standard Release Process](../../dev-proc/standard-release-process.md).

<center>
[Subscribe to Dasharo compatible with MSI PRO Z690-A WIFI DDR4 Newsletter]
[newsletter]{.md-button .md-button--primary .center}
</center>

## v0.1.0 - 2022-04-13
### Added

- Initial support for the MSI PRO Z690-A WIFI DDR4 platform
- [Dasharo boot logo](https://docs.dasharo.com/unified-test-documentation/dasharo-compatibility/304-custom-logo/)
- [Dasharo SMBIOS compatibility](https://docs.dasharo.com/unified-test-documentation/dasharo-compatibility/31L-smbios/)
- [UEFI compatibility](https://docs.dasharo.com/unified-test-documentation/dasharo-compatibility/30M-uefi-compatible-interface/)
- [UEFI shell](https://docs.dasharo.com/unified-test-documentation/dasharo-compatibility/30P-uefi-shell/)
- Configurable boot order
- Configurable boot options
- One-time boot feature
- [External HDMI and Display Port rear panel display support](https://docs.dasharo.com/unified-test-documentation/dasharo-compatibility/31E-display-ports-and-lcd/)
- [USB support](https://docs.dasharo.com/unified-test-documentation/dasharo-compatibility/306-usb-hid-and-msc-support/)

### Known issues

- [USB storage devices disappear after reboot/power failure](https://github.com/Dasharo/dasharo-issues/issues/70)

### Binaries

[MSI PRO Z690-A WIFI DDR4 v0.1.0][v0.1.0_rom]{.md-button}
[sha256][v0.1.0_hash]{.md-button}
[sha256.sig][v0.1.0_sig]{.md-button}

See how to verify signatures on [this video](https://youtu.be/741UtuZE8fA)

Commands snippet:

```
gpg --fetch-keys https://raw.githubusercontent.com/3mdeb/3mdeb-secpack/master/keys/master-key/3mdeb-master-key.asc
gpg --fetch-keys https://raw.githubusercontent.com/3mdeb/3mdeb-secpack/master/dasharo/3mdeb-dasharo-master-key.asc
gpg --fetch-keys https://raw.githubusercontent.com/3mdeb/3mdeb-secpack/master/dasharo/3mdeb-dasharo-master-key.asc
gpg --list-sigs "3mdeb Master Key" "3mdeb Dasharo Master Key" "Dasharo release 0.x compatible with MSI MS-7D25 signing key"
wget https://3mdeb.com/open-source-firmware/Dasharo/msi_ms7d25/msi_ms7d25_v0.1.0.rom
wget https://3mdeb.com/open-source-firmware/Dasharo/msi_ms7d25/msi_ms7d25_v0.1.0.rom
wget https://3mdeb.com/open-source-firmware/Dasharo/msi_ms7d25/msi_ms7d25_v0.1.0.rom.sha256.sig
sha256sum -c msi_ms7d25_v0.1.0.rom.sha256
gpg --verify msi_ms7d25_v0.1.0.rom.sha256.sig msi_ms7d25_v0.1.0.rom.sha256
```

### SBOM (Software Bill of Materials):

- [coreboot based on a552cfc9 revision 53948cd8](https://github.com/Dasharo/coreboot/commit/53948cd8)
- [edk2 based on 4d2846ba revision 4d2846ba](https://github.com/Dasharo/edk2/tree/4d2846ba)

[newsletter]: https://newsletter.3mdeb.com/subscription/aKgTJjYEA
[v0.1.0_rom]: https://3mdeb.com/open-source-firmware/Dasharo/msi_ms7d25/msi_ms7d25_v0.1.0.rom
[v0.1.0_hash]: https://3mdeb.com/open-source-firmware/Dasharo/msi_ms7d25/msi_ms7d25_v0.1.0.rom.sha256
[v0.1.0_sig]: https://3mdeb.com/open-source-firmware/Dasharo/msi_ms7d25/msi_ms7d25_v0.1.0.rom.sha256.sig
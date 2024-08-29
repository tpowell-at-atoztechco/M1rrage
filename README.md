# Welcome, 
## check out the amazing M1rrage!
<b>M1rrage</b> emulates <i>Apple Silicon</i> on <a>non-Apple hardware</a> using a custom QEMU configuration. 
<b><u>This software is still beta, we are in the process of publishing it. When we do, this disclaimer will be removed!</u></b>

## Overview
<b>M1rrage</b>, named for its ability to create the illusion of Apple hardware, was developed to emulate Apple Silicon, primarily to overcome the limitation of Apple's Xcode platform, which is currently partially confined to Apple Silicon devices, with the situation unlikely to improve or be extended to legacy products. This solution allows developers to work on ARM64, albeit with expected performance trade-offs. It is not recommended for performance-intensive tasks, professional use or really anything other than educational and/or personal cyber security use only.

## M1rrage Features
Major features and support listed below
### Enhanced OS Support
M1rrage support all versions of macOS out of the box, although you will need to ensure that the operating system is compatible with chipset you're targetting in the future.
- macOS Big Sur (11.0):
  - Supported on M1 Macs
- macOS Monterey (12.0)
  - Supported on M1, M1 Pro, M1 Max, and M1 Ultra Macs
- macOS Ventura (13.0)
  - Supported on M1, M1 Pro, M1 Max, M1 Ultra, M2, M2 Pro, M2 Max, and M2 Ultra Macs
- macOS Sonoma (14.0)
  - Supported on M1, M1 Pro, M1 Max, M1 Ultra, M2, M2 Pro, M2 Max, and M2 Ultra Macs
- macOS Sequoia (15.0)
  - Supported on M1, M1 Pro, M1 Max, M1 Ultra, M2, M2 Pro, M2 Max, and M2 Ultra Macs
#### Additional Features
- Faster boot times with fewer unnecessary patches compared to other emulation methods.
- Improved stability and precision in patching, reducing the need for frequent updates and adjustments.
### Better Security
- No need to disable System Integrity Protection (SIP).
- Built-in support for FileVault 2.
- Supports secure boot protocols and firmware protection.
- Allows boot device selection and supports boot hotkeys similar to a real Mac.
### Broad Software Compatibility
- Kexts and firmware drivers, such as APFS support and FileVault, are integrated, enhancing compatibility and ease of use.
- No need for complex workarounds, as many patches are natively supported.
## OpenCore Integration
- M1rrage uses a mix of OpenCore and custom ARM64-specific patches to emulate the Apple Silicon environment effectively.
- Quirks from OpenCore ensure proper handling of SMBIOS and ACPI data for a more seamless multiboot experience.
## Does M1rrage support Windows/Linux booting?
OpenCore will automatically detect Windows without any additional configuration. With OpenCore 0.7.3, OpenLinuxBoot was added to OpenCore as an EFI driver, which will automatically detect Linux partitions. This requires either ext4_x64.efi (opens new window)or btrfs_x64.efi (opens new window)depending on which format it used in your distro. For any OSes where their bootloader has an irregular path or name, you can simply add it to the BlessOverride section.
### Limitations and Considerations
- Performance is not/likely will never be on par with native Apple Silicon hardware, making it unsuitable for heavy computational tasks.
- Some legacy functionalities and certain patches from other bootloaders may not be fully supported or supported at all.

### Legal Disclaimer
M1rrage operates in a legal grey area, as it involves using macOS on non-Apple hardware, which breaches Apple's EULA. This is for educational and personal use, and users should consult legal counsel if they have concerns.

Legality of Hackintoshing
Where hackintoshing sits is in a legal grey area, mainly that while this is not illegal we are in fact breaking the EULA. The reason this is not illegal:

- We are downloading macOS from Apple's servers directly(opens new window)
- We are doing this as a non-profit organization for teaching and personal use
- People who plan to use their Hackintosh for work or want to resell them should refer to the <a href="https://en.wikipedia.org/wiki/Psystar_Corporation" target="_new">Psystar case</a> (opens new window) and their regional laws.
- While the EULA states that macOS should only be installed on real Macs or virtual machines running on genuine Macs (<a href="https://www.apple.com/legal/sla/docs/macOSBigSur.pdf" target="_new">sections 2B-i and 2B-iii</a> (opens new window)), there is no enforceable law that outright bans this. However, sites that repackage and modify macOS installers do potentially risk the issue of <a href="https://en.wikipedia.org/wiki/Digital_Millennium_Copyright_Act" target="_new">DMCA takedowns</a> (opens new window)and such.

<i><b>IMPORTANT Note</b>: This is not Legal advice, so please make the proper assessments yourself and discuss with your lawyers if you have any concerns.</I>

Use either the included ISO image for QEMU or manually place the files in your HDD's EFI folder

For quick and easy use, download the OpenCore.iso and mount the ISO file. Make sure to configure the UUID, Serial Number, Boot ROM and other parameters as included in EFI/OC/config.plist. Make sure they match the virtual machine settings as configured per your chosen emulation software.

To create your own ISO file (on Windows, tested Windows 11) first, update your parameters in /m1rrage/opencore/EFI/OC/config.plist and, once complete, download and install the Windows ADK (free), then launch command prompt and change directory to the root of the downloaded /m1rrage folder, and run,

oscdimg -m -o -u2 -udfver102 opencore my-opencore.iso

Otherwise, create a new VHD and boot into a partitioner first, mount the EFI partition, and copy the EFI folder so it looks like:

E:\EFI\{BOOT,OC}

and don't forget to modify the UUID, Serial Number, Boot ROM, and other parameters, and make sure they match the virtual machine settings as configured in your chosen emulation software.
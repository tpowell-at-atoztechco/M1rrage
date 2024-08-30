# Installing M1rrage on QEMU
So you've made it here, and a great challenge now stands before you. Use this guide to finish your quest and gain working Apple silicon-based operating software.
## New QEMU Installation
Getting started with M1rrage for QEMU is the simplest way to get started, at this point.
  1. Download: the latest stable release of M1rrage and obtain a copy of the macOS version you desire to use, preferably from Apple's servers directly.
  2. Compile m1rrage/qemu for the machine you wish to run it on
  3. Under the QEMU runtime folder, create a new virtual machine, and assign the following properties to the machine:
```vm.conf - added options
macos-uuid
macos-serial
macos-cpuarch
macos-bootrom
macos-sbk (secure boot key)
```
    Also, remmeber to verify the CPU architecture, RAM, GPU, Boot disk, HDD, and other settings are configured!
  4. When you think your configuration is ready, use
```shell (Linux & macOS)
chmod +x verify.sh
./verify.sh
```
```cmd (Windows)
./verify.bat
```
5. Use QEMU to launch your VM

# Filestructure Explanation of M1rrage/QEMU:
```m1rrage-master/QEMU/
- README.md: An overview of the project, including goals, features, and usage instructions.
- LICENSE.md: The licensing information for the project.
- manifest.json: Configuration file detailing debugging settings and any specific QEMU features being utilized.
- docs/: Documentation related to the emulation, including architecture-specific details and setup guides.
- src/: Contains all source code, split into directories based on the CPU architecture (ARM64 and x64). Each architecture has its own directory for CPU, memory, and I/O handling.
- configs/: Contains QEMU configuration files for each architecture.
- scripts/: Useful scripts for building, running, and managing the emulation environment.
- tests/: Test cases for both ARM64 and x64 components, ensuring that the emulation behaves as expected.
- Makefile: Provides build automation, making it easy to compile and clean the project.
```

## This guide to be updated soon!
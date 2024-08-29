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

## This guide to be updated soon!

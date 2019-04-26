# Desktop High Sierra 10.13 Hackintosh


This entire config would probably work on Mojave as well but I have a Nvidia card as my primary. If i instead switched to the Intel HD 530 it would be fine.

## Hardware
* CPU - i7-6700k - 6th Gen
* RAM - 16GB - 2 Slots
* GPU - EVGA 980 TI and Intel HD 530 (Disabled in BIOS)
* Drives - Misc selection of AHCI/Sata SSD's/HDD's
* Audio - Realtek ALC1150 (Motherboard Audio)
* Motherboard - MSI B150 M3
* Ethernet - Killer E2400 (Motherboard Gigabit Ethernet port)
* WIFI/BT - Coming Soon

## Software
Used the [Vanilla guide](https://hackintosh.gitbook.io/-r-hackintosh-vanilla-desktop-guide/) and the [Internet Recovery install method](https://internet-install.gitbook.io/macos-internet-install/)

## Config.plist (Removed to protect my PC)
* Requires Serial Number (ex. DFOWQLSGH8K)
* Requires Board-ID (ex. Mac-D859C5498DA9EE9D) 

## Kext Explanation
* AppleALC - Supports the ALC1150 Audio chip
* AtherosE2200Ethernet - Supports the Killer E2400 Ethernet Port
* FakeSMC - Fakes the Mac firmware and such to the system (Always required for Hackintosh's)
* FakeSMC_CPU/GPU_Sensors - Injects the CPU and GPU Temp and Fan speed data so the mac can see it
* Lilu - Allows patching of everything in the system
* USBInjectAll - Injects all USB ports into the system (Hacky needs to be fixed properly, but fine for now)
* WhateverGreen - Plugin for Lilu that fixes various GPU releated things in the system for AMD, Intel, Nvidia
* dAGPM - Enables Nvidia and AMD HDMI Audio

## TODO
1. Install BCM943602CS PCI-E WIFI/BT card when it arrives
2. Map the USB Ports in the proper way instead of injecting them all
3. Test HDMI Audio it should work but idk

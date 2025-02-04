# OpenCore 1.0.3 Debug - macOS Sonoma 14 - Huawei Matebook D15 boh-WAP9R (Work In Progress)

```
* I am not responsible for any damage done to your device. Use at your own risk.
* Please do some research if you concerns about features included in this EFI.
* Before continuing, you are choosing to make these modifications yourself
* if any thing goes wrong, it is your responsible for the damage that happen next.
```

## Important note

#### ***Every laptop are difference, even those with the same model number. So use this EFI as a reference and edit accordingly to your own hardware.***

### You need to generate your own SMBIOS to signin with Apple ID
Use CorpNewt's [GENSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate platforminfo using `MacBookPro16,3` as an SMBIOS for Monterey. Head to [Dortania's haswell platforminfo guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#platforminfo) for in-depth guide.

### What works (Recovery)
* Recovery Booted
* Battery readout
* Keyboard
* Trackpad
* Build-in display

### What not works
* Wifi&Bluetooth

### Untested
* N/A

## Known issues
* N/A

## Bios/UEFI Settings
* N/A

## Laptop Specs/Details
* Model: Huawei Matebook D15 boh-WAP9R
* Processor:
* CPUID:
* iGPU:
* dGPU: 
* Ram: 8gb
* DRIVE1 SSD: 
* Keyboard connection type: PS/2
* Trackpad connection type: I2C
* Audio: 
* Ethernet: None
* WLAN:

## Links/Guides
* https://github.com/acidanthera/OpenCorePkg (OpenCore Bootloader)
* https://dortania.github.io/OpenCore-Install-Guide/ (OpenCore Setup,Installation,Troubleshooting)
* https://dortania.github.io/OpenCore-Post-Install/misc/rtc.html#fixing-rtc-write-issues (Wake restart fix)
* https://openintelwireless.github.io/itlwm/ (Native Intel WiFi)
* https://openintelwireless.github.io/IntelBluetoothFirmware/ (Native Intel Bluetooth)

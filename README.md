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
* Recovery WiFi connection
* Build-in display
* Keyboard
* Trackpad
* Battery readout

### What not works
* N/A

### Untested
* N/A

## Known issues
* N/A

## Bios/UEFI Settings
* N/A

## Laptop Specs/Details
* Model: `Huawei Matebook D15 boh-WAP9R`
* Processor: `17h Zen+ AMD Ryzen 7 3700U (Picasso)`
* CPUID: `AMD Ryzen 7 Mobile 3700U`
* iGPU: `AMD Radeon RX Vega 10 Graphics`
* Ram: `8gb`
* DRIVE1 SSD: `500GB NVMe`
* Keyboard connection type: `PS/2`
* Trackpad connection type: `I2C (GXTP7863@COL01)`
* Audio: `Realtek ALC256`
* Ethernet: ~~`None`~~
* WLAN: ~~`Realtek RTL8822CE`~~ `Intel(R) Wireless-AC 9560 160MHz (MVM Gen 2)`

## Links/Guides
* https://chefkissinc.github.io/guides/hackintosh/ (AMD Hackintosh guide done right)
* https://chefkissinc.github.io/applehax/nootedred (AMD iGPU Support)
* https://github.com/acidanthera/OpenCorePkg (OpenCore Bootloader)
* https://dortania.github.io/OpenCore-Install-Guide/ (OpenCore Setup,Installation,Troubleshooting)

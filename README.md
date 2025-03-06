![screenshot2568-02-16at21 09 10~2](https://github.com/user-attachments/assets/4acc2268-31d2-4e1a-88f8-d3affdfec821)


# OpenCore 1.0.3 Debug - macOS Sonoma 14 - Huawei Matebook D15 boh-WAP9R

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

### What works
* Opencore Native macOS OTA Updates
* NootedRed Radeon buildin display support
* Metal 3 GPU Acceleration
* WiFi & Bluetooth connection
* Onboard Audio & Microphone
* Keyboard & Trackpad
* USB C, USB 3.0, USB 2.0
* HDMI Video output
* 3.5mm Audio input/output
* Battery read-out
* Display Brightness Control & BrightnessKeys
* Volume control keys
* Sleep & Wake
* lid Sleep

### What not works
* Internal Webcam (Recognized but not working)
* Fingerprint reader (Recognized as usb device)
* Lid wake

## Known issues
* Some App crash the entire system causing restart
* System can't handle intensive task
### AMD related issues
* Some MKL (Math Kernel Library) application: DSP,VSTs,DAW or any audio processing application, Discord voice processing, Adobe application as it uses MKL to perform graphic calculation/signel processing. (This may help [AMDFriend](https://github.com/NyaomiDEV/AMDFriend))
* Virtual Machine running off of AppleHV's framework will not work such as VirtualBox, Parallels  13.1+, Docker(Only Docker in VirtualBox or Docker Toolbox.) (Some Android VM does work)
#### AMD Vega NootedRed related issues
* Graphical artefacts and crash on Chromium (Blink engine) based application such as Chrome, Arc, Sublime Text, Canva will crash the entire system ([Workaround](https://chefkissinc.github.io/applehax/nootedred/) or use Safari)
* HDMI Audio out and Audio control

## Bios/UEFI Settings
* N/A

## Laptop Specs/Details
* Model: `Huawei Matebook D15 boh-WAP9R`
* Processor: `17h Zen+ AMD Ryzen 7 3700U (Picasso)`
* CPUID: `AMD Ryzen 7 Mobile 3700U`
* iGPU: `AMD Radeon RX Vega 10 Graphics`
* Ram: `8gb (Onboard)`
* DRIVE1 SSD: `500GB NVMe`
* Keyboard connection type: `PS/2`
* Trackpad connection type: `I2C (GXTP7863@COL01)`
* Audio: `Realtek ALC256`
* Ethernet: ~~`None`~~
* WLAN: ~~`Realtek RTL8822CE`~~ `Intel Dual Band Wireless AC 3160`

## Links/Guides
* https://chefkissinc.github.io/guides/hackintosh/ (AMD Hackintosh guide done right)
* https://chefkissinc.github.io/applehax/nootedred (AMD iGPU Support)
* https://github.com/acidanthera/OpenCorePkg (OpenCore Bootloader)
* https://dortania.github.io/OpenCore-Install-Guide/ (OpenCore Setup,Installation,Troubleshooting)

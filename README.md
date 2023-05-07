# Hackintosh OpenCore Lenovo L380 20M6
Opencore for Lenovo L380 (updated to Ventura)
# Specification
- Brand: Lenovo Thinkpad.
- Model: L380 (20M6).
- CPU: Intel i5-8250U (Kaby Lake R) 1.6-3.4 GHz - Intel UHD 620 - 2048MB.
- RAM: SAMSUNG 16GB x 1 (2400 MHz).
- SSD: 256GB WD WDS500G2B0C-00PXH0.
- Wi-Fi: Replaced by BCM94360NG.
# Installation
## Note Before using this pre-make OpenCore
1. Double-check the specification.
2. Some components wouldn't work because I changed them like add an NVME SSD and replace the original Wi-Fi card with BCM94360NG.
## How to install
1. Download pre-build macOS Vanilla Installer on [Olarila Forum](https://www.olarila.com) and create USB Installer
2. Download this repository and extrac its content. Copy/Replace EFI folder to USB's EFI folder.
3. Please change the SMBIOS information by using GenSMBIOS [here](https://github.com/corpnewt/GenSMBIOS). Tutorial? Check [this one](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#platforminfo) and focus on platforminfo. Save all changes to config.plist file in EFI/OC folder.
4. Configuation on BIOS:
   + Turn off Secure Boot, Intel Guard Extension.
   + Pre-Memory VRAM = 512 MB
5. Press Enter to Pause Boot Screen and F12 to enter Boot Menu and select Booting form USB.
# Gigabyte-B660M-GAMING-DDR4 Hackintosh
- Mainboard: Gigabyte B660M GAMING DDR4 (rev. 1.0)
- CPU: 12th Gen Intel(R) Core(TM) i5-12400 (F)
- RAM: DDR4 2666 32GB (16GB+16GB)
- GPU: AMD RX6600XT 8G (Sapphire)
- LAN: RTL8125 Ethernet
- Wi-Fi: BCM94360CD
- Audio: ALC897
- Generic: MacPro7.1
- macOS: Monterey
- BASE EFI: OpencCore 9.8
# ACPI
- SSDT-PLUG-ALT.aml
- SSDT-EC-USBX.aml
- SSDT-RTCAWAC.aml
- SSDT-USB-Reset.aml
- FixShutdown-USB-SSDT.aml
# Drivers
- HfsPlus.efi
- OpenRuntime.efi
- ResetNvramEntry.efi
- ToggleSipEntry.efi
- OpenCanopy.efi
# Tools
- OpenShell.efi
- ResetSystem.efi
- CFGLock.efi
- VerifyMsrE2.efi
# Kexts
- Lilu
- VirtualSMC
  + SMCProcessor
  + SMCSuperIO
- SMCRadeonGPU
- RadeonSensor
- WhateverGreen
- AppleALC
- NVMeFix
- LucyRTL8125Ethernet.kext
- RestrictEvents
- USBPorts660M (USBInjectAll)

# BIOS Settings: 
Gigabyte B660M GAMING DDR4 (rev. 1.0) BIOS: (F28) 
### Platform Power:
* ErP: **Disable**
* Power Loading: **Enabled**
### IO Ports:
- Initial Display Output: **PCle 1 Slot**
- Above 4G Decoding: **Enabled**
- Above 4G MMIO BIOS assignment: **Disabled** (Will cause the issue with and sleep)
- Super IO Configuration -> Serial Port: **Disabled** (Will cause the issue with Apple Watch unlock)
- USB Configuration:
  + XHCI Hand-off -> **Enabled**
  + Legacy USB Support -> **Enabled**
  + USB Mass Storage Driver Support -> **Enabled**
  + Port 60/64 Emulation -> **Disabled**
- Network Stack Configuration
  + Network Stack: **Disabled**
### Miscellaneous:
- Intel Platform Trust Technology (PTT): **Disabled**
- Vt-d: **Enabled**
### Boot:
- CFG Lock: **Disabled**
- Fast Boot: **Disable Link**
- Windows 10 Features: **Windows 10**
- CSM Support: **Disabled**
- Secure Boot: **Disabled** (Secure Boot will be disabled by default, but good to check)
# CPU Power Management
CPU power management is handled with 'CPUFriend and CPUFriendDataProvider for SMBIOS MacPro7, 1'.If you have CPU Geekbench score is lower than me, please check your
BIOS configuration.

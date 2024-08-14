# ASUS TUF GAMING A520M PLUS 2 + RYZEN 5 5500 + RX 6600 

![about-12 3 1](https://user-images.githubusercontent.com/23700365/161353027-9aaeddf5-7457-49a8-b322-4e99ab94c679.png)

**Latest working macOS**: 14.6.1
<br>
**Current OpenCore**: 1.0.1

## Complete hardware specs
- AMD Ryzen 5 5500 Sixcore Processor
- ASUS TUF GAMING A520M-PLUS-2 (BIOS: 3607)
- ASROCK RX 66000 CLD 8GB 
- 2x 16Gb DDR4 3200Mhz 

## What works
- Audio
- HDMI/DP
- All USB ports
- Everything iCloud related (Drive, iMessage, Facetime, etc)
- Shutdown/Reboot/Update to newer macOS builds over time

## What doesn't work
- It works, but you'll need to click the power button on your PC to wake it up! (mouse or keyboard clicks do not work)

## Kexts used:
- AMDRyzenCPUPowerManagement.kext
- AppleALC.kext
- AppleMCEReporterDisabler.kext
- Lilu.kext
- NVMeFix.kext (only if you have NVME storage in your build)
- USBMap.kext (Do it yourself, every desktop needs its own USB mapping!)
- RealtekRTL8111.kext
- RestrictEvents.kext
- SMCAMDProcessor.kext
- VirtualSMC.kext
- WhateverGreen.kext

## SSDTs used:
- Do your own SSDT search, it could be different for every setup!

## Extras (It's not just especially for this setup):
- Discord crashes or mic failure:
	- See this video: (https://www.youtube.com/watch?v=odYcvq-iTGg&lc=Ugwmaet9MEjL90f9ZAx4AaABAg.A75qVL2svqnA7756I1FDYq)
	- Disable Advanced Voice Detection in Discord Voice/Video Settings
	- Disable noise suppression in discord voice/video settings
- macOS becomes slow when formatting ssd/hd in exFAT
	- In your bios, disable the HOT PLUG function, you can find this option in the sata settings section

## Thanks/Credits
- [Opencore Team](https://dortania.github.io/getting-started/)
- [BASE EFI - for AMD Ryzen and Threadripper](https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER-PUBLIC)
- Gabriel Luchina and his magical teachings!

## Discord - Universo Hackintosh - Join our community!
- [Access Discord](https://discord.universohackintosh.com.br)

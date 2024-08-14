# ASUS TUF GAMING A520M PLUS 2 + RYZEN 5 5500 + RX 6600 

![about-12 3 1](https://github.com/user-attachments/assets/566c877d-b08c-4e5c-8694-0d521199d2d0)



⚠ UTILIZE APENAS COMO PESQUISA, NÃO CARREGUE ESSA EFI EM SEU DISPOSITIVO, CADA CONFIGURAÇÃO PRECISA TER SUA PRÓPRIA EFI CRIADA DO ZERO!
⚠ USE AS RESEARCH ONLY, DO NOT LOAD THIS EFI ON YOUR DEVICE, EACH CONFIGURATION NEEDS TO HAVE ITS OWN EFI CREATED FROM SCRATCH!
**Latest working macOS**: 14.6.1
<br>
**Current OpenCore**: 1.0.1

## 💻 Complete hardware specs
- AMD Ryzen 5 5500 Sixcore Processor
- ASUS TUF GAMING A520M-PLUS-2 (BIOS: 3607)
- ASROCK RX 66000 CLD 8GB 
- 2x 16Gb DDR4 3200Mhz 

## ✅ What works
- CPU Power Management
- Graphics acceleration (RX 6600 is native for macOS)
- Ethernet (since first install)
- Digital Rights Management (Netflix, Max, Disney+, Apple TV+ etc)
- Audio
- HDMI/DP (two monitors)
- All USB ports
- Everything iCloud related (Drive, iMessage, Facetime, etc)
- Shutdown/Reboot/Update to newer macOS builds over time
- Sleep (It works, but you'll need to click the power button on your PC to wake it up! (mouse or keyboard clicks do not work)

## ❌ What doesn't work
- Virtualization (only for Intel)
- Wifi, Bluetooth and Airdrop (because I don't have a wifi card)

## 🔐 SMBIOS
- SMBIOS iMacPro1,1 (used in this efi)
- Use GenSMBIOS to generate your own unique SMBIOS for your machine
- Every setting should have this and it's different for everyone

## Kexts used:
- AMDRyzenCPUPowerManagement.kext
- AppleALC.kext
- AppleMCEReporterDisabler.kext
- Lilu.kext
- NVMeFix.kext (only if you have NVME storage in your build)
- USBMap.kext (Do your own, every desktop needs its own USB mapping!)
- RealtekRTL8111.kext
- RestrictEvents.kext
- SMCAMDProcessor.kext
- VirtualSMC.kext
- WhateverGreen.kext


## SSDTs used:
- Do your own SSDT search, it could be different for every setup!

## 

## Extras (It's not just especially for this setup):
- Discord crashes or mic failure:
	- See this video: (https://www.youtube.com/watch?v=odYcvq-iTGg&lc=Ugwmaet9MEjL90f9ZAx4AaABAg.A75qVL2svqnA7756I1FDYq)
	- Disable Advanced Voice Detection in Discord Voice/Video Settings
	- Disable noise suppression in discord voice/video settings
![about-12 3 1](https://github.com/user-attachments/assets/a97aaef2-d910-4e01-97d5-beaf2c018013)
- macOS becomes slow when formatting ssd/hd in exFAT
	- In your bios, disable the HOT PLUG function, you can find this option in the sata settings section

## Thanks/Credits
- [Opencore Team](https://dortania.github.io/getting-started/)
- [BASE EFI - for AMD Ryzen and Threadripper](https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER-PUBLIC)
- Gabriel Luchina and his magical teachings!

## Discord - Universo Hackintosh - Join our community!
- [Access Discord](https://discord.universohackintosh.com.br)

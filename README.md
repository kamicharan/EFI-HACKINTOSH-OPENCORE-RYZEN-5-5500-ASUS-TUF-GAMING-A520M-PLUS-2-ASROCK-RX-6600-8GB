# ASUS TUF GAMING A520M PLUS 2 + RYZEN 5 5500 + RX 6600 

![about-12 3 1](https://github.com/user-attachments/assets/566c877d-b08c-4e5c-8694-0d521199d2d0)



🔴 UTILIZE APENAS COMO PESQUISA, NÃO CARREGUE ESSA EFI EM SEU DISPOSITIVO, CADA CONFIGURAÇÃO PRECISA TER SUA PRÓPRIA EFI CRIADA DO ZERO!

🔴 USE AS RESEARCH ONLY, DO NOT LOAD THIS EFI ON YOUR DEVICE, EACH CONFIGURATION NEEDS TO HAVE ITS OWN EFI CREATED FROM SCRATCH!

**Latest working macOS**: 14.6.1
<br>
**Current OpenCore**: 1.0.1

## 💻 Complete hardware specs
- CPU: AMD Ryzen 5 5500 Sixcore Processor
- MOTHERBOARD: ASUS TUF GAMING A520M-PLUS-2 (BIOS: 3607)
- RAM: 2x 16GB DDR4 3200MHZ
- GPU: ASROCK RX 6600 CLD 8GB GDDR6
- SSD 1#: KINGSTON SNV2S1000G (PCI-Express) - NVME SLOT
- SSD 2# KINGSTON SA400S37480G (PCI) - SATA SLOT
- ETHERNET: Realtek RTL8111 PCI Express Gigabit
- AUDIO: Realtek ALC897


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

## 🔴 Information about CPU Cores (IMPORTANT!) 🔴
- In AMD we need to mapp cores for our CPUs or the installation will not even began
- You can learn about this in this repository (but I highly recommend watching Gabriel Luchina's full broadcasts from the Universo Hackintosh channel on youtube!): https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER-PUBLIC

## 🔐 Bios Settings:
⛔ Disable this:
- Serial Port (Advanced Settings>Onboard Devices Configuration>Serial Port Configuration)
- SMV Mode (Advanced Settings>CPU Configuration)
  - Obs: Only if you don't use virtualization in windows (dual-boot)
- Hot Plugs (Advanced Settings> SATA Configuration)
  - Obs: It corrects problems when you use SATA storages in exfat 
- Compatibility Support Module or CSM (Boot>CSM)

✅ Enable this:
- Above 4G Decoding (Advanced Settings>PCI Subsystem Settings)
  - Obs: If when you disabled this, Resize BAR Support pops up, then disable it
- XHCI Hand-off (Advanced Settings>USB Configuration)
- SATA Mode AHCI (Advanced Settings>SATA Configuration)
  - Obs: Sata mode selection as AHCI

❎ OBSERVATIONS
- In this motherboard, the secure boot option is not avaliable to enable/disabled, so you have to disable the key SecureBootModel located in your config.plist in: Misc>Security>SecureBootModel=Disabled
![about-12 3 1](https://github.com/user-attachments/assets/6b955c60-f072-456f-97b6-fb109281a5f6)

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

❎ SE VOCÊ DESEJA UM HACKINTOSH LIMPO E BEM CRIADO, RECOMENDO FORTEMENTE QUE ENTRE NA COMUNIDADE UNIVERSO HACKINTOSH, SE TORNE MEMBRO DO CANAL NO YOUTUBE E SIGA COM CALMA E MUITA PACIÊNCIA OS PASSOS DE CONSTRUÇÃO DO SEU HACKINTOSH, ISSO NÃO SE FAZ DO DIA PARA A NOITE E LEVA TEMPO, DEDICAÇÃO E ESTUDO. SE VOCÊ NÃO POSSUÍ TEMPO PARA ISSO, PODE CONTRATAR O GABRIEL LUCHINA, MAIOR ESPECIALISTA EM HACKINTOSH NO BRASIL PARA UMA CONSULTORIA PROFISSIONAL QUE ABORDARÁ DESDE A ESCOLHA DAS PEÇAS ESPECÍFICAS PARA SEU USO ATÉ A INSTALAÇÃO E CONFIGURAÇÃO DA SUA EFI!

❎ IF YOU WANT A CLEAN AND WELL CREATED HACKINTOSH, I STRONGLY RECOMMEND THAT YOU JOIN THE HACKINTOSH UNIVERSE COMMUNITY, BECOME A MEMBER OF THE YOUTUBE CHANNEL AND FOLLOW THE STEPS OF BUILDING YOUR HACKINTOSH CALMLY AND WITH A LOT OF PATIENCE, THIS CANNOT BE DONE OVERNIGHT AND IT TAKES TIME, DEDICATION AND STUDY. IF YOU DON'T HAVE TIME FOR THIS, YOU CAN HIRING GABRIEL LUCHINA, THE LARGEST HACKINTOSH SPECIALIST IN BRAZIL FOR A PROFESSIONAL CONSULTANCY THAT WILL COVER FROM THE CHOICE OF SPECIFIC PARTS FOR YOUR USE TO THE INSTALLATION AND CONFIGURATION OF YOUR EFI!

You can acess our discord server in the link below:

## Discord - Universo Hackintosh - Join our community!
- [Access Discord](https://discord.universohackintosh.com.br)

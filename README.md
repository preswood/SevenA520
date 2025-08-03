#### Notice 02/05/2025: this project has been renamed from SevenA520 to Seven500.
# SEVEN500 - Running Windows 7 on A520, B550 and X570

## About
*Seven500* is a project that provides the necessary software to get Windows 7 running on AMD AM4 500 chipsets. Note that the drivers and installers included are **NOT** developed by me. Some people use Windows 7 for the vibes, others **need** it to run software that won't work on newer systems such as medical staff or accountants. No matter what you wish to do, this project is here to do its best to help you.

## Requirements (DO NOT SKIP)
It is absolutely crucial that you have:

- a copy of Windows 7 on a **DVD** (AMD 500 USB ports don't work on Windows 7 out of the box)
- a SATA DVD reader (again, USB doesn't work)
- a PS/2 mouse or keyboard
- a motherboard with CSM enabled
- a SATA HDD/SSD (PCI-E and NVM-E drives might work but you'll run into a myriad of problems)

## 1 - Check if your motherboard has a PS/2 port
Given the age difference between Windows 7 and the AMD 500 chipsets USB ports are a no-go. As such if your machine does not have at least one PS/2 port it may become impossible to install and use Windows 7. The rest of the readme assumes that you only have a PS/2 keyboard, however if you also / only have a PS/2 mouse you can still follow the instructions.

## 2 - Check if your graphics device is supported
> [!NOTE]
> If your device isn't listed consult the manufacturer's website (AMD/NVIDIA)

Before you try and install Windows 7 on your A520 system please make sure your hardware is compatible, specifically your GPU or iGPU:

### AMD/ATI Graphics (Radeon)
- [ ] AMD Radeon RX 9000
- [ ] AMD Radeon 800M iGPUs
- [ ] AMD Radeon 700M iGPUs
- [ ] AMD Radeon RX 7000
- [ ] AMD Radeon 600M iGPUs
- [ ] AMD Vega iGPUs (Ryzen 3000/4000/5000)
- [X] AMD Radeon RX 6000
- [X] AMD Vega iGPUs (Ryzen 2000 / Athlon Zen)
- [X] AMD Radeon RX 5000
- [X] AMD Radeon RX 500
- [X] AMD Radeon RX 400
- [X] AMD Radeon RX 300
- [X] AMD Radeon RX 200
- [X] AMD Radeon HD 7000 / HD 8000
- [X] AMD Radeon HD 6000
- [X] ATI Radeon HD 5000
- [X] ATI Radeon HD 4000
- [X] ATI Radeon HD 3000
- [X] ATI Radeon HD 2000
- [X] ATI Radeon X1000 / X800 / X700 (PCIe)
- [ ] ATI Radeon X1000 / 8000 / X700 (AGP)
- [ ] ATI Radeon 9000 and older
- [ ] Other ATI AGP cards

### NVIDIA Graphics (GeForce)
- [ ] NVIDIA GeForce RTX 50
- [ ] NVIDIA GeForce RTX 40
- [X] NVIDIA GeForce RTX 30
- [X] NVIDIA GeForce RTX 20 / GTX 16
- [X] NVIDIA GeForce GTX 10
- [X] NVIDIA GeForce GTX 900
- [X] NVIDIA GeForce GTX 700
- [X] NVIDIA GeForce GTX 600
- [X] NVIDIA GeForce GTX 500
- [X] NVIDIA GeForce GTX 400
- [X] NVIDIA GeForce GTX 300
- [X] NVIDIA GeForce GTX 200
- [X] NVIDIA GeForce 10
- [X] NVIDIA GeForce 9
- [X] NVIDIA GeForce 8
- [X] NVIDIA GeForce 7 (PCIe)
- [ ] NVIDIA GeForce 7 (AGP/PCI)
- [X] NVIDIA GeForce 6 (PCIe)
- [ ] NVIDIA GeForce 6 (AGP/PCI)
- [ ] NVIDIA GeForce 5 and older
- [ ] Other NVIDIA AGP cards

## 3 - Installing Windows 7
It is absolutely crucial that you install an ***x64*** version of ***STOCK*** Windows 7. No bootlegs. No modded versions. Just bog standard Windows 7. Here is a list of tested versions that should work just fine:

- Windows 7 Ultimate SP1
- Windows 7 Professional SP1
- Windows 7 Home Premium SP1
- Windows 7 Enterprise SP1

If you don't have a copy of Windows 7 you can download it from [here](https://massgrave.dev/windows_7_links).
If you don't have a mouse remember that you can still use TAB to navigate through both the installer and Windows in general.

## 4 - Installing drivers
Download, copy and extract the zip included in the release files from another OS (Linux on a USB, Windows on another drive, etc) onto the new Windows 7 drive. You can place it anywhere but for convenience it's best to place it into Windows 7's "C:" drive. Once you've done that we'll get Windows 7 ready for the driver installations.

### 

### 4.2 - WUFUC
Before you update Windows using the included update file you must first run **wufuc.exe*** to disable the CPU check. This is because the windows update we need checks your CPU before installing and because it doesn't recognise Ryzen CPUs it halts and gives errors. To bypass this you must install wufuc. You can find the executable in the extracted folder.

### 4.3 - 

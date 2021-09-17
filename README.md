Resources for HP Probook 430 G3 to run macOS
============================================

- Bootloader version: Opencore 0.7.3
- macOS version: macOS Big Sur 11.6 (20G165)
- Windows version: Windows 11 Insider Preview Build 22000.194 for the Beta Channel
![Oops!There was supposed to be an image here](https://i.imgur.com/33J0ITE.png)
![Oops!There was supposed to be an image here](https://i.imgur.com/evyClZk.png)
![Oops!There was supposed to be an image here](https://i.imgur.com/EAKVfPD.png)

#### What works
- iGPU acceleration (Intel HD 520)
- Sleep
- Battery Percentage
- Display Brightness
- USB ports
- Internal Camera
- Audio with mute button (Both internal speakers and Microphone) (cx20724)
- Native Power Management/(Also with cpufriend)
- SMBus Controller
- CPU Temperature Monitoring
- Fan Speed Monitoring
- VGA (*suprisingly*)
- Boot Chime
- Dualbooting with Windows 11 Insider Preview Build 22000.194 for the Beta Channel
- iMessage
- Facetime

#### What doesn't work
- Built-In Wifi+Bluetooth (*unsupported*)

#### Specs

| Component      | Brand                                                            |
|----------------|------------------------------------------------------------------|
| **CPU**        | `Intel Core i5-6200U ` |   
| **iGPU**       | `Intel HD Graphics 520 `                                         |
| **Audio**      | `Conexant 20724 - layout 3`                                      |
| **Ethernet**   | `Realtek RTL8111/8168`                                           |
| **OS**         | `macOS Big Sur 11.6 (20G165)` and `Windows 11 Insider Preview 22000.194 for the Beta Channel`|

#### Not tested
- HDMI output (both audio and video)
- RTS522A PCI Express Card Reader
- (*Ideally both should work, If some is willing to test, create an issue*)

#### To Do
- ~~Add pci devices in system information~~  *done*
- macOS Powerchime (*I don't know what I will do, if you have any suggestions,create an issue*)
- ~~Real Time Clock Loss (RTC)~~ *done*
- ~~Battery Cycle count~~ *Fixed by updating to the Latest Bios*
- ~~Fan Speed Monitoring~~ *done*
- Let me know more 

#### Benchmarks
- Geekbench 5 [Multi-core and Single core](https://browser.geekbench.com/v5/cpu/8013906)

#### Important
- In the config.plist, section `PlatformInfo > Generic`, the following fields are currently edited with CHANGEME. Please generate your own serial. 

- This repo can be helpful for other HP Probook/Elitebook series notebooks
 
### Bios Configuration


#### Enable

- Fast Boot
- Runtime Power Management
- Extended Idle Power States
- Deep Sleep
- Power Control
- Turbo Boost
- Virtualization Technology (VTx)
- Hyperthreading
- Multi Processor

 #### Disable
 
- Legacy boot
- Wake when lid is opened
- Wake on USB

#### Having some problem
Create an issue and I'll try to help as many as I can

#### Credits
- [Apple](https://apple.com) for [macOS](https://www.apple.com/macos/big-sur/)
- [Acidanthera](https://github.com/Acidanthera) for [OpenCorepkg](https://github.com/acidanthera/OpenCorePkg) and necessary kexts
- [dortania](https://github.com/dortania) for its detailed guides
- [Corpnewt](https://github.com/CorpNewt) for [USBMap](https://github.com/corpnewt/USBMap)

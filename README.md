# macOS-HP-Probook-430-G3-Resources
Resources for HP Probook 430 G3 to run macOS
============================================

-Bootloader version:Opencore 0.6.9
-macOS version:macOS Big Sur 11.3.1 Release
![Oops!There was supposed to be an image here](https://user-images.githubusercontent.com/84245065/119499806-b8e0b900-bd84-11eb-8607-9476fbbfde9d.png)

![Oops!There was supposed to be an image here](https://user-images.githubusercontent.com/84245065/119499843-c26a2100-bd84-11eb-8bc7-a26cf0b433c4.png)

![Oops!There was supposed to be an image here](https://user-images.githubusercontent.com/84245065/119499872-c8600200-bd84-11eb-8485-282e9efa092c.png)


####What works
- iGPU acceleration (Intel HD 520)
- Sleep
- Battery Percentage
- Display Brightness
- USB ports
- Internal Camera
- Audio with mute button (Both internal speakers and Microphone) (cx20724)
- Native Power Management/(Also with cpufriend)
- VGA(*suprisingly*)
- Dualbooting with Windows10(21H1)

####What doesn't work
- Built-In Wifi+Bluetooth(*unsupported*)
- iMessage and Facetime (*May work for you as it is smbios related*)

#### Specs

| Component      | Brand                                                            |
|----------------|------------------------------------------------------------------|
| **CPU**        | `Intel Core i5-6200U (2.4 GHz, up to 3 GHz 3 MB cache, 2 cores)' |   
| **iGPU**       | `Intel HD Graphics 520 `                                         |
| **Audio**      | `Conexant 20724 - layout 3`                                      |
| **Ethernet**   | `Realtek RTL8111/8168`                                           |
| **WiFi Card**  | `Realtek (Unsupported)`                                          |
| **OS**         | `macOS Big Sur 11.3.1`                                           |

####Not tested
- HDMI output(both)
- RTS522A PCI Express Card Reader
(*Ideally both should work,If some is willing to test,create an issue*)

####To Do
- ~~Add pci devices in system information~~ *done*
- Battery cycle count
- macOS Powerchime(*I don't know what I will do,if you have any suggestions,create an issue*)

####Benchmarks
- Geekbench 5 [Multi-core and Single core] (https://browser.geekbench.com/v5/cpu/8013906)

####Important
- In the config.plist, section `PlatformInfo > Generic`, the following fields are currently edited with CHANGEME. Please  generate your own serials. 
 - `MLB`
  - `ROM`
  - `SystemSerialNumber` 
  - `SystemUUID`

-This repo can be helpful for other HP Probook/Elitebook series notebooks

####Having some problem
Create an issue and I'll try to help as many as I can.

####Credits
- [Apple](https://apple.com) for [macOS] (https://www.apple.com/macos/big-sur/)
- [Acidanthera](https://github.com/Acidanthera) for [OpenCorepkg] (https://github.com/acidanthera/OpenCorePkg) and necessary kexts
- [dortania](https://github.com/dortania) team for its detailed guides
- [Corpnewt](https://github.com/CorpNewt) for [SSDTTime] (https://github.com/corpnewt/SSDTTime) and [USBMap] (https://github.com/corpnewt/USBMap)

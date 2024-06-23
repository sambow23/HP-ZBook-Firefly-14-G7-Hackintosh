# HP ZBook Firefly 14 G7
<img src="https://i.imgur.com/c63OLOQ.png" width="500">

Specs:
---

- **CPU** : Intel® Core™ i7-10610U @ 4.90 GHz
- **RAM** : 16GB dual-channel 2667MHz DDR4
- **GPU** : Intel UHD Graphics 630
- **dGPU** : NVIDIA Quadro P520 Max-Q 4GB
- **Storage** : ADATA SX8100NP 512GB NVME SSD
- **Screen** : 14" 1920x1080 Touchscreen
- **WiFi** : Intel® Wi-Fi 6 AX201
- **Soundcard** : Realtek ALC285

## Hardware compatibility

#### What works
- CPU power management
- GPU acceleration and video codecs
- SSD (SATA/NVME)
- Wi-Fi (itlwm)
- All USB ports
- USB-C Video
- Touchscreen (with gestures)
- Trackpad
- FN Keys
- Webcam
- Screen Brightness
- Internal Audio (Speakers, Headphones)
- Battery percentage
- Thunderbolt
  * Tested with a CalDigit TS3 Plus, hotplug is working.
    * The PCIe Ethernet NIC on the dock causes system instability when a Ethernet cable is plugged in, disable the NIC by putting `dk.e1000=0 e1000=0` into your boot-args.
    * The DisplayPort out has major performance issues (cursor updates at about 11fps). For some reason plugging in a USB-C to HDMI Adapter into a Thunderbolt port on the dock works fine. Possibly a firmware issue with the Thunderbolt controller?
- Closing and Waking the Internal Display


#### Untested
- iCloud Services
- Bluetooth (no kext installed yet)

#### Not working
- Sleep (Works if laptop is left idle and Power Nap is on, closing lid will induce a crash, under investigation)
  * Recommended to disable Sleep with `sudo pmset -a disablesleep 1` otherwise the system will freeze when closing the lid
- Facial Recognition IR Camera
- Fingerprint Sensor
- NFC
- Smartcard
- Internal Microphone
- HDMI Out
  * Does not work under Linux/macOS because of HP Firmware issues.
- dGPU (disabled)

## Tested/Working macOS Versions
- macOS Big Sur
- macOS Sonoma

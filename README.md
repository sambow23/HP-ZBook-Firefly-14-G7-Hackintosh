# HP ZBook Firefly 14 G7 (WIP)

Specs:
---

- **CPU** : Intel® Core™ i7-10610U @ 4.90 GHz
- **RAM** : 16GB dual-channel 2667MHz DDR4
- **GPU** : Intel UHD Graphics 630
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
  * Tested with a CalDigit TS3 Plus, hotplug is working to some extent
    * PCIe Ethernet sometimes causes kernel panics
    * The DisplayPort out has major performance issues (cursor updates at about 11fps)
- Closing and Waking the Internal Display


#### Untested
- iCloud Services
- Bluetooth (no kext installed yet)

#### Not working
- Sleep (will never work, no S3 support)
- Facial Recognition IR Camera
- Fingerprint Sensor
- NFC
- Smartcard
- Internal Microphone
- HDMI Out
  * Unsure why, the USB-C video outs work fine

## Tested/Working macOS Versions
- macOS Big Sur
- macOS Sonoma

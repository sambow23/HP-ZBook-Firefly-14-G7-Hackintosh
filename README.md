# HP ZBook Firefly 14 G7
<img src="https://i.imgur.com/c63OLOQ.png" width="500">

| Hardware  | |
| ------------- | ------------- |
| CPU  | Intel® Core™ i7-10610U |
| RAM  | 16GB DDR4 (Soldered) |
| GPU  | Intel UHD Graphics 630  |
| dGPU  | NVIDIA Quadro P520 Max-Q 4GB  |
| Network  | Intel® Wi-Fi 6 AX201 |
| Storage  | SAMSUNG 980 PRO SSD 2TB |
| OS  | NixOS, macOS Sequoia 15.1, Windows 11 24H2 LTSC |
| Screen  | 14" 1920x1080 Touchscreen |
| Bootloader | Uses [Super-UEFIinSecureBoot-Disk](https://github.com/ValdikSS/Super-UEFIinSecureBoot-Disk) 

## Hardware compatibility

#### What works
- CPU power management
- GPU acceleration and video codecs
- SSD (SATA/NVME)
- Wi-Fi (AirportItlwm.kext)
- All USB ports
- USB-C Video
- Touchscreen
- Trackpad
- FN Keys
- Webcam
- Screen Brightness
- Internal Audio (Speakers, Headphones)
- Battery percentage
- Thunderbolt
- Sleep
  - Uses Deep Idle instead of S3, blame HP not me :)

#### Untested
- iCloud Services
- Bluetooth (no kext installed)

#### Not working
- Facial Recognition IR Camera
- Fingerprint Sensor
- NFC
- Smartcard
- Internal Microphone
- HDMI Out
  * Does not work due to missing HDMI functionality in the ICL driver.
- dGPU (disabled)

## Tested/Working macOS Versions
- macOS Big Sur
- macOS Sonoma

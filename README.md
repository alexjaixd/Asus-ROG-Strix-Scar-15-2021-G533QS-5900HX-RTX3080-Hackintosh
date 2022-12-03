# Asus-ROG-Strix-Scar-15-2021-G533QS-5900HX-RTX3080-Hackintosh
Documentation of Asus ROG Strix Scar 15 2021 G533QS 5900HX RTX3080 Hackintosh

**Brief Overlook**

This repository is for the documentation of installing Mac OS on to an 2021 Asus ROG Strix Scar 15 (G533QS) with Ryzen 9 5900HX & RTX3080 laptop GPU. Both the AMD iGPU and RTX3080 **DOES NOT** work at the time of writing, so don't expect Graphics Acceleration anytime soon. However, contratry to popular opinions, the laptop 5900HX does work with a custom SSDT-CPUR patch. CPU Performance is also quite fast and capable of normal tasks (browsing, watching videos, office tasks, etc...) Just don't expect any GPU performance with no hardware acceleration. **This is very much only a proof of concept.**

So if you have a laptop with 5900HX and is not a Strix Scar 15, this EFI might or might not work for you. But you're welcomed to try and see for yourself.

**Current Booted Version** :Opencore 0.8.5

**Current Status** :Alpha build WIP (needs a lot of development)

**Supported OS** :
- Catalina (MacOS recognises all 8 CPU cores)
- Big Sur (Boots, only recognises as 1 CPU core)
- Monterey (Boots, only recognises as 1 CPU core)
- Ventura (Boots, only recognises as 1 CPU core)

![screenshot blurred serial](https://user-images.githubusercontent.com/86264021/205434871-ed1778d4-db22-4987-a30f-c959720916ca.png)

Machine Specs:
- CPU: AMD Ryzen 9 5900HX
- iGPU: AMD Cezanne [Radeon Vega Mobile]
- dGPU: RTX3080 Laptop GPU GA104M
- RAM: 32GB 3200MHZ DDR4
- Wifi & BT: Intel Killer AX1675X (AX210 chipset) (self replaced)

What's working:
- Intel Wifi & Bluetooth (Airportitlwm) 
- Keyboard (works but problematic)
- Volume hotkeys
- USB Ports
- Internal Speakers ALC285 (with Fuzzy blurred Noises)

What's not working:
- GPU acceleration
- Trackpad (Trackpads on AMD chipset is very complicated)
- Brightness Control (no gpu accel, no brightness control)
- Keyboard backlight always on 
- Battery Status

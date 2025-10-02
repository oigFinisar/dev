---
layout: instrument
title: WaveMaker
---

# Getting Started

This page helps you to get started with your WaveMaker.

For more information, visit the [WaveMaker Page](https://www.coherent.com/networking/optical-instrumentation/wavemakers) on our website.

## Requirements

To get started with your WaveMaker, you will need:

- 1x WaveMaker
- 1x Ethernet or USB cable
- 1x power cable
- 1x PC or laptop (not supplied)

## System

- Google Chrome, Mozilla Firefox, or Microsoft Edge browser
- Operating System: Windows 10 or above
- mDNS support (e.g. Bonjour on Windows)

# Connecting to the WaveMaker

## Connect via USB (Recommended)

1. Connect WaveMaker to a PC via USB.
2. Turn on WaveMaker.
3. Wait 5 minutes for startup.
4. Go to the device webpage in the browser. The serial number can be found on the device.
   - mDNS: [http://{SERIAL_NUMBER}.local]()
   - USB: [http://192.168.6.8](http://192.168.6.8)

## Connect via Ethernet (LAN)

### Option 1: Dynamic IP Address (DHCP Server Available)

After startup, the WaveMaker will look for a DHCP server. If your network provides a DHCP server, the WaveMaker will receive its IP address automatically.

1. **Optional**. If you are unsure if the WaveMaker is in its factory setting:
   - Turn the WaveMaker on and wait for 2 minutes.
   - Use a small screwdriver to press the "RESET" button on the rear panel of the WaveMaker for 10 seconds.
   - Turn the WaveMaker off.
2. Connect WaveMaker to the LAN socket or router.
3. Turn on WaveMaker. If the WaveMaker was turned on when you connected the cable, make sure to power-cycle the WaveMaker to trigger DHCP discovery.
4. Wait 5 minutes for startup.
5. Go to the device webpage in the browser. The serial number can be found on the device.
   - mDNS: [http://{SERIAL_NUMBER}.local]()
   - Dynamic IP: [http://{IP_ADDRESS}]()

### Option 2: Fixed IP Address / Direct Connection

If there is no response from a DHCP server, the WaveMaker will fall back to using a fixed IP address (factory default: [http://169.254.6.8](http://169.254.6.8)). Alternatively, if you make a direct connection to your PC using an Ethernet cable, the WaveMaker will use its fixed IP address.

1. **Optional**. You need to connect to the WaveMaker using the factory setting once in order to reassign the fixed IP address.
2. Connect WaveMaker to the LAN socket or router or PC via Ethernet.
3. Turn on WaveMaker. If the WaveMaker was turned on when you connected the cable, make sure to power-cycle the WaveMaker to trigger DHCP discovery.
4. Wait 5 minutes for startup.
5. Go to the device webpage in the browser. The serial number can be found on the device.
   - mDNS: [http://{SERIAL_NUMBER}.local]()
   - Fixed IP: [http://{IP_ADDRESS}]()

### Option 3: Assign a new Fixed IP Address

If you would like to reassign the fixed IP address for the WaveMaker, continue with the following.

1. Open the _Tools_ page from the navigation bar.
2. Open the _Networking Configuration_ tab.
3. Follow the instructions to change the network configuration to the desired network settings.
4. Check that the WaveMaker is connected to the LAN socket or router or PC via Ethernet.
5. Power cycle the WaveMaker.
6. Wait 5 minutes for startup.
7. Go to the device webpage in the browser. The WaveMaker will now use the newly assigned fixed IP address.
   - mDNS: [http://{SERIAL_NUMBER}.local]()
   - Fixed IP: [http://{NEW_IP_ADDRESS}]()

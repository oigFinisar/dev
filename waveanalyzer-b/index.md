---
layout: instrument
title: WaveAnalyzer B-Series
---

## Software and updates

### WaveAnalyzer software

Install the WaveAnalyzer software on your PC to connect to your instrument. Requires Windows 10 or later.

[Download WaveAnalyzer software (ZIP)](https://files.finisar.com/f/268277cac276b5f7)

### WaveAnalyzer 1500B Update Package

[Download the WA1500B update package v1.1.0.1](https://files.finisar.com/f/d87dbbf59ceaf6d1)

Install this package using WaveHub. See [WaveHub downloads and update instructions]({{ '/wavehub/' | relative_url }}).

## Connect via USB (recommended)

1. Connect the WaveAnalyzer to your PC via USB.
2. Turn on the instrument.
3. Wait 2 minutes for startup.
4. Open the WaveAnalyzer software and follow the instructions.

## Connect via Ethernet (LAN)

At startup, the instrument looks for a DHCP server. If none responds, it uses a fixed IP address. The factory default is [http://169.254.12.8](http://169.254.12.8).

Choose the setup that matches your connection:

- [Network with DHCP](#network-with-dhcp): your network assigns the IP address.
- [Fixed IP address](#fixed-ip-address): you configure the IP address through USB first.
- [Direct connection](#direct-connection): you connect the instrument to your PC with an Ethernet cable.

### Network with DHCP

1. If you are unsure whether the instrument has its factory settings, reset it before connecting:
   - Turn on the instrument and wait 2 minutes.
   - Use a small screwdriver to press the "RESET" button on the rear panel for 10 seconds.
   - Turn off the instrument.
2. Connect the WaveAnalyzer to the LAN socket or router.
3. Turn on the instrument. If it was already on when you connected the cable, turn it off and on again to trigger DHCP discovery.
4. Wait 5 minutes for startup.
5. Open the WaveAnalyzer software and its connection wizard.
6. Select "Network with DHCP" and enter the serial number without the "WA" prefix when prompted.

### Fixed IP address

Configure your chosen IP address through USB before connecting via Ethernet.

1. Disconnect Ethernet and connect via USB, following the [USB instructions](#connect-via-usb-recommended) above.
2. Open [http://192.168.12.8](http://192.168.12.8) in your browser. The page shows the current network status on the left and setup on the right.
3. Click "Change" and enter your chosen address under "IP Address".
4. Disconnect USB and connect Ethernet.
5. Turn the instrument off and on again.
6. Wait 2 minutes for startup.
7. Open the WaveAnalyzer software and click "Connection Wizard".
8. Select "Network which uses static IP" and enter the fixed IP address when prompted.

### Direct connection

When connected directly to your PC with an Ethernet cable, the instrument uses its fixed IP address. The factory default is [http://169.254.12.8](http://169.254.12.8).

1. If you are unsure whether the instrument has its factory settings, reset it before connecting:
   - Turn on the instrument and wait 2 minutes.
   - Use a small screwdriver to press the "RESET" button on the rear panel for 10 seconds.
   - Turn off the instrument.
2. Connect the instrument to your PC with an Ethernet cable.
3. Turn on the instrument.
4. Wait 2 minutes for startup.
5. Open the WaveAnalyzer software. It will discover the instrument automatically.

## Product information

For more information, visit the [WaveAnalyzer product page](https://www.coherent.com/networking/optical-instrumentation/waveanalyzer).

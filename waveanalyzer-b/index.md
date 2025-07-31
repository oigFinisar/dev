---
layout: instrument
title: WaveAnalyzer B-Series

downloads:
#   - label: PDF Manual
#     url: /assets/pdfs/WaveAnalyzerB_Quickstart_Guide.pdf
#     style: pdf_download_link
#   - label: PC-Software(Windows 10+)
#     url: https://repo.coherent.com/software/waveanalyzer-1.9.0.zip
#     style: zip_download_link

---

# WaveAnalyzer B-Series - Getting Started

This page gets you started with your WaveAnalyzer.

For more information, visit the [WaveAnalyzer Page](https://www.coherent.com/networking/optical-instrumentation/waveanalyzer) on our web site.

# Software

Please install the WaveAnalyzer Software on your PC: 

[Download (ZIP file)](https://files.finisar.com/f/268277cac276b5f7)

Requirements: Windows 10 or above

# Connect via USB (Recommended)
1. Connect WaveAnalyzer to a PC via USB.
2. Turn on WaveAnalyzer.
3. Wait 2 minutes for startup.
4. Run the WaveAnalyzer Software and follow the instructions. The connection wizard will start automatically.


# Connect via Ethernet (LAN)

## Overview
- After power-up the instrument will look for a DHCP server. 
- If there is no response from a DHCP server it will fall back to a fixed IP address (factory: [http://169.254.12.8](http://169.254.12.8))

### Option 1: Dynamic IP Address (DHCP Server Available)
If your network provides a DHCP server, the instrument will receive its IP address automatically.
1. Optional: If you are unsure if the instrument is in its factory setting:
    - Turn the instrument on and wait for 2 minutes.
    - Use a screw driver to push in the "RESET" button on the backside of the instrument for 10 seconds.
    - Turn the instrument off
2. Connect WaveAnalyzer to the LAN socket or router. 
3. Turn on WaveAnalyzer (if the instrument was turned on when you connected the cable, make sure to power-cycle the instrument to trigger DHCP discovery)
4. Wait 5 minutes for startup.
5. Run the WaveAnalyzer Software. Use the connection wizard to discover the instrument. Select "Network with DHCP". You will be asked to enter the serial number (without the "WA" prefix).

### Option 2: Fixed IP Address
If there is no DHCP server the instrument will fall back to a fixed IP address. The factory setting is (factory: [http://169.254.12.8](http://169.254.12.8)).

1. You need to connect through USB once in order to configure the desired IP address: Disconnect Ethernet and connect USB. Follow the instructions under "Connect via USB".
2. Open a web browser and go to [http://192.168.12.8](http://192.168.12.8). You should see a web page with the current network status (left) and the setup (right).
3. Click on "Change" and enter your IP address under "IP Address".
4. Disconnect USB and connect Ethernet.
5. Power-cycle the instrument.
6. Wait 2 minutes for startup.
7. Run the WaveAnalyzer Software. Click on "Connection Wizard". Select "Network which uses static IP". You will be asked to enter the fixed IP address.

### Option 3: Direct Connection
If you make a direct connection to your PC using an Ethernet cable, the unit will use its fixed IP address (factory: [http://169.254.12.8](http://169.254.12.8)).

1. Optional: If you are unsure if the instrument is in its factory setting:
    - Turn the instrument on and wait for 2 minutes.
    - Use a screw driver to push in the "RESET" button on the backside of the instrument for 10 seconds.
    - Turn the instrument off
2. Connect the instrument using an Ethernet cable
3. Turn the instrument on.
4. Wait 2 minutes for startup.
5. Run the WaveAnalyzer Software. The instrument will be automatically discovered.

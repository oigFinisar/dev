---
layout: instrument
title: WaveMaker
header_logo: WaveMaker4000A.png
---

[Homepage](https://www.coherent.com/networking/optical-instrumentation/wavemakers)

# Prerequisites
- To get started with the WaveMaker, you will need:
  - 1x WaveMaker
  - 1x Ethernet or USB cable
  - 1x power cable
  - 1x PC or laptop (not supplied)

# Connect via Local Area Network

- Connect the Ethernet cable from the WaveMaker to a network switch or wall socket port within the same subnet as the PC.
- Connect the power cable from the WaveMaker to a mains power inlet.
- Switch on the WaveMaker power from the rear panel. The front panel indicator LED should now turn orange/red to indicate that the device is OFF.
- Turn the key to the ON position from the front panel. The front panel indicator LED should now turn green to indicate that the device is ON.
- Wait at least five minutes for the device to warm up.
- Open a web browser on the PC.
- Navigate to the following web page.
  - mDNS: {serial number}.local
  -  DHCP: IP address automatically assigned by the DHCP server
  -  Fixed IP (Ethernet): 169.254.6.8 (default)
  -  Fixed IP (USB): 192.168.6.8 (default)
- The WaveMaker can now be controlled using the web interface.

# Connecting via Direct Connection
- Connect the Ethernet or USB cable from the WaveMaker directly to a PC.
- Connect the power cable from the WaveMaker to a mains power inlet.
- Switch on the WaveMaker power from the rear panel. The front panel indicator LED should now turn orange/red to indicate that the device is OFF.
- Turn the keylock switch to the ON position from the front panel. The front panel indicator LED should now turn green to indicate that the device is ON.
- Open the network settings on the PC. The network adapter for the WaveMaker should appear in the adapters list after a short time.
- Configure the IPv4 properties of the network adapter. The recommended settings are as follows.
  - IP Address: set to Auto.
  - DNS Server Address: set to Auto.
  - Private IP Address: set to Auto.
- Save the new network settings and reboot the WaveMaker.
- Wait at least five minutes for the device to warm up.
- Open a web browser on the PC.
- Navigate to the following web page.
  - mDNS: {serial number}.local
  - Ethernet: 169.254.6.8 (default)
  - USB: 192.168.6.8 (default)
- The WaveMaker can now be controlled using the web interface.

# Troubleshooting

## Check Physical Connections
- Option 1: Ethernet cable is connected to networked wall socket port within the same subnet as PC.
- Option 2: Ethernet or USB cable is connected directly to PC.
- Power cable is connected from the WaveMaker to mains power.

## Reboot Devices
- WaveMaker
- Host PC
- Networking Equipment: router, modem, switch, etc.

## Check the Network Settings (connecting via Local Area Network)
- Confirm WaveMaker is in the same subnet as host PC.
- Confirm WaveMaker is assigned a valid IP address.
- Confirm host PC and network supports mDNS discovery protocol.
- Ask network administrator to whitelist the WaveMaker within the network.
- Connect to WaveMaker via direct connection, then use the Tools page to configure the WaveMaker network settings.

## Check the Host PC Settings (connecting via Direct Connection)
- Check the IPv4 properties of the network adapter.
- Confirm the IP address and subnet mask of the WaveMaker is valid.

## Reset the WaveMaker Network Configuration
- Power on the WaveMaker using the keylock switch from the front panel.
- Wait at least five minutes for the device to warm up.
- Long press the Reset button from the rear panel using a small tool, such as a screwdriver. Hold down the button for at least ten seconds.
- Release the Reset button.
- Power cycle the WaveMaker.
- After power cycling, the WaveMaker network configuration should now be reset to the default values.

## Network Configuration Default Values
- Mode: DHCP then Fixed IP
- IP Address (Ethernet): 169.254.6.8
- IP Address (USB): 192.168.6.8
- Subnet Mask: 255.255.0.0

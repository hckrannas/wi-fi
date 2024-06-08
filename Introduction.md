# Basic Terminologies & Concept 
## 1. Access Point (AP)
An Access Point (AP) is a device that creates a wireless local area network (WLAN), typically in an office or large building. It connects to a wired router or switch and allows WiFi-enabled devices to connect to the network.
  * Purpose: To serve as a bridge between wired and wireless networks.
  * Functionality: Broadcasts a WiFi signal, allowing devices to connect to it wirelessly.
## 2. Service Set Identifier (SSID)
The SSID is the name of a WiFi network. It's what you see when you search for available networks on your device.
  * Purpose: Identifies the network.
  * Configuration: Can be set to a unique name by the network administrator.
## 3. Basic Service Set Identifier (BSSID)
The BSSID is the MAC address (hardware address) of the AP or wireless router. It uniquely identifies each AP on the network.
  * Purpose: Distinguishes between different APs within the same network.
  * Format: Typically in hexadecimal format, e.g., 00:14:22:01:23:45.
## 4. Extended Service Set Identifier (ESSID)
The ESSID refers to the SSID used across a group of APs that form an Extended Service Set (ESS). An ESS consists of multiple APs with the same SSID, allowing seamless roaming for clients.
  * Purpose: Facilitates roaming and consistent connectivity across multiple APs.
  * Example: Multiple APs in a large office building using the same SSID.
## 5. Roaming
Roaming in WiFi refers to the ability of a device to move between different APs within the same ESS without losing the connection or needing to reconnect manually.
  * Purpose: Maintains network connection while moving.
  * Mechanism: The device automatically switches to the AP with the strongest signal.
## 6. Channel
WiFi channels are specific frequency ranges within the broader WiFi frequency bands (2.4 GHz and 5 GHz) used for communication.
  * Purpose: Allows multiple networks to operate without interfering with each other.
  * Selection: Channels should be set to minimize interference from nearby networks.
## 7. Data Rate 
Data rate refers to the speed at which data is transmitted over the wireless network, typically measured in megabits per second (Mbps).
  * Purpose: Indicates network performance and bandwidth.
  * Influencing Factors: Signal strength, distance from the AP, network congestion.
## 8. Beacon 
A beacon is a type of frame sent by an AP at regular intervals to announce the presence of the network.
  * Purpose: Helps devices locate and connect to the network.
  * Contents: Includes SSID, supported data rates, and other network information.

# Wireless Operating Modes
## 1. Managed Mode (Station Mode)
 * Default Mode: Used by client devices to connect to WiFi networks.
 * Behavior: Receives only packets addressed to it or broadcast by the network it’s connected to.
## 2. Monitor Mode
 * Packet Capture: Captures all wireless packets in the vicinity, not just those intended for the device.
 * Uses: Packet sniffing, network diagnostics, and security testing.
 * Key features and benefits:
    - Complete Packet Capture
    - Passive Monitoring
    - Network Analysis
    - Security Assessment
    - Traffic Analysis
 * How to:
    - List all avalaible wireless interface `airmon-ng`
    - Start monitor mode `airmon-ng start <interface>`
    - Stop monitor mode `airmon-ng stop <monitor_interface>`, check the monitor_interface with `iwconfig`
## 3. Promiscuous Mode
 * Context: Used in wired networks to capture all packets.
 * WiFi Relevance: Less commonly used in wireless because monitor mode provides a superset of promiscuous mode functionality.

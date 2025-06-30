# Task 5 - Wireshark Packet Capture & Protocol Analysis (Linux)

## Objective:
Capture live network traffic using Wireshark and identify common network protocols such as TCP, DNS, ARP, and ICMP.

## Tools Used:
* Kali Linux - Running in VirtualBox
* Wireshark - Pre-installed in Kali
* Firefox - browser to generate traffic
* ping - command in terminal

## Files:
* 'network_capture.pcap': The packet capture file
* 'README.md': This report

## Steps Performed:

### Step 1: Launch Wireshark
    Open Wireshark in Kali Linux from the app menu or using terminal:
  ```bash
  wireshark

### Step 2: Select the Correct Interface

    From the interface list, selected the active one eth0 showing live traffic.

### Step 3: Start Capturing Packets

    Clicked on the correct interface to start live packet capture.

### Step 4: Generate Traffic

    Opened Firefox and visited:

        * https://wikipedia.org

        * http://neverssl.com (plain HTTP)

    Ran the following command in terminal:

    ping google.com

### Step 5: Stop the Capture

    After 1 minute, clicked the red square button in Wireshark to stop the capture.

### Step 6: Save the Capture File

    Saved the file as: network_capture.pcap

### Step 7: Analyze the Traffic

    Applied filters in Wireshark to view specific protocols:

        icmp for ping traffic

        dns for name resolution

        http, tcp, arp, etc.

    Examined packet details such as source/destination IP, protocol type, and payload.

## Protocols Observed:

ARP - Resolves IP addresses to MAC addresses on local network
ICMP - Ping requests and replies
TCP	- Connection protocol for reliable data transfer
DNS	- Resolves domain names (e.g., google.com)
HTTP	- Unencrypted web traffic (e.g., neverssl.com)

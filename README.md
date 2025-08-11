# Task 5 – Capture and Analyze Network Traffic Using Wireshark

## Objective
Capture live network packets using Wireshark and identify basic protocols and traffic types.

## Tools Used
- Kali Linux (Debian-based penetration testing distribution)
- Wireshark (Free and Open Source Network Protocol Analyzer)

## Steps Performed
1. Launched Kali Linux and installed Wireshark using:
   ```bash
   sudo apt update && sudo apt install wireshark
   ```
2. Selected the active network interface (wlan0) and started packet capture.

3. Generated traffic by:

   Browsing websites

   Running ping commands to external servers (www.google.com)

4. Stopped the capture after approximately 1 minute.

5. Applied protocol filters in Wireshark to identify different types of packets.

6. Saved the capture as task5_capture.pcap.

## Protocols Identified

1. DNS (Domain Name System)

Purpose: Translates domain names into IP addresses.

Observation: Queries were made to resolve hostnames such as google.com.

2. ARP (Address Resolution Protocol)

Purpose: Maps IP addresses to MAC addresses in the local network.

Observation: Multiple ARP requests were broadcast to find hardware addresses.

3. ICMP (Internet Control Message Protocol)

Purpose: Used for diagnostics and error messages (e.g., ping requests/replies).

Observation: ICMP Echo Request and Echo Reply packets were captured during ping tests.


## Observations

- DNS queries were primarily sent to Google’s public DNS server (8.8.8.8).

- ARP requests resolved local network devices’ MAC addresses.

= ICMP packets verified network connectivity.


## Outcome

Successfully captured and analyzed live network traffic in Kali Linux.

Learned to identify DNS, ARP, and ICMP protocols using Wireshark.

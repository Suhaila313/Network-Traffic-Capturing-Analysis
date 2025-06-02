# Wireshark Network Traffic Analysis

A hands-on lab capturing and analyzing live network traffic using Wireshark on Kali Linux, identifying key protocols (TCP, ICMP, DNS) and exporting findings.

# Task Overview
- Objective: Capture live packets, identify protocols, and analyze traffic.
- Tools: Wireshark (Kali Linux).
- Key Skills: Packet filtering, protocol analysis, `.pcap` export.

# Steps Performed
1. Captured traffic on interface `eth0` (ICMP pings + HTTP browsing).
2. Filtered protocols:
   - `tcp` (e.g., web connections)
   - `icmp` (ping tests)
   - `dns` (domain resolution)
3. Exported results as `task5_capture.pcap`.
4. Documented findings with screenshots and analysis.


# Key Findings
| Protocol | Example Traffic | Purpose |
|----------|------------------|---------|
| TCP  | `10.0.2.15 → 34.36.137.293:448` | Web connections |
| ICMP | Ping to `142.250.205.14` | Network testing |
| DNS  | Queries to `192.168.1.1` | Domain resolution |


# How to Reproduce
1. Install Wireshark:
   sudo apt update && sudo apt install wireshark -y
2. Filter protocols:
   tcp || icmp || dns

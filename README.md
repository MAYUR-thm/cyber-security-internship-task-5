# cyber-security-internship-task-5
Network packet capture &amp; analysis using Wireshark. Includes .pcap file, protocol analysis report

# Task 5 Report: Network Traffic Analysis with Wireshark

## 1. Overview
This task involved capturing live network traffic using Wireshark and analyzing different network protocols. The objective was to gain hands-on experience with packet analysis and protocol identification.

## 2. Tools Used
- **Wireshark** - Network protocol analyzer
- **Kali Linux** - Operating system
- **Web Browser** - To generate HTTP/HTTPS traffic
- **Ping Command** - To generate ICMP traffic

## 3. Capture Process
1. Started Wireshark capture on the active network interface
2. Generated traffic by:
   - Browsing multiple websites (google.com, kali.org, etc.)
   - Running ping commands
   - Normal system network activity
3. Captured traffic for approximately 60 seconds
4. Stopped capture and saved as `.pcap` file

## 4. Protocols Identified
Based on the packet capture analysis, I identified the following protocols:

| Protocol | Purpose | Example in Capture |
|----------|---------|-------------------|
| **TCP** | Reliable data transmission | Web browsing connections, [ACK] packets |
| **TLSv1.2** | Encrypted communication | HTTPS traffic, Encrypted Alert messages |
| **ARP** | IP to MAC address resolution | "Who has 192.168.1.13?" queries |
| **ICMPv6** | IPv6 network diagnostics | Neighbor Solicitation/Advertisement |

## 5. Key Findings
- **TCP** was the most common protocol, handling reliable connections
- **TLSv1.2** secured web traffic to various servers
- **ARP** resolved local network device addresses
- **ICMPv6** handled IPv6 neighbor discovery on the network
- Most web traffic was encrypted (TLS), showing modern security practices

## 6. Screenshots
- `capture-screenshot.png` - Main capture window
- `tcp-filter.png` - TCP packets filtered view
- `tls-filter.png` - TLS encrypted traffic
- `arp-filter.png` - ARP address resolution
- `icmpv6-filter.png` - ICMPv6 neighbor discovery

## 7. Files Included
- `my_capture.pcap` - Original packet capture file
- `README.md` - This report file


---

*This report was generated as part of a Cyber Security Internship Task.*

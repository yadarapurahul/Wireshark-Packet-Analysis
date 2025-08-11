## Wireshark-Packet-Analysis
Hands-on Wireshark project for capturing, filtering and analyzing live network traffic. Identifies multiple protocols, applies packet filters and provides insights into TCP/IP communication for network troubleshooting and cybersecurity learning.

## Tools Used
- **Wireshark** (Free & Open Source Network Protocol Analyzer)  
- **Operating System:** Windows 10 / Linux / macOS
- **Network Interface:** Wi-Fi

---

## Steps Performed

### 1. Install Wireshark
- The Wireshark is pre- installed in kali linx.
- If is didn't installed the install it from **https://www.wireshark.org/download.html**.
- Installed **Npcap** driver for packet capturing.

### 2. Start Packet Capture  
- Opened Wireshark and selected the active **Wi-Fi network interface** (eth0, lan0 , etc..)
- Double click on it to **Start Capturing** button (blue shark fin icon).

### 3. Generate Network Traffic
- Opened multiple websites (Google, Youtube, Wikipedia).
- Run *Ping google.com* in terminal.
- Sent a test email to genearte SMTP/IMAP traffic.

### 4. Stop Capture
- Captured for around **1 minute**.
- Stoppeed the capture and saved it as **Result Sample.pcap**.

### 5. Filter and Analyze Packet
- Applied display filters;
  - *http* -> To view HTTP packets.
  -  *dns* -> To view DNS query & response packets.
  -  *tcp* and *udp* -> To view transport layer traffic.

### 6. Identify Protocols
- Found multiple protocols in the capture:
  - **HTTP** - Website requests & responses.
  - **DNS** - Domain name lookups.
  - **TCP** - Transport control for reliable connections.
  - **ICMP** - Ping request & reply messages.
  - **ARP** - Address resolution for MAC to IP mapping.

---

## Summary of Findings

|**Protocol**|**Packets**|**% of Total**|**Purpose**|
|:---------|--------:|-----------:|:--------|
|**DNS**|110|1.2%|Domain name resolution|
|**HTTP**|2|0.02%|Web browsing(unencrypted)|
|**TCP**|528|5.9%|Reliable,connection-oriented data transport|
|**ICMPv6**|10|0.1%|IPv6 network diagnostics|
|**ARP**|8|0.1%|Local network device address resolution|
|**QUIC IETF**|8372|93.8%|Secure, low-latency transport for HTTP/3 traffic|
|**TLS**|120|1.3%|Encryption for secure web/email traffic|

- **Total Packet Caputred**: 8930

## Screenshots

- **Protocols appear in packet.png** - After the capture the network what area the protocols are appear
- **Dashboard of Wireshark.png** - Dashboard of wireshark and selecting the network to capture and analyze the network traffic.
- **capture the network .png** - Capture the network traffic with select of the network interference.
- **Result Sample.pcapng** - The result sample of the network traffic after capture; from the result sample we can alanyse the protocols etc..

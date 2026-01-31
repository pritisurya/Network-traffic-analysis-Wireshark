# 📡 Network Traffic Analysis using Wireshark (PCAP Lab)

## 🔍 Project Overview
This project demonstrates hands-on network traffic analysis using **Wireshark** on a private home Wi-Fi network.  
The goal of the lab was to capture, filter, and analyze real network packets to understand how common protocols operate at the packet level.

Through this project, raw packet captures (PCAP files) were analyzed to identify **ICMP, DNS, TCP handshake, and HTTP-related traffic**, simulating the type of analysis performed by SOC analysts and network security engineers.

---

## 🎯 Objectives
- Capture live network traffic using Wireshark
- Analyze common network protocols
- Apply Wireshark display filters
- Understand how user actions translate into packets
- Document findings with screenshots and explanations

---

## 🛠 Tools & Environment
- **Wireshark**
- **Windows OS**
- **Private Home Wi-Fi Network**
- Command Line Utilities (`ping`, `nslookup`, `curl`)
- Web Browser

---

## 📦 Protocols Analyzed

### 🔹 ICMP (Ping Traffic)
- Generated using `ping 8.8.8.8`
- Captured Echo Request and Echo Reply packets
- Used to verify network connectivity

**Wireshark Filter**
Screenshot ICMP


---

### 🔹 DNS (Domain Name System)
- Generated using `nslookup openai.com`
- Captured DNS query and response packets
- Demonstrates domain-to-IP resolution

**Wireshark Filter**
Screenshots DNS


---

### 🔹 TCP Port 80 (HTTP Attempt)
- Captured TCP packets directed to port 80
- Demonstrates HTTP traffic behavior despite HTTPS enforcement
- Shows that TCP metadata remains visible even when payloads are encrypted

**Wireshark Filter**
screenshot TCP


---

### 🔹 Background / Miscellaneous Traffic
- Captured real-world background traffic
- Includes OS services, DNS chatter, and routine TCP communication
- Demonstrates realistic network noise

---

## 📸 Screenshots
Screenshots of each filtered analysis are included to visually demonstrate packet inspection and protocol behavior.

---

## 📂 Project Structure
Wireshark-Network-Analysis/
│
├── captures/
│ └── home-network-analysis.pcapng
│
├── screenshots/
│ ├── icmp.png
│ ├── dns.png
│ ├── tcp-handshake.png
│ ├── tcp-port-80.png
│ └── random-traffic.png
│
└── README.md


---

## 🧠 Key Learnings
- Network traffic follows predictable patterns
- Packet captures tell a complete story of communication
- Modern security mechanisms (HTTPS, DoH) affect visibility
- DNS and TCP behavior are critical for threat detection
- Real-world networks contain significant background noise

---

## 🚀 Future Enhancements
- Analyze malicious PCAP files
- Detect port scans and suspicious traffic
- Integrate IDS tools like Suricata
- Apply machine learning for traffic anomaly detection

---

## 🛡 Disclaimer
All traffic captured was generated on a private network for educational purposes only.  
No unauthorized interception or analysis was performed.

# 🛡️ CyberSecurity-TASK-5

## Task 5: Capture and Analyze Network Traffic Using Wireshark

### 📌 Objective

The objective of this task is to capture live network traffic using **Wireshark** and analyze the captured packets to identify common network protocols and understand basic traffic behavior.

This practical exercise provides hands-on experience with packet capture, protocol filtering, and basic network traffic analysis.

---

## 🛠️ Tools Used

* 🦈 Wireshark
* 💻 Windows PC
* 🌐 Internet Connection
* 📦 PCAP File Format

---

## 🔎 Task Performed

The following steps were performed during the network traffic analysis:

1. Installed Wireshark.
2. Identified the active network interface.
3. Started a live packet capture.
4. Generated network traffic by browsing websites and/or communicating with a server.
5. Stopped the capture after collecting sufficient traffic.
6. Applied protocol filters to analyze different types of packets.
7. Identified at least three network protocols.
8. Examined packet information such as source, destination, protocol, and packet details.
9. Exported the captured traffic as a `.pcap` file.
10. Documented the observations and findings.

---

## 🔍 Wireshark Filters Used

The following display filters can be used to analyze common protocols:

```text
dns
```

Shows DNS queries and responses.

```text
tcp
```

Displays TCP traffic.

```text
http
```

Displays HTTP traffic when HTTP packets are present.

Additional useful filters:

```text
udp
```

Displays UDP traffic.

```text
icmp
```

Displays ICMP traffic such as ping packets.

---

## 🌐 Protocols Identified

### 1. DNS – Domain Name System

DNS is used to translate domain names into IP addresses.

**Example:**

```text
example.com → IP Address
```

DNS packets can be used to observe domain-name resolution activity.

---

### 2. TCP – Transmission Control Protocol

TCP provides reliable, connection-oriented communication between network devices.

TCP is commonly used by applications such as web browsing, email, and file transfers.

Important TCP flags include:

* SYN
* ACK
* FIN
* RST

---

### 3. HTTP – Hypertext Transfer Protocol

HTTP is used for transferring web content between clients and servers.

> HTTP traffic may not appear during normal browsing because most modern websites use HTTPS.

---

### 4. UDP – User Datagram Protocol

UDP is a connectionless protocol that is commonly used where speed and low overhead are important.

Examples include DNS queries and certain streaming or real-time applications.

---

## 📊 Packet Analysis

During packet analysis, the following information can be examined:

| Field       | Description                           |
| ----------- | ------------------------------------- |
| Source      | Device sending the packet             |
| Destination | Device receiving the packet           |
| Protocol    | Network protocol being used           |
| Length      | Size of the packet                    |
| Info        | Additional packet information         |
| Time        | Time at which the packet was captured |

---

## 📈 Findings

The captured network traffic demonstrated that multiple protocols can operate simultaneously during normal internet activity.

The analysis helped identify:

* DNS requests and responses.
* TCP connections between network endpoints.
* UDP-based traffic where present.
* HTTP traffic where available.
* Source and destination information.
* Different packet types and communication patterns.

> **Note:** The final protocol findings should match the protocols actually present in the submitted `.pcap` file.

---

## 📦 PCAP Capture

The captured network traffic is stored in a `.pcap` file.

Recommended project file:

```text
Capture/
└── network-traffic.pcap
```

The PCAP file can be opened in Wireshark for further packet-level analysis.

---

## 📸 Screenshots

Screenshots can be included as evidence of the packet capture and analysis.

Recommended files:

```text
Screenshots/
├── packet-capture.png
└── protocol-analysis.png
```

A screenshot should preferably show the Wireshark interface with captured packets and the applied protocol filter.

---

## 📁 Project Structure

```text
CyberSecurity-TASK-5/
│
├── README.md
│
├── Capture/
│   └── network-traffic.pcap
│
├── Report/
│   └── network-traffic-analysis-report.md
│
└── Screenshots/
    ├── packet-capture.png
    └── protocol-analysis.png
```

---

## 🛡️ Security and Privacy Considerations

Network captures can contain sensitive information such as:

* IP addresses
* Domain names
* Device information
* Network metadata
* Application traffic

Therefore, only capture traffic from networks and devices that you are authorized to monitor.

Before publishing a `.pcap` file to GitHub, review it carefully and remove or avoid sharing sensitive information.

---

## 🎯 Learning Outcomes

After completing this task, I learned:

* How to capture live network traffic using Wireshark.
* How packets are transmitted across a network.
* How to filter traffic by protocol.
* How to identify DNS, TCP, UDP, HTTP, and other protocols.
* How to examine packet source and destination information.
* How to save and analyze `.pcap` files.
* The importance of network monitoring and packet analysis.

---

## ✅ Conclusion

This task provided practical experience in capturing and analyzing network traffic using Wireshark.

By examining individual packets and applying protocol filters, I gained a better understanding of how different network protocols communicate and how packet analysis can be used for network troubleshooting, monitoring, and cybersecurity investigations.

---

## ⚠️ Disclaimer

This project is intended for **educational and cybersecurity awareness purposes only**.

Network traffic was captured only from an authorized device/network. No unauthorized monitoring, interception, or access was performed.

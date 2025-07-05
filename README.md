# Construction of Simple LAN and Understanding ARP using Cisco Packet Tracer

## 📌 Aim
To construct a simple Local Area Network (LAN) using Cisco Packet Tracer and to observe the working of the Address Resolution Protocol (ARP) for resolving IP addresses to MAC addresses.

---

## 📝 Problem Statement
In Ethernet-based networks, communication is carried out using MAC addresses, but most applications use IP addresses. Address Resolution Protocol (ARP) is needed to map IP addresses to MAC addresses for successful communication. This project aims to simulate a LAN setup where devices resolve MAC addresses using ARP.

---

## 📈 Scope of the Solution
- Setup and configure a LAN with 4 PCs connected through an 8-port switch.
- Assign IP addresses within the same subnet.
- Demonstrate ARP in action using ping and ARP table commands.
- Use Cisco Packet Tracer’s simulation mode to visualize ARP packets.

---

## 🧱 Network Architecture / Overview

```
PC0 ---\
        \
PC1 ----- Switch (8-Port)
        /
PC2 ---/
       \
        PC3
```

- All PCs are in the same subnet (192.168.1.0/24).
- Devices communicate through a central switch.
- ARP resolves unknown MAC addresses when pinging.

---

## ⚙️ Components Required

| Component                  | Quantity | Description                         |
|----------------------------|----------|-------------------------------------|
| PC                         | 4        | End devices for the LAN             |
| Cisco 2960-8TT Switch      | 1        | 8-port switch for internal LAN      |
| Copper Straight-through Cable | 4    | For PC-to-switch connections        |
| Cisco Packet Tracer        | 1        | Network simulation software         |

---

## 🧪 Steps to Simulate

1. **Launch Cisco Packet Tracer**
2. **Place 4 PCs** (`PC0`, `PC1`, `PC2`, `PC3`) and an **8-Port Switch**
3. **Connect each PC to the switch** using straight-through cables
4. **Assign IP Addresses**:
   - PC0: `192.168.1.10 /24`
   - PC1: `192.168.1.11 /24`
   - PC2: `192.168.1.12 /24`
   - PC3: `192.168.1.13 /24`
5. **Test Connectivity**:
   - Ping from `PC0` to `PC1`, `PC2`, and `PC3`
   - Use command `arp -a` to view resolved MAC addresses
6. **Use Simulation Mode**:
   - Filter for ARP packets
   - Observe ARP request and reply when initiating ping

---

## 🖼️ Screenshot of Logical Topology

![LAN Screenshot](screenshot.png)
> *(Replace with your actual screenshot from Packet Tracer's logical workspace)*

---

## ✅ Expected Results
- All PCs can ping each other successfully.
- ARP tables show resolved MAC addresses.
- ARP packets appear in simulation mode (Request → Reply).

---

## 📚 Additional Notes
- ARP is a layer-2 protocol essential for IP-to-MAC mapping in LANs.
- Cisco Packet Tracer provides a visual and interactive way to understand ARP.

---

## 👨‍💻 Author
**Your Name**  
**Date:** July 2025

---

## 📁 File Structure

```
├── LAN_ARP_Simulation/
│   ├── SimpleLAN_ARP.pkt         # Cisco Packet Tracer file
│   ├── README.md                 # This documentation
│   └── screenshot.png            # Topology screenshot (insert manually)
```

---

## 🔗 References
- Cisco Networking Academy
- CCNA Curriculum: Network Fundamentals

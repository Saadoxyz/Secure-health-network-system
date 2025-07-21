# 🏥 Secure Health Network System — Cisco Packet Tracer

## 🔐 Project Overview

Design and implement a **secure and segmented healthcare network** using Cisco Packet Tracer. This system simulates a robust, scalable infrastructure that spans internal floors, DMZ, cloud integration, VLAN segmentation, redundancy, and secure services.

---

## 🚀 Key Features

- **🏗️ Hierarchical & Redundant Design**  
  Core–Distribution–Access layers with HSRP, OSPF, and EtherChannel redundancy

- **🌐 VLAN Segmentation**  
  - VLAN 10: LAN  
  - VLAN 50: WLAN  
  - VLAN 99: VoIP  
  - DMZ hosting critical servers

- **🔄 Inter-VLAN Routing**  
  Managed by multilayer switches and HSRP virtual routers

- **🛡️ Secure Firewall Configuration (Cisco ASA)**  
  - Security zones (INSIDE, DMZ, EXTERNAL)  
  - Zone-based ACLs, NAT/PAT, default routes

- **📶 Wireless LAN Controller**  
  Centralized WAP management + VLAN-specific wireless access

- **📞 VoIP Services**  
  IP telephony with VoIP VLAN, VoIP DHCP, and telephony service support

- **🧰 Utility Servers in DMZ**  
  - DHCP & DNS (Azure Directory-integrated)  
  - Email, File, Web servers  
  - Virtualization via ESXi for failover

- **☁️ Cloud Integration**  
  Simulated AWS Cloud segment connected via secure OSPF routing

- **🧪 Protocol Configuration**  
  OSPF across routers, switches, firewall  
  SSH access via ACL-limited VTY lines

---

## 🛠️ Configuration Summary

| Component                   | Configuration Highlights |
|----------------------------|--------------------------|
| **Multilayer Switches**    | VLAN SVIs, HSRP groups, DHCP helper addresses |
| **EtherChannel**           | LACP trunk bundles between distribution switches |
| **Firewall (ASA)**         | Zone-based policies, NAT, ACLs for DMZ separation |
| **Routers / OSPF**         | Area 0 across LAN, DMZ, Cloud, WAN |
| **DHCP / DNS**             | Pools for LAN/WLAN/VoIP, DNS entries via Directory Server |
| **VoIP Gateway**           | VoIP VLAN, DHCP, telephony-service, auto phone registration |
| **WLC & WAPs**             | VLAN 50 WiFi access with CAPWAP connectivity |
| **Redundancy**             | Hot-standby router with HSRP, trunk-level redundancy |

---

## 🧪 Testing & Verification

- ✅ **End-to-End Connectivity**: VLANs ping across devices  
- ✅ **Service Accessibility**: Web, Email, File, VoIP, DHCP, DNS reachable  
- ✅ **Wireless Clients**: Connected via WLC to correct WLAN VLAN  
- ✅ **HSRP Validation**: Failover simulation between multilayer switches  
- ✅ **ACL Effectiveness**: Internal traffic allowed while DMZ/external is regulated

---

## 📂 Environment

- **Tool**: Cisco Packet Tracer 8.x  
- **Platform**: Windows/Linux/macOS  
- **Prerequisites**: Basic familiarity with VLANs, OSPF, EtherChannel, HSRP, ASA, VoIP, DHCP, DNS

---

## 👤 Author

**Saad Khan**  
📧 saado652004@gmail.com  
🌀 GitHub: [@saadoxyz](https://github.com/saadoxyz)

---

> 🎯 *“Building secure, redundant, scalable healthcare networks—where segmentation meets service reliability.”*


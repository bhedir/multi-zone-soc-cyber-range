<!-- PROJECT HEADER -->
<div align="center">

# 🛡️ Network Infrastructure and Security Project  
### A Multi-Zone Network with an Integrated Security Operations Center (SOC)

[![Made with GNS3](https://img.shields.io/badge/Made%20with-GNS3-blue?logo=gns3&logoColor=white)]()
[![VMware](https://img.shields.io/badge/VMware-Workstation-orange?logo=vmware)]()
[![FortiGate](https://img.shields.io/badge/FortiGate-Firewall-red?logo=fortinet)]()
[![Linux](https://img.shields.io/badge/Linux-Ubuntu%20%7C%20CentOS-green?logo=linux&logoColor=white)]()
[![Windows Server](https://img.shields.io/badge/Windows%20Server-2022-blue?logo=windows&logoColor=white)]()
[![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?logo=docker&logoColor=white)]()
[![Security](https://img.shields.io/badge/Security-SOC%20%7C%20SIEM%20%7C%20SOAR-critical?logo=securityscorecard)]()

📘 **Author:** *Hadir Ben Arbia*  
📅 **Date:** August 2025  

</div>

---

## 📖 Overview

This project demonstrates the **design and implementation** of a **multi-zone enterprise network** integrated with a **Security Operations Center (SOC)**.  
It combines advanced network segmentation, intrusion prevention, and **automated incident response** using open-source and commercial technologies.

The environment was built using **GNS3** and **VMware Workstation**, integrating the following technologies:

- 🧱 FortiGate (Next-Generation Firewall)  
- 🧠 Windows Server 2022 (Active Directory & DNS)  
- 🐧 Ubuntu Clients  
- 🕵️ Suricata (Intrusion Prevention System)  
- 🧩 Wazuh (SIEM)  
- ⚙️ Shuffle (SOAR)  
- 🔐 PacketFence (Network Access Control)

---

## 🧩 Architecture Overview

The network is divided into **three primary zones** controlled by FortiGate:

| Zone | Subnet | Purpose |
|------|---------|----------|
| 🟢 **LAN** | `192.168.10.0/24` | Internal trusted network with AD, clients, SOC |
| 🟠 **DMZ** | `192.168.30.0/24` | Hosts public web services |
| 🔵 **WAN** | DHCP | Internet access via GNS3 NAT Cloud |

## 🌐 Network Topology

The project implements a multi-zone architecture segmented into **LAN**, **DMZ**, and **WAN** zones — all managed by FortiGate.  
Below is the real topology used for the deployment:

<p align="center">
  <img src="./schema_topologie.png" alt="Network Topology" width="800">
</p>


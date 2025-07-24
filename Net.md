# Home Network Documentation

---

## 1. Physical Topology

###  Description

My home network span includes both wired and wireless connections. The **Shaw router** are located in the **living room**, distributing connectivity to several devices across rooms. Devices such as a **desktop PC** is connected via Ethernet, while laptops, mobile devices, and IoT appliances connect via **Wi-Fi**.

### Device Placement (by Location)

- **Living Room**  
  - Router (connected to ISP)
  - Laptop (Wi-Fi)
  - TV (Wi-Fi)
  - Tablet (Wi-Fi)
- **Bedroom1**
  - PC (Ethernet)
  - Smartphone (Wi-Fi)

- **Bedroom2**
  - Laptop (Wi-Fi)
  - Smartphone (Wi-Fi)

### Physical Topology Diagram

<img width="851" height="471" alt="image" src="https://github.com/user-attachments/assets/c622a1c8-edaa-4e4a-a4b2-a66304820c25" />

---

## 2. Logical Topology

### Logical Network Overview

All devices are connected to a single **local network (LAN)** with subnet `192.168.83.0/24`. The **router handles DHCP, NAT, and DNS**, and distributes addresses dynamically. There are no VLANs in use. Wi-Fi and Ethernet connections share the same IP range.

### Network Design Highlights

- **Router IP:** 192.168.83.1 (Default Gateway + DNS)
- **Subnet:** 255.255.255.0 
- **DHCP Range:** 192.168.83.100 – 192.168.83.200
- **SSID:** HSNET (WPA3 secured)


### Logical Topology Diagram




---

## 3.  Addressing Documentation

| Device         | MAC Address        | IP Address       | Hostname     | Connection | Assigned By | Notes               |
|----------------|--------------------|------------------|--------------|------------|-------------|----------------------|
| Router         | `00:11:22:33:44:55`| `192.168.83.1`    | router       | LAN        | Static      | Gateway + DHCP/DNS   |
| Desktop PC     | `11:22:33:44:55:66`| `192.168.83.100`  | pc-living    | Ethernet   | Static      | Used for work        |
| Laptop HP       | `AA:BB:CC:DD:EE:FF`| `192.168.83.101`  | HP            | Wi-Fi      | DHCP        | Student device       |
|  Laptop Lenovo  | `66:77:88:99:AA:BB`| `192.168.83.102`  | Lenovo     | Wi-Fi   | DHCP              | Personal Use  |
| TV             | `77:88:99:AA:BB:CC`| `192.168.83.103`  | tv-living    | Wi-Fi      | DHCP        | Streaming Services   |
| Samsung S21    | `88:99:AA:BB:CC:DD`| `192.168.83.104`  | S21       | Wi-Fi      | DHCP        | Personal phone       |
| Iphone 14        | `88:99:AB:BB:CC:AE` | `192.168.83.105`   |  IPhone14 | Wi-Fi       | DHCP      |  Personal phone    |

---

## 4.  Device Configuration Details

###  Router Configuration

- IP: `192.168.83.1`
- DHCP Enabled: `192.168.83.100–200`
- SSID: `HSNET`
- Security: WPA3-Personal
- Firewall: Enabled
- DNS Forwarding: Auto via ISP
- Remote Admin: Disabled
- Auto Updates: Enabled

### Desktop PC (Static IP)

- IP: `192.168.83.100`
- Subnet: `/24`
- Gateway: `192.168.83.1`
- DNS: `192.168.83.1`
- Windows Firewall: Enabled


---

## 5.  Credential Storage Method

All login credentials are stored in **Bitwarden**, a secure and encrypted password manager.

### Security Features Used:

- **Master Password**: Strong + memorable
- **Two-Factor Authentication (2FA)**: Enabled via Authenticator App
- **Vault Encryption**: End-to-end (AES-256)
- **Device Lock**: Biometric authentication on phone


---

## ✅ Final Notes

This network documentation outlines the **entire structure** and **configuration** of my home network in accordance with best practices. It includes visual topology diagrams, IP addressing, detailed configurations, and secure password storage — demonstrating a full understanding of both **physical** and **logical** network design.






# **PacketTracer-Company-Network**

**Project File:** `pk.pkt`

A small corporate network simulation for **IT, HR, and Guest VLANs** using Cisco Packet Tracer.
Demonstrates practical networking, system administration, and basic cybersecurity skills.

---

## **Project Overview**

This project simulates a secure company network with multiple departments and essential services.
It highlights VLAN segmentation, DHCP, DNS, HTTP, Email (demo), FTP (optional), and ACL-based security.

* **Departments / VLANs:**

  * **IT (VLAN 10)** – Blue squares
  * **HR (VLAN 20)** – Green squares
  * **Guest (VLAN 30)** – Yellow squares
* **Core Infrastructure:**

  * **Router (R1)** – Gray rectangle, inter-VLAN routing
  * **Switch (SW)** – Light gray rectangle, connects all PCs and Server
  * **Server** – Red rectangle, provides DHCP, DNS, HTTP, Email, FTP

---

## **Network Services**

| Service            | IP / VLAN                                                  | Description                                                     |
| ------------------ | ---------------------------------------------------------- | --------------------------------------------------------------- |
| **DHCP**           | 192.168.10.1 (IT), 192.168.20.1 (HR), 192.168.30.1 (Guest) | Automatic IP assignment per VLAN                                |
| **DNS**            | 192.168.10.100                                             | Resolves `company.local` for internal websites and email        |
| **HTTP**           | 192.168.10.100                                             | Web pages for IT and HR departments                             |
| **Email**          | 192.168.10.100                                             | Demo internal email between IT & HR                             |
| **FTP (optional)** | 192.168.10.100                                             | File sharing for department folders                             |
| **ACL / Security** | Router & Switch                                            | IT VLAN → server access only; HR limited; Guest → internet-only |
| **Port Security**  | Switch ports                                               | Limits MAC addresses, prevents unauthorized devices             |

---

## **VLAN / Device Visual Style**

| Device / VLAN | Color      | Label  |
| ------------- | ---------- | ------ |
| IT VLAN       | Blue       | IT     |
| HR VLAN       | Green      | HR     |
| Guest VLAN    | Yellow     | Guest  |
| Server        | Red        | Server |
| Router        | Gray       | Router |
| Switch        | Light Gray | SW     |

* PCs organized in **blocks by VLAN**
* Router at **top center**, Switch below, Server near center
* Connections labeled by port (e.g., `Fa0/1 IT PC1`, `G0/0.10 IT VLAN`)

---

## **Key Features & Learning Outcomes**

* **VLAN Segmentation:** Separates departments to improve security and organization
* **Inter-VLAN Routing:** Router-on-a-stick configuration for cross-VLAN communication
* **DHCP:** Automatic IP assignment per VLAN
* **DNS & HTTP:** Internal website simulation using `company.local`
* **Email:** Internal mail simulation for IT & HR
* **ACLs:** Restrict access based on VLAN, secure sensitive services
* **Port Security:** Protect switch ports from unauthorized devices
* **CV Demonstration:** Showcases practical networking, IT administration, and basic cybersecurity skills

---

## **Network Layout (Text Diagram)**

```
         Router (Gray)
             |
        Switch (Light Gray)
  -----------------------------
  | IT VLAN (Blue)           |
  | PC1  PC2                 |
  -----------------------------
  | HR VLAN (Green)          |
  | PC1  PC2                 |
  -----------------------------
  | Guest VLAN (Yellow)      |
  | PC1                       |
  -----------------------------
             |
           Server (Red)
```

---

## **How to Use**

1. Download the project file: `pk.pkt`
2. Open it in **Cisco Packet Tracer**
3. Test network services:

   * Ping between VLANs (per ACL rules)
   * DHCP IP assignment for all VLAN PCs
   * HTTP access from IT and HR PCs
   * Send/receive email internally
   * FTP file sharing (optional)
4. Observe VLAN separation and security features in simulation mode




If you want, I can also create a **short one-image visual “network map” in Markdown** to embed in this README — it’ll make your GitHub page **look even more professional at first glance**.

Do you want me to do that?

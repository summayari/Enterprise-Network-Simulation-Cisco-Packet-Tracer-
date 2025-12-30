# Enterprise Network Infrastructure Design (Cisco Packet Tracer)

![Status](https://img.shields.io/badge/Status-Completed-success)
![Tool](https://img.shields.io/badge/Tool-Cisco%20Packet%20Tracer-blue)
![Category](https://img.shields.io/badge/Category-Network%20Engineering-orange)

## 🌐 Overview
This project simulates a robust and scalable network infrastructure for a mid-sized enterprise organization. Designed in **Cisco Packet Tracer**, the topology focuses on hierarchy, security, and traffic management. 

The simulation demonstrates a fully functional campus network including **departmental segmentation (VLANs), secure internet access (NAT), and traffic prioritization (QoS)** to ensure optimal performance for critical applications.

## 🏗️ Network Topology
*(Optional: Add a screenshot of your topology here)*
> The design follows the Cisco 3-Layer Model (Core, Distribution, Access) to ensure redundancy and scalability.

## 🚀 Key Features & Configurations

### 1. Switching & Segmentation
* **VLAN Configuration:** Segmented traffic into distinct departments (e.g., HR, IT, Sales) to reduce broadcast domains and improve security.
* **Inter-VLAN Routing:** Configured **Router-on-a-Stick** (or Layer 3 Switching) to allow communication between trusted departments.
* **VTP & Trunking:** Implemented VLAN Trunking Protocol (VTP) for centralized VLAN management.

### 2. Routing & Connectivity
* **Routing Protocols:** Configured **OSPF / RIP / EIGRP** *[Choose the one you used]* for dynamic path selection and redundancy.
* **Static NAT:** Implemented Network Address Translation to provide secure public internet access for internal servers.
* **DHCP Services:** Automated IP address allocation for end devices using router-based DHCP pools.

### 3. Security & Management
* **Access Control Lists (ACLs):** Applied Standard and Extended ACLs to filter traffic and restrict unauthorized access to sensitive servers.
* **Port Security:** Enabled stick mac-addresses on access switches to prevent unauthorized device connections.
* **SSH Configuration:** Secured remote management of routers and switches.

### 4. Traffic Optimization
* **Quality of Service (QoS):** Prioritized voice/video traffic to prevent latency and jitter during high congestion.

## 🛠️ Tools Used
* **Simulator:** Cisco Packet Tracer (Version 8.x recommended)
* **Devices:** Cisco 2911 Routers, 2960 Switches, Server PT, Generic End Devices.

## 📂 Project Structure
```text
├── design/
│   ├── enterprise_network.pkt    # Main Packet Tracer simulation file
│   └── topology_diagram.png      # Image of the network layout
├── configs/                      # (Optional) Exported text configs for Routers/Switches
├── docs/
│   └── project_report.pdf        # Detailed documentation/Report
└── README.md

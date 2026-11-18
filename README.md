# Enterprise Network Infrastructure Design

A multi-site enterprise network infrastructure designed and implemented using **Cisco Packet Tracer** as part of the Network Infrastructure Design module.

## Project Overview

This project involved designing a scalable, secure and resilient network infrastructure for Excel-Tec Inc, a fictional company operating across four UK locations: London, Leeds, Liverpool and Leicester.

The network was designed to support approximately 5,600 hosts across four sites while providing reliable inter-site communication, departmental segmentation, controlled internet access and network security.

## Network Topology

The proposed infrastructure uses a four-site ring topology, connecting London, Leeds, Liverpool and Leicester.

The design incorporates three departmental VLANs at each location:

| VLAN ID | Department |
| ------- | ---------- |
| 30      | Finance    |
| 40      | Executive  |
| 50      | Employees  |

## Technologies Implemented

* **Cisco Packet Tracer:** Network design, configuration and simulation.
* **VLSM:** Efficient IP address allocation based on departmental host requirements.
* **OSPF:** Dynamic routing between all four geographical locations using Area 0.
* **Static Routing:** Additional fallback routing configuration.
* **VLANs:** Departmental network segmentation.
* **802.1Q Trunking:** Carrying multiple VLANs across network links.
* **Router-on-a-Stick:** Inter-VLAN routing.
* **DHCP:** Automatic IP address assignment.
* **ACLs:** Controlling network traffic and restricting internet access at branch locations.
* **NAT/PAT:** Allowing London-based devices to access the internet.
* **DMZ:** Isolating a public-facing web server.
* **SSH:** Secure remote management of network devices.

## Network Security

Several security mechanisms were implemented:

* Departmental traffic segmentation using VLANs.
* Extended ACLs to restrict internet access at branch offices.
* NAT/PAT for controlled internet connectivity.
* DMZ architecture for isolating the public-facing web server.
* SSH version 2 instead of Telnet.
* Encrypted device passwords.
* Secured console and VTY access.
* Login banners and session timeouts.

## Testing and Verification

The network was tested in Cisco Packet Tracer to verify its functionality.

Testing included:

* OSPF neighbour adjacency and routing table verification.
* Connectivity between the four geographical sites.
* VLAN creation and trunk port verification.
* Inter-VLAN connectivity.
* Automatic DHCP address allocation.
* Internet connectivity from London.
* Internet access restrictions at branch locations.
* DMZ web server accessibility.
* ACL and NAT verification.
* SSH configuration verification.

Screenshots demonstrating the testing results are available in the `Screenshots` directory.

## Project Files

* `Packet-Tracer/` – Cisco Packet Tracer network simulation file.
* `Documentation/` – Detailed network design report.
* `Screenshots/` – Network topology and configuration testing evidence.

## Tools

Cisco Packet Tracer | Networking | Routing | Switching | Network Security

## Learning Outcomes

This project strengthened my understanding of enterprise network architecture, IP addressing, dynamic routing, network segmentation, access control and infrastructure security.

It also provided practical experience in designing, configuring and testing a multi-site network infrastructure.

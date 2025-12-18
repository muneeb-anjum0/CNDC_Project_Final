# Smart Government Service Center Network
Cisco Packet Tracer Network Design and Configuration

## Overview
This project implements a complete enterprise-style network using Cisco Packet Tracer.  
The scenario represents a Smart Government Service Center where multiple departments operate under a secure and scalable network infrastructure.

The project was developed as part of the Computer Networks Lab (CNDC) at SZABIST.

---

## Scenario
A Smart Government Service Center provides digital services to citizens through multiple internal departments.  
Each department requires isolation, controlled communication, and access to centralized services such as DNS and web portals.

---

## Network Architecture
- Design Type: Hierarchical enterprise network
- Simulation Tool: Cisco Packet Tracer
- Routing Model: Hybrid routing architecture
- Inter-VLAN Routing: Router-on-a-Stick

---

## VLAN and Department Mapping

| VLAN ID | Department |
|-------|------------|
| 10 | Citizen Services |
| 20 | Finance and Revenue |
| 30 | Records and Data Management |

Each VLAN represents a separate broadcast domain.

---

## IP Addressing Scheme

| Network | Description |
|--------|------------|
| 192.168.0.0/24 | VLAN 10 – Citizen Services |
| 192.168.1.0/24 | VLAN 20 – Finance |
| 192.168.2.0/24 | VLAN 30 – Records |
| 8.0.0.0/24 | Regional Government Office |

---

## Routing Configuration

### Dynamic Routing
- OSPF implemented in the main service center network
- RIP implemented in the regional office network

### Static Routing
- Static routes configured to demonstrate administrative route control

---

## Switching and Inter-VLAN Routing
- VLAN creation on access switches
- Access port assignment per department
- VLAN trunking between switch and router
- Inter-VLAN routing using Router-on-a-Stick
- IEEE 802.1Q encapsulation for VLAN tagging

---

## Security Implementation
- Extended Access Control Lists (ACLs) implemented
- Traffic from the regional network restricted from accessing sensitive departments
- ACLs applied close to the source interface

---

## Server Configuration

### DNS Server
- Provides domain name resolution for internal services

### HTTP Server
- Hosts a sample government service webpage
- Accessible only to authorized users

---

## End Devices
- PCs assigned to each department VLAN
- Devices configured with static IP addressing
- Connectivity verified across VLANs and WAN

---

## Testing and Verification
The network was verified using:
- Ping tests between VLANs
- Ping tests across WAN links
- Routing table verification
- VLAN membership checks
- ACL behavior validation
- DNS and HTTP access tests

---

## Repository Contents
- Cisco Packet Tracer (.pkt) file
- Network topology diagram
- IP addressing table
- Configuration screenshots
- Project documentation

---

## Academic Information
- Course: LAB Computer Networks (CNDC)
- University: SZABIST
- Instructor: M Farooq

---

## Learning Outcomes
- VLAN-based network segmentation
- Router-on-a-Stick implementation
- Dynamic and static routing configuration
- Network security using ACLs
- Practical troubleshooting in Packet Tracer

---

## Future Enhancements
- DHCP server integration
- Wireless access deployment
- Network redundancy and failover
- Enhanced security policies

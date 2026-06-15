# Financial-Institution-Network-Design-Lab-8

## Overview

In this project, I designed and implemented a secure network for a financial institution using Cisco Packet Tracer. The network includes multiple departments, VoIP services, wireless access, centralized servers, dynamic routing, VPN connectivity, and internet redundancy through two ISPs.

## Technologies Used

* VLANs
* Inter-VLAN Routing
* Multilayer Switching
* OSPF
* DHCP
* DNS
* Email Services
* VoIP
* SSH
* ACLs
* NAT/PAT
* Site-to-Site IPsec VPN
* Wireless Access Points

## Network Design

The network consists of five departments:

* Human Resources (HR)
* Customer Service (CS)
* Marketing (MK)
* Legal Management (LM)
* Information Technology (IT)

Each department has:

* PCs
* IP Phones
* Printer
* Wireless Access Point

An external server site hosts:

* DHCP Server
* DNS Server
* Web Server
* Email Server

The headquarters is connected to the server site and two ISP routers for redundancy.

## Implementation

* Created separate VLANs for each department.
* Configured Voice VLAN 120 for IP phones.
* Implemented inter-VLAN routing using multilayer switches.
* Configured OSPF between routers and Layer 3 switches.
* Enabled DHCP services for automatic IP allocation.
* Configured VoIP services and phone extensions.
* Implemented SSH for secure remote management.
* Applied port security using sticky MAC addresses.
* Configured Standard ACL for SSH access control.
* Implemented NAT/PAT for internet connectivity.
* Configured Site-to-Site IPsec VPN between HQ and server site.
* Tested connectivity between all departments and servers.

## Verification Commands

show vlan brief

show ip interface brief

show ip route

show ip ospf neighbor

show interfaces trunk

show ip dhcp binding

show ephone registered

show dial-peer voice summary

show access-lists

show crypto isakmp sa

show crypto ipsec sa

show ip nat translations

show ip ssh

## Results

* All departments communicate successfully.
* VoIP phones can call each other.
* OSPF routing operates correctly.
* DHCP assigns IP addresses automatically.
* Internal users can access DNS, Web, and Email servers.
* SSH access works as expected.
* NAT/PAT provides internet connectivity.
* VPN tunnel between HQ and server site is operational.
* Port security and ACL policies are functioning properly.

## Key Learnings

This project provided practical experience with enterprise routing, VLAN design, VoIP deployment, VPN implementation, ACLs, NAT, and network security. It closely resembles the type of network commonly found in banks, insurance companies, and financial institutions.

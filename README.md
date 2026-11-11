# Fortigate-network-security-lab
FortiGate firewall configuration and network security lab built with EVE-NG.
# FortiGate Network Security Lab

A hands-on network security lab built with **FortiGate 7.2.4, Cisco IOSvL2 and EVE-NG**.

## Project Overview

This project demonstrates the deployment and configuration of a FortiGate firewall in a virtual enterprise network environment.

The lab covers WAN/LAN connectivity, DHCP, DNS, outbound NAT, firewall policies and traffic logging.

## Lab Topology

**Components:**
- FortiGate 7.2.4 Firewall
- Cisco IOSvL2 Virtual Switch
- Three VPCS endpoints:
  - PC-HR
  - PC-IT
  - DMZ-Zone
- EVE-NG virtualization platform

## IP Addressing

| Component | Configuration |
|---|---|
| WAN | DHCP |
| LAN Gateway | 192.168.10.1/24 |
| DHCP Pool | 192.168.10.100–192.168.10.200 |
| LAN Interface | FortiGate port2 |

## Implemented Features

- FortiGate WAN and LAN interface configuration
- DHCP server configuration
- DNS resolution
- Outbound NAT configuration
- LAN-to-WAN firewall policy
- Cisco IOSvL2 switch port configuration
- Firewall traffic logging
- End-to-end connectivity testing

## Verification and Testing

The following tests were performed successfully:

- DHCP address assignment to VPCS clients
- LAN gateway connectivity using ICMP
- Internet connectivity using `ping 8.8.8.8`
- DNS resolution using `ping google.com`
- LAN-to-WAN traffic through FortiGate

## Network Design Note

All three endpoints currently operate in the same LAN subnet and VLAN 10. Separate HR, IT and DMZ security zones and inter-VLAN isolation are not implemented in this version.

## Technologies

- FortiGate 7.2.4
- EVE-NG
- Cisco IOSvL2
- VPCS
- DHCP
- DNS
- NAT
- Firewall Policies
- ICMP

## Author

Burak Kılıç

Network & Security Engineering Portfolio Project

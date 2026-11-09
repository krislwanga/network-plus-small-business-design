# Small Business Network Design

## Project Overview

This project demonstrates the design of a small business network for a fictional nonprofit organization called Helping Hands.

The project was created as part of my CompTIA Network+ studies and focuses on network design, VLAN segmentation, Layer 3 switching, DHCP planning, access control, and network security.

## Business Requirements

The organization requires:

- 25 Staff Members
- 2 Wireless Access Points
- 2 Network Printers
- 6 VoIP Phones
- Guest Wireless Access

## Network Devices

- FortiGate 60F Firewall
- Cisco Catalyst 9200 Switch
- Cisco Meraki MR36 Access Points
- Windows Server 2022 DHCP Server

## VLAN Design

| VLAN | Purpose | Network |
|------|---------|---------|
| 10 | Staff | 192.168.10.0/24 |
| 20 | Guest Wi-Fi | 192.168.20.0/24 |
| 30 | Printers | 192.168.30.0/24 |
| 40 | Voice | 192.168.40.0/24 |

## Security Controls

- Guest Wi-Fi isolated from Staff network
- Separate Printer VLAN
- Separate Voice VLAN
- Perimeter firewall protection

## Network Diagram


<img width="1482" height="1232" alt="network-diagram-v4" src="https://github.com/user-attachments/assets/ebf1089a-bd27-46b8-b221-08b72ed77ea7" />


## Network Architecture

Internet traffic enters through a FortiGate 60F firewall and connects to a Cisco Catalyst 9200 core switch. The switch provides connectivity to staff workstations, wireless access points, network printers, and VoIP phones. Network traffic is segmented using VLANs to improve security and network performance.

## Security Architecture

The network uses security segmentation and ACLs to control communication between VLANs.

### Security Zones

| Zone | Purpose |
|------|---------|
| Trusted Zone | VLAN 10 |
| Untrusted Zone | VLAN 20 |
| Restricted Zone | VLAN 30|
| Voice Zone | VLAN 40 |

### Key Security Controls

- Guest Wi-Fi isolated from internal resources
- VLAN segmentation
- ACL-based traffic restrictions
- Firewall protection
- Least Privilege access model

## Project Documentation

### Network Documentation

-ip-addressing-plan.md
-switch-port-map.md

### Security Documentation

-acl-policy.md
-firewall-rules.md

## Skills Demonstrated

### Networking

- Network Design
- VLAN Segmentation
- Inter-VLAN Routing
- IPv4 Addressing
- Subnetting
- TCP/IP Concepts
- Wireless Networking
- Trunking (802.1Q)
- Layer 3 Switching

### Security 

- Network Segmentation
- Access Control Lists (ACLs)
- Firewall Rule Development
- Guest Network Isolation

### Documentation

- Network Diagramming
- Technical Documentation
- GitHub Portfolio Management

## Project Evolution

### Version 1

- Initial topolgy
- VLAN segmentation

### Version 2

- DHCP Server
- DHCP Scopes
- Default Gateways
- 802.1Q trunking

### Version 3

- Layer 3 Switching
- Switch Virtual Interfaces (SVIs)
- Inter-VLAN Routing
- Switch Port Mapping

### Version 4

- ACL Policies
- Security Zones
- Firewall Rules
- Traffic Flow Restrictions

## Lessons Learned

While creating this project, I gained experience with:

- Designing a small business network from requirements
- Implementing VLAN segmentation
- Planning DHCP Scopes
- Creating Layer 3 switching designs
- Developing ACL security policies
- Allocating private IPv4 address space
- Documenting network infrastructure using GitHub
- Maintaining project versions and change history

## Future Improvements

Planned enhancements include:

- Network monitoring implementation
- Redundant Internet connectivity
- High Availability (HA) firewall deployment
- Wireless security enhancements
- Disaster recovery planning
- VPN access for remote workers
- Network Access Control (NAC)

## Project Updates

### Version 2 Enhancements

- Added DHCP Server
- Added DHCP Scope Planning
- Added Default Gateways
- Added VLAN Trunk Link
- Added Guest Wi-Fi Isolation Controls
- Enhanced Security Documentation

### Version 3 Enhancements

- Added Layer 3 switching
- Added Inter-VLAN routing design
- Added Switch Virtual Interfaces (SVIs)
- Added switch port assignments
- Added traffic flow documentation

### Version 4 Enhancements

- Added ACL Policies
- Added Security Zones
- Added Firewall Rule Documentation
- Added Traffic Flow Documentation
- Implemented Least Privilege Design
- Restricted Guest Wi-Fi to internet-only access


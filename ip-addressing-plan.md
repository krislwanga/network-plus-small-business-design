# IP Addressing Plan

## Overview

This document provides the IP addressing plan for the Helping Hands Nonprofit Small Business Network Design.

---

## VLAN 10 - Staff Network

Network Address: 192.168.10.0/24

Subnet Mask: 255.255.255.0

Default Gateway: 192.168.10.1

DHCP Scope:

192.168.10.100 - 192.168.10.199

Devices:

- 25 Staff Workstations

Purpose:

Provides network connectivity for employee computers.

---

## VLAN 20 - Guest Wi-Fi

Network Address: 192.168.20.0/24

Subnet Mask: 255.255.255.0

Default Gateway: 192.168.20.1

DHCP Scope:

192.168.20.100 - 192.168.20.199

Devices:

- Guest Wireless Clients

Purpose:

Provides Internet-only access for guests.

---

## VLAN 30 - Printer Network

Network Address: 192.168.30.0/24

Subnet Mask: 255.255.255.0

Default Gateway: 192.168.30.1

DHCP Scope:

Reserved Static Addresses

Devices:

- Network Printer 1
- Network Printer 2

Purpose:

Dedicated network for shared printers.

---

## VLAN 40 - Voice Network

Network Address: 192.168.40.0/24

Subnet Mask: 255.255.255.0

Default Gateway: 192.168.40.1

DHCP Scope:

192.168.40.100 - 192.168.40.150

Devices:

- 6 VoIP Phones

Purpose:

Dedicated network for voice communications.

---

## Design Considerations

- VLAN segmentation improves security.
- Guest Wi-Fi is isolated from internal resources.
- Printers are separated from user workstations.
- Voice traffic is isolated to support Quality of Service (QoS).
- Default gateways provide inter-VLAN routing capability.

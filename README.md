# Small Business Network Design

## Overview

This project demonstrates the design of a small business network for a fictional nonprofit organization called Helping Hands.

## Business Requirements

- 25 Staff Members
- 2 Wireless Access Points
- 2 Network Printers
- 6 VoIP Phones
- Guest Wireless Access

## Network Devices

- FortiGate 60F Firewall
- Cisco Catalyst 9200 Switch
- Cisco Meraki MR36 Access Points

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

![Network Diagram](network-diagram.png)

## Skills Demonstrated

- Network Design
- VLAN Segmentation
- IP Addressing
- TCP/IP Concepts
- Wireless Networking
- Network Documentation

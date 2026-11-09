## Access Control List (ACL) Policy

## Purpose

This document defines traffic restrictions between VLANs for the Helping Hands Nonprofit network.

---

## Allowed Traffic

## VLAN 10 - Staff Network

Allowed:

- Internet Access
- Printer Access
- Voice Services Access

---

## VLAN 40 - Voice

Allowed:

-VoIP Services

---

## VLAN 20 - Guest Wi-Fi

Denied:

  - VLAN 10 (Staff)
  - VLAN 30 (Printers)
  - VLAN 40 (Voice)

Allowed:

  - Internet Access Only

---

## Security Principles

- Network Segmentation
- Least Privilege
- Defense in Depth
- Access Control

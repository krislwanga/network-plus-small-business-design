## Firewall Rules

## Rule 1

  -Allow Staff VLAN to access Internet
  
  -Source: VLAN 10
  
  -Destination: Internet
  
  -Action: Allow

---

## Rule 2

  -Allow Staff VLAN access to Printers
  
  -Source: VLAN 10
  
  -Destination: VLAN 30
  
  -Action: Allow

---

## Rule 3

  -Block Guest Wi-Fi access to Staff VLAN
  
  -Source: VLAN 20
  
  -Destination: VLAN 10
  
  -Action: Deny

---

## Rule 4 

  -Block Wi-Fi access to Printers
  
  -Source: VLAN 20
  
  -Destination: VLAN 30
  
  -Action: Deny

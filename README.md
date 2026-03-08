# Network Config Builder

A single-page web app that generates network device configuration scripts for **Cisco** and **Juniper** equipment. Choose vendor, device type, OS, and a feature—then fill in parameters to get ready-to-use config snippets. No server or build step required.

## Features

- **Vendors:** Cisco, Juniper  
- **Device types:** Switch, Router  
- **OS support:** Cisco IOS/IOS-XE, NX-OS; Juniper Junos  

### Configuration options

Supported features by platform (✓ = available):

| Feature | Cisco Switch | Cisco Router | Juniper |
|--------|:---:|:---:|:---:|
| **Access & security** | | | |
| Backup Config to TFTP Server | ✓ | ✓ | ✓ |
| Banner MOTD | ✓ | ✓ | ✓ |
| Enable Secret / Password Encryption | ✓ | ✓ | ✓ |
| Line Console 0 | ✓ | ✓ | ✓ |
| Line AUX 0 | ✓ | ✓ | ✓ |
| Line VTY (SSH) | ✓ | ✓ | ✓ |
| Username (Local User) | ✓ | ✓ | ✓ |
| SSH (Hostname, Domain, RSA, VTY) | ✓ | ✓ | ✓ |
| Switch Security with SSH (Full) | ✓ | — | ✓ |
| **Layer 2** | | | |
| VLANs | ✓ | — | ✓ |
| VLAN Trunking | ✓ | — | ✓ |
| Spanning Tree (STP) | ✓ | — | ✓ |
| STP Root Bridge Primary/Secondary | ✓ | — | ✓ |
| Portfast & BPDUGuard (Interface) | ✓ | — | ✓ |
| Enable Global Portfast BPDUGuard | ✓ | — | ✓ |
| Enable Interface Portfast BPDUGuard | ✓ | — | ✓ |
| Port-Security | ✓ | — | ✓ |
| LACP EtherChannel | ✓ | — | ✓ |
| **ACLs** | | | |
| Standard IP ACLs | ✓ | ✓ | ✓ |
| Extended IP ACLs | ✓ | ✓ | ✓ |
| Named ACL (Extended) | ✓ | ✓ | ✓ |
| Insert Extended ACL Entry | ✓ | ✓ | ✓ |
| Delete Extended ACL Entry | ✓ | ✓ | ✓ |
| **IP services** | | | |
| DHCP Server | ✓ | ✓ | ✓ |
| Static Route (IPv4/IPv6) | ✓ | ✓ | ✓ |
| Loopback Address | — | ✓ | ✓ |
| **Routing** | | | |
| OSPF | — | ✓ | ✓ |
| RIPv2 | — | ✓ | ✓ |
| BGP | — | ✓ | ✓ |
| Enable IPv6 Unicast Routing | — | ✓ | ✓ |
| IPv6 OSPFv3 | — | ✓ | ✓ |
| Router on a Stick (ROAS) | — | ✓ | ✓ |
| IPv6 ROAS | — | ✓ | ✓ |
| **Tunnels & VPN** | | | |
| GRE Tunnel | — | ✓ | ✓ |
| IPsec VPN (Site-to-Site) | — | ✓ | ✓ |
| NAT Overload (PAT) | — | ✓ | ✓ |
| **Redundancy** | | | |
| HSRP | ✓ | ✓ | — |
| VRRP | — | — | ✓ |

- **Dark mode** — toggle with preference saved in the browser  
- **Copy to clipboard** and **Download .txt** for the generated script  
- **Editable output** — Cisco output omits `!` comment lines; Juniper uses `#` for inline notes. You can edit the script in the text area before copying or downloading.

## Usage

1. Open `index.html` in a modern browser (no server required).  
2. Select **Vendor**, **Device Type**, and **OS**.  
3. Choose **Feature to Configure** and fill in the parameters.  
4. The script updates as you type. Copy or download, and edit in the text area if needed.

## Tech

- Plain HTML, CSS, and JavaScript—no build step or dependencies.  
- Theme and dark mode use CSS custom properties and `localStorage`.

## License

Use and modify as you like.

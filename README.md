# Network Config Builder

A single-page web app that generates network device configuration scripts for **Cisco** and **Juniper** equipment. Choose vendor, device type, OS, and a feature—then fill in parameters to get ready-to-use config snippets.

## Features

- **Vendors:** Cisco, Juniper  
- **Device types:** Switch, Router  
- **OS support:** Cisco IOS/IOS-XE, NX-OS; Juniper Junos  

### Configuration options

| Feature | Cisco | Juniper |
|--------|--------|---------|
| VLANs | ✓ | ✓ |
| Spanning Tree (STP) | ✓ | ✓ |
| Portfast & BPDU Guard | ✓ | ✓ |
| Access Control Lists (ACL) | ✓ | ✓ |
| DHCP Server | ✓ | ✓ |
| Static Route (IPv4/IPv6) | ✓ | ✓ |
| GRE Tunnel | ✓ | ✓ |
| IPsec VPN (Site-to-Site) | ✓ | ✓ |
| HSRP | ✓ | — |
| VRRP | — | ✓ |

- **Dark mode** toggle with preference saved in the browser  
- **Copy to clipboard** and **Download .txt** for the generated script  
- Output is command-only (no comment lines); you can edit the script in the text area  

## Usage

1. Open `index.html` in a modern browser (no server required).  
2. Select **Vendor**, **Device Type**, and **OS**.  
3. Choose **Feature to Configure** and fill in the parameters.  
4. Use the generated script in the text area: copy or download, and edit if needed.  

## Tech

- Plain HTML, CSS, and JavaScript—no build step or dependencies.  
- Theme and dark mode use CSS custom properties and `localStorage`.  

## License

Use and modify as you like.

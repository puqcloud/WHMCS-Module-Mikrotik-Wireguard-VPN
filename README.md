# Description

### Mikrotik WireGuard VPN module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/store/whmcs-module-mikrotik-wireguard-vpn) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/) | [FAQ](https://community.puqcloud.com/)

## PUQ Mikrotik WireGuard VPN — WHMCS Server Module

**PUQ Mikrotik WireGuard VPN** is a WHMCS server provisioning module for automated deployment of WireGuard VPN accounts on Mikrotik routers. The module communicates with Mikrotik via REST API and provides full lifecycle management of VPN services including creation, suspension, unsuspension, termination, and package changes.

---

## Key Features

- **Automatic WireGuard VPN provisioning** — create and deploy VPN accounts on Mikrotik routers automatically
- **Full lifecycle management** — suspend, unsuspend, terminate, and change packages
- **Mikrotik REST API only** — communicates via Mikrotik REST API (RouterOS 7+)
- **Bandwidth speed limits** — configurable upload/download speed limits per product using Mikrotik Simple Queues
- **Private and public IP support** — assign IPs from a configurable pool per server
- **Metric billing** — usage-based billing for incoming and outgoing traffic (GB)
- **WireGuard configuration export** — text and QR code formats for easy client setup
- **VPN connection status monitoring** — real-time endpoint, handshake, and transfer info
- **VPN interface reboot** — reset frozen connections from client or admin area
- **Traffic statistics** — daily and monthly traffic charts with Google Charts (can be disabled per product)
- **Multilingual interface** — 25 languages: Arabic, Azerbaijani, Catalan, Chinese, Croatian, Czech, Danish, Dutch, English, Estonian, Farsi, French, German, Hebrew, Hungarian, Italian, Macedonian, Norwegian, Polish, Romanian, Russian, Spanish, Swedish, Turkish, Ukrainian
- **Custom links** — configurable links to setup instructions and VPN client downloads in client area

---

## Available Options in the Admin Panel

- Create / Suspend / Unsuspend / Terminate users
- Change package (update bandwidth limits and WireGuard interface)
- VPN connection status and peer information
- VPN interface reboot function
- Text and QR code configuration display
- Metric Billing (Bandwidth Usage Download/Upload in GB)

---

## Available Options in the Client Panel

- VPN connection status (endpoint, handshake, RX/TX)
- Text and QR code configuration with download button
- VPN interface reboot function
- Traffic statistics with daily and monthly charts
- Links to user manual and VPN client downloads

---

## System Requirements

| Requirement | Minimum |
|-------------|---------|
| **WHMCS** | 9.x+ |
| **PHP** | 8.2+ |
| **ionCube Loader** | v13 or newer (v14, v15) |
| **Mikrotik RouterOS** | 7+ |

---

## Important Notes

- The upload and download speed settings in the WHMCS module register the opposite values on the Mikrotik router (e.g., download speed in WHMCS = upload speed in Mikrotik).
- To ensure proper VPN functionality, the administrator must correctly configure the Mikrotik router: NAT, Firewall, routing, and all required settings for VPN to operate correctly.

---

## Links

- **Product page:** [https://puqcloud.com/](https://puqcloud.com/)
- **Documentation:** [https://doc.puq.info/books/mikrotik-wireguard-vpn-whmcs-module](https://doc.puq.info/books/mikrotik-wireguard-vpn-whmcs-module)
- **Support:** [https://puqcloud.com/submitticket.php](https://puqcloud.com/submitticket.php?step=2&deptid=1)
- **Community:** [https://community.puqcloud.com/](https://community.puqcloud.com/)

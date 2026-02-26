# Changelog

### Mikrotik WireGuard VPN module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/store/whmcs-module-mikrotik-wireguard-vpn) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/) | [FAQ](https://community.puqcloud.com/)

## v3.1 — 2026-02-26

### New Features

- Added option to disable traffic statistics collection per product
- When statistics collection is disabled, traffic data is not collected and the statistics page is hidden from the client area

---

## v3.0 — 2026-02-02

### Changes

- Support for WHMCS 9+ with redesigned product module settings
- Updated client area interface design
- New admin settings UI with custom panels (Mikrotik & Bandwidth, WireGuard Configuration, History, Client Area)
- Configuration stored as JSON in configoption24 instead of individual config options

> **Warning:** Product reconfiguration is required after update from v2.x.

---

## v2.0 — 2024-09-23

### Changes

- Module is coded with ionCube v13
- Supports PHP 7.4, 8.1, and 8.2 with WHMCS 8.11.0 and later versions

---

## v1.3 — 2024-07-29

### New Features

- Added metric pricing for incoming and outgoing traffic (Bandwidth Usage Download/Upload in GB)

---

## v1.2 — 2024-06-17

### New Features

- Implemented VPN interface reboot capability for connection resets

### Improvements

- Improved mobile client area adaptation
- Minor translation adjustments

---

## v1.1 — 2023-12-15

### New Features

- Package change functionality introduced

### Improvements

- Minor administrative and client interface modifications

---

## v1.0 — 2023-10-09

First release.

### Features

- Automatic creation and deployment of WireGuard VPN accounts on Mikrotik routers
- Suspend, unsuspend, and terminate VPN accounts
- Integration with Mikrotik REST API only (RouterOS 7+)
- Configurable bandwidth speed limits (upload/download)
- Support for private and public IP addresses
- IP address pool management per server
- Text and QR code WireGuard configuration formats
- VPN connection status monitoring (endpoint, handshake, RX/TX)
- Traffic statistics with daily and monthly charts
- Client area with configuration download and connection info
- Admin area with peer management and API status
- Multilingual support (25 languages)
- License verification system

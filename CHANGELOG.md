# Changelog

### Mikrotik WireGuard VPN module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/whmcs-module-mikrotik-wireguard-vpn.php) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/) | [Community](https://community.puqcloud.com/)

## v4.1.0 — 2026-09-30

- **Fault-Tolerant Cron & Usage Tracking.** Daily usage updates and metric harvesting tasks in WHMCS automation are now strictly isolated per WireGuard service. Any momentary network loss or unreachable router will be safely logged without interrupting the synchronization of remaining customer accounts.
- **PHP 8.x Type Safety Hardening.** Thoroughly hardened typed property handling across bandwidth and package limits, preventing `TypeError` exceptions on PHP 8.1, 8.2, and 8.3 environments.
- **Zero-Touch Settings Auto-Migration.** Existing WireGuard products configured on legacy schemas automatically upgrade their settings into modern unified parameters (`configoption24`) upon product saving, ensuring smooth maintenance.
- **Enhanced Select2 & WHMCS 9 Admin UX.** Upgraded dynamic settings panel detection to guarantee instant and reliable form reactivity across WHMCS 9 and Select2 interfaces.
- **Clean Module Logging.** Excluded local database license verification checks (`License_Verification (db)`) from the WHMCS Module Log, recording exclusively online verification calls to keep diagnostic logs clean.

---

## v4.0.0 — 2026-09-22

- **WireGuard Simple Queue and metric collection fix.** Resolved router 404 errors caused by slashes (`%2F`) in Base64 public keys in REST API paths by introducing `apiFindQueue()` with dedicated IP (`target=.../32`) and query-parameter lookups. Queue deletion and counter resets are now executed reliably via internal RouterOS `.id`.
- **Atomic traffic statistics collection.** Replaced read-modify-write logic with atomic SQL increments (`Capsule::raw`) in `StatisticsSaveTraffic()`, eliminating race conditions and traffic data loss during concurrent WHMCS cron jobs and metric queries.
- **WHMCS Usage Billing MetricProvider fix.** Resolved zero-traffic reporting so that `Usage(0.0)` is reliably returned when usage is 0 GB, preventing "No usage data" statuses in WHMCS.
- **Human-readable Transfer RX & TX units.** Replaced raw byte integers in the client area with dynamically formatted units (`B`, `KB`, `MB`, `GB`, `TB`) with 2-decimal precision.
- **Admin API connection timeout and performance optimization.** Enforced a strict 15-second timeout on router status checks and removed early blocking API calls from constructor, eliminating admin panel delays and cron execution lags.
- **PHP 7.4 & PHP 8.x compatibility.** Resolved syntax compatibility issues across PHP 7.4 through PHP 8.4.
- **ionCube 15 & PHP 8.2+ architectural upgrade.** Transitioned `hooks.php` to an unencoded lightweight bootstrap delegating logic to `lib/puqMikrotikWireGuardVPNHooks.php` for seamless ionCube 15 compatibility.
- **Automated usage cleanup on termination.** Local usage statistics in `puqMikrotikWireGuardVPN_statistics` are now automatically purged when a service is terminated.
- **Enhanced Client Area UI.** Integrated standard PUQ client area UI toolkit with `header.tpl`, QR code rendering, dynamic config download, copy-to-clipboard, CSRF protection, and streamlined layout.
- **Legacy configuration fallback.** Added transparent backward compatibility for products migrating from older configuration schemas.

---

## v3.2.1 — 2026-06-02

- **Full compatibility with the latest Mikrotik RouterOS 7.21.4.** The module has been tested and certified against RouterOS 7.21.4, so you can confidently run the newest firmware on your routers without any provisioning hiccups.
- **Rock-solid REST API connections.** Resolved rare cases where requests to the router could stall and time out, leaving operations hanging. Account creation, suspension, statistics collection and status checks now complete instantly and reliably.
- **Snappier, more dependable automation.** With every API call responding without delay, day-to-day provisioning and billing run faster and smoother — fewer retries, no stuck tasks, and a more responsive experience for both your team and your customers.
- **PHP 7.4 support restored.** The module once again runs on PHP 7.4 in addition to PHP 8.x, so hosting environments that have not yet migrated to PHP 8 can keep using the latest version. PHP 7.4 will remain supported for as long as it is technically possible to do so.

---

## v3.2 — 2026-04-21

- **Improved stability across the WHMCS admin area.** Rare page-loading errors that could appear on some admin screens (for example when opening a support ticket on installations with non-standard file layouts, symlinks or custom hosting paths) have been eliminated. The admin panel now loads smoothly in every environment.
- **Greater compatibility with complex hosting setups.** The module is now fully resilient to WHMCS installations using symlinked directories, multi-domain hosting and custom include paths.
- **Smoother day-to-day operation for administrators.** Fewer interruptions, no unexpected "Oops!" pages, and a more predictable experience when working with tickets, clients and services — so your team can focus on customers, not on troubleshooting.

---

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

# WHMCS Setup (Install / Update)

### Mikrotik WireGuard VPN module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/store/whmcs-module-mikrotik-wireguard-vpn) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/) | [FAQ](https://community.puqcloud.com/)

## System Requirements

| Requirement | Minimum |
|-------------|---------|
| **WHMCS** | 9.x+ |
| **PHP** | 8.2+ |
| **ionCube Loader** | v13 or newer (v14, v15) |

---

## Download

Download the latest version of the module:

```bash
wget https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/php82/PUQ_WHMCS-Mikrotik-WireGuard-VPN-latest.zip
```

Unzip the archive:

```bash
unzip PUQ_WHMCS-Mikrotik-WireGuard-VPN-latest.zip
```

---

## Installation

**Step 1.** Download and unzip the module archive (see above).

**Step 2.** Copy the `puqMikrotikWireGuardVPN` directory to your WHMCS installation:

```
WHMCS_WEB_DIR/modules/servers/puqMikrotikWireGuardVPN
```

The resulting directory structure should look like:

```
modules/
  servers/
    puqMikrotikWireGuardVPN/
      puqMikrotikWireGuardVPN.php
      hooks.php
      lib/
      templates/
      lang/
      ...
```

**Step 3.** The module is ready to use. Proceed to configure a server and product in WHMCS.

---

## Update

The update process is identical to the installation — simply download the latest version and replace the existing `puqMikrotikWireGuardVPN` directory.

> **Note:** When updating from v2.x to v3.x, product reconfiguration is required due to the new settings storage format.

---

## Legacy Versions

For older WHMCS versions (8.x), legacy module builds are available:

- **All versions:** [https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/)
- **PHP 7.4:** [https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/php74/](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/php74/)
- **PHP 8.1:** [https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/php81/](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/php81/)

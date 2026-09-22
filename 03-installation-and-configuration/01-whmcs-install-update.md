# WHMCS Installation and Update

### Mikrotik WireGuard VPN module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/whmcs-module-mikrotik-wireguard-vpn.php) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/) | [Community](https://community.puqcloud.com/)

## System requirements

| Requirement | Minimum |
|-------------|---------|
| **WHMCS** | 8.x+, 9.x+. |
| **PHP** | 7.4, 8.1, 8.2, 8.3, 8.4 |
| **ionCube Loader** | v15+ |
| **Mikrotik RouterOS** | 7.x+ |

> **Note:** The module uses ionCube encoding. Make sure ionCube Loader is installed and active on your server.

## Installation

> **Note:** The module now uses **ionCube 15**, which provides universal out-of-the-box support for all encodings.
>
> All versions can be found at this link:
> `https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/`
>
> Older module versions for WHMCS 8 are available in the archive directory:
> `https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/archive/`

1. Download the latest version from the PUQ download page:
   ```bash
   wget https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/PUQ_WHMCS-Mikrotik-WireGuard-VPN-latest.zip
   ```

2. Unzip the archive:
   ```bash
   unzip PUQ_WHMCS-Mikrotik-WireGuard-VPN-latest.zip
   ```

3. Copy the `puqMikrotikWireGuardVPN` directory into your WHMCS installation under `modules/servers/`:
   ```bash
   cp -r puqMikrotikWireGuardVPN /path/to/whmcs/modules/servers/
   ```

   The resulting directory structure should look like:
   ```text
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

## Update

The update process is identical to the installation:

1. Download the latest archive from the download page:
   ```bash
   wget https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Mikrotik-WireGuard-VPN/PUQ_WHMCS-Mikrotik-WireGuard-VPN-latest.zip
   ```

2. Unzip the archive:
   ```bash
   unzip -o PUQ_WHMCS-Mikrotik-WireGuard-VPN-latest.zip
   ```

3. Replace the existing `puqMikrotikWireGuardVPN` directory in your WHMCS installation:
   ```bash
   cp -r puqMikrotikWireGuardVPN /path/to/whmcs/modules/servers/
   ```

> **Warning:** When updating from v2.x to v3.x+, product reconfiguration is required due to the new settings storage format.

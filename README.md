# Guardzera releases

Download Guardzera, the all-in-one VPN client for WireGuard and PPTP (FortiVPN, OpenVPN, Outline and Cisco AnyConnect coming soon).

**[Latest release](https://github.com/zerazyrus/guardzera-releases/releases/latest)**

| Platform | File |
|---|---|
| macOS, Apple Silicon (M1 and later) | `Guardzera-macos-arm64.dmg` |
| Windows 10/11, x64 | `Guardzera-windows-x64-setup.exe` |

The app checks this page for new versions and updates itself.

## First launch on macOS

Builds are not notarized yet, so macOS blocks the first launch. After copying Guardzera to Applications, run once:

```sh
xattr -dr com.apple.quarantine /Applications/Guardzera.app
```

## Third-party components

- `pptp` (macOS): built from pptp-linux 1.10.0, GPL-2.0. Source: https://sourceforge.net/projects/pptpclient/files/pptp/pptp-1.10.0/
- `wireguard.dll` (Windows): WireGuardNT 1.1 by WireGuard LLC, redistributed unmodified under its Prebuilt Binaries License: https://download.wireguard.com/wireguard-nt/
- boringtun (BSD-3-Clause), Tauri (MIT / Apache-2.0).

"WireGuard" is a registered trademark of Jason A. Donenfeld. Guardzera is not affiliated with or endorsed by the WireGuard project.

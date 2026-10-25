# Sunday Operational Council desktop releases

Official compiled SOC installers and cryptographically signed update manifests for macOS Apple Silicon and Windows x64/ARM64.

This repository contains distribution binaries only. It contains no private Council source, records, account/device credentials, signing private keys or recovery keys.

## Install
Download SOC-Windows-0.7.0.zip from the v0.7.0 release on Windows, extract the whole folder, then open Install-Council.cmd. The installer detects x64 or ARM64. macOS uses SOC-0.7.0-macos-arm64.zip. Keep normal operating-system security protections.

The first Windows native installation and actual audible reminder delivery must be checked on the recipient device. Windows binaries are not Authenticode-signed; update manifests use a separately pinned RSA signature. macOS is ad-hoc signed. Do not bypass a security block.

## Updates
SOC checks the signed stable manifest once a day when opened. It verifies release version, expiry, platform, architecture, signature and package hashes. New desktop updates stage separately from reminders and account data, and wait for saved work and a safe restart. The update host does not require the Council work server or the owner Mac.

Shared work remains protected at https://council.tomecast.world/ and uses each member's own identity and the existing runtime-budget controls.

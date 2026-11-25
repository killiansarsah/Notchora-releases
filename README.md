# Notchora â€” Official Production Releases

[![Release](https://img.shields.io/badge/Release-v1.0.0--Genesis-blue.svg)](https://github.com/killiansarsah/Notchora-releases)
[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011%20(x64)-black.svg)](https://github.com/killiansarsah/Notchora-releases)
[![Status](https://img.shields.io/badge/Status-Production%20Ready-green.svg)](https://github.com/killiansarsah/Notchora-releases)

This repository contains official production distribution binaries, installers, and release checksums for **Notchora** â€” the Apple Dynamic Island experience for Windows.

---

## Downloads

| Package | Format | File Size | Description |
| :--- | :--- | :--- | :--- |
| **[NotchoraSetup.exe](NotchoraSetup.exe)** | 1-Click Installer | ~57.8 MB | Recommended. Automatically installs Notchora to `%LocalAppData%\Programs\Notchora`, registers Start Menu & Desktop shortcuts, and provisions background helpers. |
| **[Notchora-v1.0.0-win-x64.zip](Notchora-v1.0.0-win-x64.zip)** | Portable Archive | ~57.7 MB | Standalone portable bundle. Extract to any folder and run `Notchora.exe` directly without administrative elevation. |

---

## Release Verification & SHA-256 Checksums

Verify your downloaded binary using PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 .\NotchoraSetup.exe
```

| File Name | SHA-256 Checksum |
| :--- | :--- |
| `NotchoraSetup.exe` | `447ff81828b9f1debdba1b06719cbbd04926bbf46ac0ea6bff085d29490b3dd5` |
| `Notchora-v1.0.0-win-x64.zip` | `4dc90311f15a225e7a6f62b600dbc4220b76336834944b98aefe376565a4b7a5` |

Official checksum file: [`SHA256SUMS.txt`](SHA256SUMS.txt)

---

## What's New in v1.0.0 â€” Genesis Edition

### Dynamic Island Engine & Spring Physics
* **High-Fidelity Differential Spring Solver** ($k=360, c=27.5, \zeta=0.725$): Zero oscillation, instant interruption momentum preservation, and convergence in $\le 200\text{ ms}$.
* **Multi-Dock Orientations**: Top horizontal dock ($189 \times 27\text{ px}$), Left & Right side docks ($42 \times 124\text{ px}$) with automatic rotation and layout reflow.
* **Apple Concentric Geometry**: Mathematical inner/outer corner radius matching ($R_{\text{inner}} = 16\text{ px}$, $R_{\text{outer}} = 28\text{ px}$) across all expanded cards.

### Notchora Drop (AirDrop Companion)
* **Intelligent Tri-Zone SmartDrop**: Drag files over the notch to instantly route to **Send to Phone** (Wi-Fi Drop), **File Shelf** (temporary holding), or **Convert Format** (instant document/image transcoding).
* **Self-Contained DropHost**: Bundled single-file win-x64 .NET 10 web server for lightning-fast file streaming to any iOS or Android phone on your local network.
* **Interactive Send Pill**: Real-time link/note input box with high-contrast icon rendering and resting/active opacity states.

### Power, Battery & Hardware Intelligence
* **Instant Detection** ($\le 80\text{ ms}$): Dynamic Island charging bolt alerts, debounced AC cable flapping protection, and high-visibility 10% critical battery warnings.
* **Focus Immunity**: Power events smoothly badge inside the header without shrinking or collapsing active tools.

### Production Hardening
* **Zero Resource Leaks**: GDI and User object leak audit passed with strictly $\Delta = 0$ over 50+ continuous morphing cycles.
* **100% Automated QA Verification**: Passed all 14 phases (195/195 tests) under the UASET G6 Quality Gate.

---

## System Requirements
* **OS:** Windows 10 (Version 1903+) or Windows 11 (x64)
* **Architecture:** 64-bit (x64)
* **Dependencies:** None (All runtimes and WebView2 bootstrapper are self-contained)

---

## License & Support
Notchora is proprietary software. All rights reserved.  
Source code repository: [killiansarsah/Notchora](https://github.com/killiansarsah/Notchora)

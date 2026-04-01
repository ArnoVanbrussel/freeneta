# FreeNeta

Lightweight **PROFINET discovery and commissioning tool** written in Python.

FreeNeta allows you to quickly discover and configure PROFINET devices using **DCP** without needing heavyweight vendor tools.

The project started because downloading Siemens **PRONETA** requires creating an account and registering personal details just to access a "free" tool. FreeNeta aims to provide a **simple, lightweight, open-source alternative** for basic discovery and diagnostics.

FreeNeta is meant as a lightweight quick-scan tool, not a full replacement for Proneta.

---

## Features

- Discover PROFINET devices via **DCP**
- View **station name, MAC, vendor, IP, subnet, gateway**
- **Vendor lookup** via MAC OUI
- **DCP access detection (read-only vs read-write)** using raw DCP response analysis
- **Ping monitoring** for device reachability
- Set **device IP address**
- Set **station name**
- Reset **communication parameters**
- **Quick connect** actions (HTTP / HTTPS / SSH)
- **Visual topology overview** of discovered devices

---

## Requirements (Windows)

FreeNeta v1.5 uses packet capture to determine DCP access levels.

👉 This requires **Npcap** to be installed:

https://nmap.org/npcap/

Recommended install options:
- Install Npcap in **WinPcap API-compatible Mode**

⚠️ Without Npcap:
- Device discovery still works
- **Read-only / read-write detection will NOT work**

---

## Notes

- Running FreeNeta as **Administrator** may be required for packet capture
- If devices show no access status, check that Npcap is installed correctly

---

## Screenshot

![FreeNeta UI](/images/FreeNeta-v1.5-screenshot.png)

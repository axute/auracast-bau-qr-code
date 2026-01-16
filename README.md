# Auracast BAU QR Generator (Pro)

A lightweight, browser‑based tool for generating **Broadcast Audio URI (BAU)** QR codes for Auracast™‑compatible Bluetooth LE Audio transmitters.  
The generator runs entirely client‑side and requires no backend, no data storage, and no external services.

This project is intended for developers, testers, and hobbyists working with BLE Audio broadcast devices who want a simple way to create BAU‑formatted QR codes for pairing and configuration.

---

## Features

- Full support for **BAU v1.0 field structure**:
  - `BN` – Broadcast Name (Base64)
  - `BI` – Broadcast ID (Hex)
  - `AT` – Announcement Type
  - `SQ` – Sequence Number
  - `BC` – Broadcast Code / Password (Base64)
  - `AD` – Announcement Data (Hex)
  - `AS` – Audio Stream Count
  - `NS` – Number of Subgroups
  - `NB` – Number of BIS
  - `BS` – BIS Mask (Hex)
  - `PI` – Presentation Info (Hex)
  - `SM` – Service Metadata (Base64)

- Automatic Base64 encoding for BN and BC  
- Automatic Hex normalization for BI, AD, BS, PI  
- Built‑in presets (public, encrypted, mono, stereo)  
- Live QR code preview  
- Export QR code as PNG  
- Copy BAU string to clipboard  
- Fully mobile‑friendly UI  
- 100% offline — all processing happens in the browser

---

## Usage

1. Open the hosted page (GitHub Pages or local file).  
2. Enter your Auracast broadcast parameters:
   - Broadcast Name
   - Broadcast ID
   - Optional password
   - Audio configuration fields
3. The BAU string and QR code update instantly.
4. Scan the QR code with an Auracast‑capable device to join the broadcast.
5. Enhanced documentation, you will find here: https://www.bluetooth.com/specifications/specs/html/?src=BAU_v1.0/out/en/index-en.html
---

## Hosting

This project is designed to run directly on **GitHub Pages**:

1. Upload `index.html` to your repository  
2. Enable GitHub Pages (Settings → Pages → Deploy from branch)  
3. Access the tool at:

https://axute.github.io/auracast-bau-qr-code/index.html

No server or build step required.

---

## Technology

- **HTML + Vanilla JavaScript**
- **QRCode.js** (MIT licensed)
- No frameworks, no dependencies, no tracking

---

## Disclaimer

This is an **unofficial** tool created for educational and interoperability testing purposes.  
It is **not affiliated with the Bluetooth SIG** or any hardware manufacturer.  
Auracast™ is a trademark of the Bluetooth SIG.

---

## License

This project is released under the **MIT License**.  
See `LICENSE` for details.

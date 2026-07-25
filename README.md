# UI Components — iOS 27 & Samsung OneUI 8 / 8.5 / 9 System Icons & Vectors

Official extracted system icons, vector glyphs, app logos, fonts, and metadata for **iOS 27 (Apple SF Symbols 8)** and **Samsung OneUI 8 / 8.5 / 9 (Galaxy S26 Ultra)**.

## 📱 Repository Overview

| System | Target OS | Extracted Vectors | Fonts | Key Features |
| :--- | :--- | :--- | :--- | :--- |
| **iOS** | iOS 27 | 7,473 SVG files across 30 categories | `SF-Pro.ttf`, `SF-Compact.ttf`, `SFSymbolsFallback.otf` | Apple SF Symbols 8, App Icons, Metadata Plists |
| **Samsung OneUI** | OneUI 8 / 8.5 / 9 | System Nav, Quick Settings, Status Bar, Settings, Galaxy AI | N/A | OneUI Squircles, App Icons, Firmware Extractor Pipeline |

---

## 📂 Directory Layout

- **[`iOS/`](./iOS)**: Extracted SF Symbols 8 vector glyphs, SF Pro variable fonts, system badges, app icons, and full JSON metadata map.
- **[`OneUI/`](./OneUI)**: Extracted OneUI 8/8.5/9 vector icons (Galaxy AI 3.0, Quick Settings, Status Bar, Gestural Navigation), squircle app icons, and automated Samsung AP firmware extraction script.

---

## 🛠️ Extraction Scripts
- iOS extraction pipeline powered by Apple SF Symbols 8 CPIO/XAR payload decompressor and OpenType CFF2 vector parser.
- OneUI firmware extraction script: `OneUI/scripts/extract_samsung_firmware.py` for parsing `AP_*.tar.md5` and Android VectorDrawable XMLs.

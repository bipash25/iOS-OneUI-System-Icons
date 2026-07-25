# Samsung OneUI 8 / 8.5 / 9 System Icons, Vectors & App Icon Library

Extracted vector assets and automated firmware pipeline for **Samsung OneUI 8, OneUI 8.5, and OneUI 9** (Samsung Galaxy S26 Ultra / S25 Series).

## 📂 Extracted Directory Structure

```
OneUI/
├── Frija_v2.0.26142.10.zip     # Official Samsung Firmware Downloader tool
├── extracted_assets/
│   ├── app_icons/              # Official Samsung OneUI squircle app icons (Gallery, Camera, Phone, Settings, Notes, Health, Wallet, Bixby, Device Care, Members, etc.)
│   ├── vectors/                # Categorized Vector XML & SVG icons
│   │   ├── galaxy_ai/          # Circle to Search, Live Translate, Generative Edit, AI Stars, Audio Zoom, Sketch to Image, Now Bar
│   │   ├── quick_settings/     # Wi-Fi, Bluetooth, Flashlight, Smart View, DND, Flight Mode
│   │   ├── status_bar/         # Battery, 5G, Wi-Fi 7, Signal, Alarm, Vibration
│   │   ├── system_nav/         # OneUI gestural bar, back, home, recents
│   │   └── settings_icons/     # OneUI Settings category vector drawables
│   └── metadata/               # oneui_icons_metadata.json (squircle radius, app package IDs, icon list)
└── scripts/
    └── extract_samsung_firmware.py  # Automated python firmware decompressor & VectorDrawable XML -> SVG converter
```

## 🛠️ Samsung Firmware Extraction Guide (OneUI 8 / 8.5 / 9)
To unpack assets directly from a downloaded Samsung Firmware `.tar.md5` package (e.g. Galaxy S26 Ultra / S25):

1. **Download AP via Frija**: Use `Frija.exe` to fetch official firmware for model `SM-S928B` / `SM-S938B`.
2. **UnLZ4 System Image**: `lz4 -d AP_*.tar.md5/system.img.lz4 system.img`
3. **Mount/Extract System APKs**: Unpack `/system/framework/framework-res.apk`, `/system/priv-app/SamsungOneUIHome/SamsungOneUIHome.apk`, `/system/priv-app/SecSettings/SecSettings.apk`, and `/system/priv-app/SystemUI/SystemUI.apk`.
4. **Run Extraction Script**: `python3 scripts/extract_samsung_firmware.py`

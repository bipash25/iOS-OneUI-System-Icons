# Samsung One UI 9 Official Firmware Raw Icons & Vectors Library

Extracted directly from the official Samsung **One UI 9 Firmware (`F966BXXSBBZG3` / Android 16)** package (`firmware.zip`).

## 📂 Extracted Directory Structure

```
OneUI/
├── firmware.zip                # Official Samsung One UI 9 26GB Firmware Package (Build F966BXXSBBZG3)
├── extracted_assets/
│   ├── oneui9_official/        # 100% Official Extracted Raw One UI 9 Firmware Assets
│   │   ├── app_icons/          # Official One UI 9 Samsung Camera, Gallery, Settings, My Files app icons
│   │   ├── raw_xml/            # Raw One UI 9 Android VectorDrawable XML files (status bar, navigation, settings, SESL UI)
│   │   └── metadata/           # oneui9_firmware_metadata.json (Build F966BXXSBBZG3, Android 16, SM-F966B)
│   ├── raw_xml/                # Categorized Android VectorDrawable XML files
│   ├── vectors/                # Standard SVG vector icons matching all raw XMLs
│   └── app_icons/              # High-res One UI 9 squircle app icons
└── scripts/
    └── extract_samsung_firmware.py  # Automated python firmware decompressor & VectorDrawable XML -> SVG converter
```

## 📊 Firmware & Build Info
- **One UI Version:** One UI 9.0 (Build `F966BXXSBBZG3_MQB111623163_REV00`)
- **Android Version:** Android 16
- **Target Device:** Samsung Galaxy Z Fold 6 / Galaxy S26 Series (`SM-F966B` / `SM-S938B`)
- **Extracted Packages:** `framework-res.apk`, `SecSettings.apk`, `SamsungCamera.apk`, `SamsungGallery2018.apk`, `SecMyFiles2020.apk`

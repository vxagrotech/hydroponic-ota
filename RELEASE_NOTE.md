# VX Agrotech Hydroponic Tower
## Firmware Release Notes
---
## Version 2.0.0
Release Date:  16 July 2026

### New Features
- Added GitHub HTTPS OTA firmware update.
- Added manual OTA update using Blynk V40.
- Added OTA status display using Blynk V41.
- Added firmware version management using `FW_VERSION`.
- Added semantic version comparison.
- Added GitHub `version.json` support.

### Improvements
- OTA only starts when requested by the user.
- OTA is blocked while nutrient dosing is active.
- Added OTA progress reporting to Serial Monitor.
- Added OTA progress reporting to Blynk.
- Added firmware validation before reboot.
- Added rollback protection if OTA fails.

### Fixed
- Improved OTA reliability.
- Preserved all existing hydroponic control logic.

### Notes
- Repository: https://github.com/vxagrotech/hydroponic-ota
- OTA deployment:
  1. Export compiled binary
  2. Rename to firmware.bin
  3. Upload firmware.bin
  4. Update version.json
  5. Commit changes
  6. Press OTA button (V40)

---

## Version 2.0.1
Release Date: 21 July 2026

### Fixed
- Prevent duplicate pH status messages in Blynk Terminal.
- Refactored EC and pH status updates to only send changes.
- Reduced unnecessary Blynk traffic.

### Improvements
- Added helper functions:
  - updatePHStatus()
  - updateECStatus()
- Improved Terminal logging consistency.

---

## Version 2.0.2

### Added
- ...

### Fixed
- ...

### Improvements
- ...

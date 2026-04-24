# WM_BKW_ATCMD

## Firmware Binaries

This repository includes the following firmware binaries:

### 1. ATBleService.bin
- Used for creating and managing BLE GATT services during BLE provisioning.
- Must be flashed at the following memory address:
0x1EF000

---

### 2. beken_7238_host_mcu_1.0.1.bin
- Main application firmware for the host MCU.
- Must be flashed at the base address:
0x000000


---

## Flashing Layout

| Binary File                         | Address   | Description                     |
|-----------------------------------|----------|---------------------------------|
| ATBleService.bin                  | 0x1EF000 | BLE GATT service configuration  |
| beken_7238_host_mcu_1.0.1.bin     | 0x000000 | Main application firmware       |

---

## Versioning

The firmware follows semantic versioning.

- **Version: 1.0.1**
  - This version includes a **minor bug fix** over the default `SDK_3.0.x`.
  - No major feature changes; stability improvements only.

---

## Notes
- Ensure correct flashing addresses to avoid boot or provisioning issues.
- It is recommended to erase flash before programming both binaries.

# Changelog (Aqua-DCS)

All notable code changes to this project will be documented in this file.

---

## [Unreleased]

### Added
- `MILESTONES.md` for session restore and milestone tracking.

### Fixed
- DS18B20 1-Wire GPIO pin mapping confusion:
  - Physical pin 7 is **BCM GPIO4**, not BCM7.
  - Use `dtoverlay=w1-gpio-pi5,gpiopin=4` in `/boot/firmware/config.txt`.

### Changed
- DS18B20 driver/collector can pin a specific sensor id via `AQUA_DS18B20_ID`.

# Changelog

All notable changes to GatewayOps Cloud are documented in this file.

This changelog uses plain-language categories so customers, support teams, QA testers, and product stakeholders can quickly understand each release.

## [2.4.0] - 2026-06-15

### Added

- Added a new gateway pairing status panel.
- Added clearer error messages when a sensor fails to pair.
- Added a firmware compatibility warning before pairing starts.
- Added a downloadable gateway health report.

### Changed

- Updated the pairing workflow to show progress in four stages:
  1. Gateway detected
  2. Sensor signal received
  3. Security handshake started
  4. Pairing complete

- Improved dashboard load time for locations with more than 500 sensors.
- Updated the gateway health check page with clearer labels.

### Fixed

- Fixed an issue where offline gateways sometimes appeared as active.
- Fixed an issue where failed pairing attempts did not always appear in the activity log.
- Fixed a bug that caused duplicate sensor names after a retry.
- Fixed incorrect timestamps in exported health reports.

### Breaking Changes

- The `pairing_status` API field now returns `pending`, `in_progress`, `failed`, or `complete`.
- Previous API responses used `true` or `false`.

### Known Issues

- The dashboard may take longer to load for locations with more than 2,000 sensors.
- Firmware warnings may not appear for gateways running firmware earlier than version 1.8.0.

---

## [2.3.1] - 2026-05-22

### Fixed

- Fixed a minor display issue on the gateway detail page.
- Fixed missing help text for signal strength warnings.

---

## [2.3.0] - 2026-05-01

### Added

- Added gateway health check summaries.
- Added sensor count totals to the location dashboard.

### Changed

- Improved error handling for weak signal readings.

### Fixed

- Fixed an issue where some gateways showed outdated firmware status.

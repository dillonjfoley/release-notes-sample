# GatewayOps Cloud 2.4.0 Release Notes

**Release date:** June 15, 2026  
**Release name:** Gateway Pairing Reliability Update  
**Audience:** Technicians, operations teams, support teams, and account administrators

## Summary

GatewayOps Cloud 2.4.0 improves the gateway and sensor pairing experience. This update adds clearer pairing status messages, better firmware warnings, improved health reports, and several fixes for common field troubleshooting issues.

## What's New

### New Gateway Pairing Status Panel

The pairing page now shows each step in the pairing process:

1. Gateway detected
2. Sensor signal received
3. Security handshake started
4. Pairing complete

This helps technicians see where a pairing attempt failed instead of only seeing a general failure message.

### Firmware Compatibility Warning

GatewayOps Cloud now checks gateway firmware before pairing begins.

If a gateway is running older firmware, the dashboard displays a warning before the technician starts the pairing process.

### Downloadable Gateway Health Report

Users can now download a gateway health report from the health check page.

The report includes:

- Gateway name
- Location
- Firmware version
- Last check-in time
- Signal strength
- Paired sensor count
- Open warnings

## Fixed Issues

This release fixes several issues:

- Offline gateways sometimes appeared as active.
- Failed pairing attempts did not always appear in the activity log.
- Retried pairings sometimes created duplicate sensor names.
- Exported health reports sometimes showed incorrect timestamps.

## Known Issues

The following issues are still being worked on:

| Issue | Workaround |
|---|---|
| Large locations with more than 2,000 sensors may load slowly | Filter by building, floor, or gateway group |
| Firmware warnings may not appear for gateways below firmware 1.8.0 | Check firmware manually before pairing |
| Activity log export may take longer during peak usage | Wait one minute and retry the export |

## Breaking Change

The `pairing_status` API field has changed.

Previous values:

```json
true
false

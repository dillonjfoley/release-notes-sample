# Fixed Issues — GatewayOps Cloud 2.4.0

This document lists issues fixed in version 2.4.0.

| ID | Issue | Resolution |
|---|---|---|
| FIX-2387 | Offline gateways sometimes appeared as active | Updated gateway check-in logic |
| FIX-2392 | Failed pairing attempts did not always appear in the activity log | Added event capture for failed pairing states |
| FIX-2398 | Retried pairings sometimes created duplicate sensor names | Added duplicate name validation before retry |
| FIX-2400 | Exported health reports sometimes showed incorrect timestamps | Updated report export timezone handling |

## Verification

QA verified these fixes using:

- Standard gateway configuration
- Weak signal simulation
- Offline gateway simulation
- Duplicate sensor retry test
- CSV health report export test

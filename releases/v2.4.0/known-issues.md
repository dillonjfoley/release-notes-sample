# Known Issues — GatewayOps Cloud 2.4.0

This document lists known issues for the 2.4.0 release.

## Known Issues

| ID | Issue | Impact | Workaround | Status |
|---|---|---|---|---|
| KI-2401 | Large locations with more than 2,000 sensors may load slowly | Medium | Filter by building, floor, or gateway group | Open |
| KI-2402 | Firmware warnings may not appear for gateways below firmware 1.8.0 | Medium | Check firmware manually before pairing | Open |
| KI-2403 | Activity log export may take longer during peak usage | Low | Wait one minute and retry export | Monitoring |

## Escalation Guidance

Escalate to engineering if:

- A gateway shows as online but has not checked in for more than 24 hours.
- A pairing attempt fails at the same stage more than three times.
- A health report cannot be generated after two retries.

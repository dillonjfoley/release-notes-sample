# Upgrade Notes — GatewayOps Cloud 2.4.0

Most dashboard users do not need to take action before using version 2.4.0.

API users should review the breaking change to the `pairing_status` field.

## Before You Upgrade

Review the following:

- Do you use the GatewayOps Cloud API?
- Do any scripts check `pairing_status`?
- Do any dashboards, alerts, or reports expect `pairing_status` to be `true` or `false`?

If yes, update those integrations before upgrading.

## Dashboard Users

No action required.

New features will appear automatically after release.

## API Users

Update any integration that expects this response:

```json
"pairing_status": true

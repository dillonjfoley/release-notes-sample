# Breaking Changes — GatewayOps Cloud 2.4.0

Version 2.4.0 includes one breaking API change.

## API Field Changed: `pairing_status`

The `pairing_status` field now returns a string value instead of a boolean value.

### Previous Response

```json
{
  "gateway_id": "GW-10482",
  "sensor_id": "SN-8831",
  "pairing_status": true
}

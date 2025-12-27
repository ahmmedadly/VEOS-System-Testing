# VEOS API & Communication Testing Summary

VEOS uses a hybrid communication model:
- SOME/IP for real-time vehicle data
- RESTful APIs for cloud-to-mobile communication

## Scope
- Validate correctness of telemetry data sent from VHAL to cloud
- Validate vehicle restriction updates from mobile app
- Verify data consistency across AAOS, cloud, and mobile app

## Limitations
- APIs currently lack authentication mechanisms
- Some vehicle restrictions update VHAL values but do not affect actual car behavior


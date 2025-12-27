# VEOS Test Strategy

## Testing Objectives
- Validate end-to-end vehicle data flow across all system nodes
- Ensure correctness of vehicle telemetry updates
- Identify latency, synchronization, and integration issues
- Validate remote control and restriction mechanisms

## Test Levels
- System Testing
- Integration Testing
- Manual Functional Testing
- Communication Testing (SOME/IP & REST)

## Test Environment
- STM32 (Bare-metal)
- Yocto Linux (Middleware)
- Android Automotive OS (AAOS)
- VEOS Mobile App (Android)
- Cloud Backend (REST APIs)

## Tools
- Android Logcat
- ADB
- Postman (documentation & basic REST validation)
- Network monitoring tools
- Manual test execution


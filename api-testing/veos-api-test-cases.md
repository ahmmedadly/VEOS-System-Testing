# VEOS API Test Cases

## TC_API_001 – Retrieve vehicle telemetry from cloud

**Endpoint:** GET /telemetry/  
**Expected Result:**
- Valid vehicle data returned (speed, gear, temperature)
- Data matches AAOS VHAL values

---

## TC_API_002 – Post vehicle restriction from mobile app

**Endpoint:** POST /vehicle-readings/  
**Expected Result:**
- Restriction value stored successfully
- VHAL property updated

**Actual Result:**
- VHAL updated but restriction not enforced on vehicle

**Status:** Failed

---

## TC_API_003 – API security validation

**Expected Result:**
- API should require authentication

**Actual Result:**
- Endpoints accessible without authentication

**Status:** Failed


## TC_API_004 – REST API without authentication

**Endpoint:** GET /telemetry/

**Expected Result:**
- API should require authentication

**Actual Result:**
- Endpoint accessible without auth

**Status:** Failed

---

## TC_API_005 – Invalid payload handling

**Endpoint:** POST /vehicle-readings/

**Steps:**
1. Send malformed JSON

**Expected Result:**
- 4xx error returned

**Actual Result:**
- Request accepted

**Status:** Failed


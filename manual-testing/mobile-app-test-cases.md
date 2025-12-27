# VEOS Mobile App Test Cases

## TC_MOB_001 – View vehicle telemetry

**Expected Result:**
- Real-time vehicle data displayed

**Actual Result:**
- Data accurate but delayed

---

## TC_MOB_002 – Apply speed restriction

**Expected Result:**
- Speed limit enforced on vehicle

**Actual Result:**
- Limit updates cloud & VHAL only

## TC_MOB_003 – Cloud data refresh latency

**Steps:**
1. Change vehicle speed
2. Observe mobile app update

**Expected Result:**
- Near real-time update

**Actual Result:**
- Delay of ~2 seconds

---

## TC_MOB_004 – Apply AC temperature restriction

**Steps:**
1. Set AC temperature limit from mobile app
2. Observe vehicle behavior

**Expected Result:**
- AC temperature limited

**Actual Result:**
- VHAL updated only, no real effect

**Status:** Failed


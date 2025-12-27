# VEOS Integration Test Cases

## TC_INT_001 – SOME/IP data propagation

**Steps:**
1. Send speed and gear via SOME/IP
2. Observe AAOS dashboard

**Expected Result:**
- Real-time updates without delay

**Actual Result:**
- Delay observed (~1–2 seconds)

---

## TC_INT_002 – Cloud sync flow

**Flow:**
SOME/IP → VHAL → Cloud → Mobile App

**Result:**
- Data reaches cloud successfully
- Mobile app displays correct values

## TC_INT_003 – VHAL update after SOME/IP message

**Steps:**
1. Send speed value via SOME/IP from Yocto
2. Monitor VHAL property update on AAOS

**Expected Result:**
- VHAL property updated with correct value

**Actual Result:**
- VHAL updated successfully
- Delay observed (~1 second)

---

## TC_INT_004 – Data propagation from VHAL to Cloud

**Steps:**
1. Update speed via SOME/IP
2. Verify Retrofit POST request to cloud API

**Expected Result:**
- Cloud receives latest vehicle data

---

## TC_INT_005 – Dashboard behavior after reboot

**Steps:**
1. Reboot AAOS system
2. Observe dashboard behavior

**Expected Result:**
- Dashboard auto-launches

**Actual Result:**
- Manual launch required

**Status:** Failed


# Router & Access Point Troubleshooting Guide

## Research Sources

| Site | URL |
|------|-----|
| Juniper Mist Documentation | https://www.juniper.net/documentation/us/en/software/mist/mist-wireless/topics/concept/ap-troubleshooting-overview.html |
| StayFi Access Point Support | https://hubspot.stayfi.com/knowledge/troubleshooting-disconnected-access-points |
 
---

## When to Focus on Router/Access Point Issues

**Signs the problem is router/AP, not user device:**
- Multiple devices unable to connect
- All users in area experiencing issues
- Network was working before and suddenly stopped
- Devices can't see the network at all
- All connection attempts fail

---

## Part 1: Access Point (AP) LED Status Diagnosis

### What LED Lights Mean

#### Steady Green Light
- **Status:** Access point is working normally
- **Action:** No action needed; monitor connectivity

#### Flashing Green Light
- **Status:** AP is initializing or has temporary issue
- **Action:** Wait 60 seconds for boot to complete

#### Steady Blue Light
- **Status:** AP is powered but issue detected
- **Possible Issues:** 
  - No internet connection
  - AP unplugged from router
  - Local ISP outage
- **Action:** Check power, cables, and ISP status

#### Flashing Blue Light
- **Status:** AP trying to connect to network
- **Possible Issues:**
  - Recently powered on
  - Network disconnection
  - Cable issues
- **Action:** Check cable connections; restart if necessary

#### Steady White Light
- **Status:** AP was factory reset
- **Action:** Re-adopt AP to your account (contact vendor support)

#### No Light / Off
- **Status:** No power to AP
- **Action:** Check power cable and outlet; verify Power over Ethernet (PoE) injector is active

---

## Part 2: Basic Access Point Troubleshooting Steps

### Step 1: Check Power & Physical Connections

**Power Supply:**
- Verify AP is plugged into power outlet
- Check if using PoE (Power over Ethernet) injector - verify it's plugged in
- Ensure power cord is not damaged
- Try different power outlet to rule out outlet issues

**Network Cables:**
- Verify Ethernet cable is firmly connected to router/switch
- Confirm cable is connected to correct port
- Check if using PoE injector, ensure cable goes to PoE port
- Inspect cable for damage or kinks
- Try different Ethernet cable if available

**LED Status:**
- Record what color lights are showing
- Match to the LED status guide above
- Document when lights change (initialization may take 1-2 minutes)

### Step 2: Verify AP Can See Router/Switch

The switch/router must be able to recognize AP's MAC address:
- Access router administration page
- Look for connected devices list
- Verify AP appears in the list
- If not listed, AP may not be properly connected
- Try different switch port to confirm cable/connection works

### Step 3: Test with Different Cable and Port

- Disconnect AP from current port
- Use a different Ethernet cable (borrow if needed)
- Connect to different port on switch/router
- Power cycle AP (unplug, wait 30 seconds, plug back in)
- Check if AP comes online

**Purpose:** This isolates whether problem is cable, port, or AP hardware

### Step 4: Power Cycle the Equipment

1. Unplug power from AP
2. Unplug power from router/modem
3. Wait 30 seconds minimum
4. Plug router/modem back in first
5. Wait for modem/router to fully boot (2-3 minutes - check lights)
6. Plug AP back in
7. Wait 1-2 minutes for AP to fully boot
8. Check if AP comes online and lights show normal status

### Step 5: Check ISP Status

1. Can any device connect to the internet?
2. Is other equipment showing internet connection?
3. Check ISP's status page for outages
4. Call ISP if broader outage suspected
5. Verify modem lights show normal status

---

## Part 3: Intermittent Access Point Issues

### If AP Keeps Bouncing Online/Offline

**Symptoms:**
- AP works sometimes, then drops offline
- Connection is unstable and inconsistent
- Takes time to reconnect after dropping

**Common Causes:**
- Loose cable connections
- Unstable power supply
- Overcrowded Wi-Fi channels (interference)
- Router DHCP server issues
- Damaged ethernet cable

**Troubleshooting:**
1. **Check all connections:** Ensure cables are plugged in firmly at both ends
2. **Restart equipment:** Full power cycle of router and AP
3. **Test cable:** Try different ethernet cable
4. **Check router logs:** Some routers log AP disconnections
5. **Reduce interference:** Move AP away from walls, metal objects
6. **Update firmware:** Check if router or AP firmware is outdated
7. **Monitor temperatures:** Overheating can cause intermittent issues

---

## Part 4: Multiple Device Connection Failures

### When Multiple Devices Can't Connect

**Diagnose the Scope:**
- Are ALL devices unable to connect?
- Or just specific device types (only laptops, or only mobile phones)?
- Are some users successful while others fail?

**If ALL devices failing:**
- Issue is definitely router/AP side
- Follow basic troubleshooting above
- Escalate to network administrator

**If SOME devices failing:**
- May be device-specific (driver, settings, compatibility)
- May be account/credential issue
- Escalate affected devices to help desk for individual support

---

## Part 5: When to Escalate

### Escalate to Level 2/Network Team If:

- LED troubleshooting indicates hardware failure (no light, won't respond)
- Multiple resets and power cycles don't resolve issue
- AP doesn't appear in router's connected device list
- Different cables and ports don't fix the problem
- PoE injector power light is off or abnormal
- Firewall rules may be blocking AP communication

### Information to Provide When Escalating:

1. AP model number and firmware version
2. LED status and color sequence
3. MAC address of AP (usually on label)
4. Router/switch model it's connected to
5. When problem started (during outage, after change, etc.)
6. Whether issue is intermittent or constant
7. Devices that can and cannot connect
8. Any recent network changes

---

## Part 6: Access Point Configuration Check

### Common Configuration Issues

**Verify These Settings (if you can access router):**

- SSID is enabled and broadcasting
- Wireless channel is set appropriately (not overlapping with neighbors)
- Security type matches what devices are configured for
- 2.4 GHz and 5 GHz bands are both enabled (if dual-band)
- DHCP is enabled so router assigns IP addresses
- Channel width is compatible with devices

**How to Check:**
- Log into router's admin page (usually 192.168.1.1)
- Look for Wireless Settings or Wi-Fi Settings section
- Verify broadcast is enabled
- Check channel selection (1, 6, or 11 for 2.4 GHz; automatic for 5 GHz)
- Ensure compatibility with device specifications

---

## Quick Reference: Troubleshooting Flowchart

AP Not Working?
↓
Are there lights on the AP?
├─ NO → Check power cable and outlet → Restart if powered
└─ YES → Check LED color
├─ Green → Check if devices can connect
├─ Blue → Check cables → Restart modem/router → Check ISP
├─ White → Factory reset occurred → Re-adopt to system
└─ Flashing → Wait 60 seconds for boot completion

Can devices see/connect to the network?
├─ NO → Verify SSID is broadcasting → Check AP appears in router device list
└─ YES → Can devices access internet?
├─ NO → Verify router has internet → Check firewall/security
└─ YES → Issue resolved; monitor for stability

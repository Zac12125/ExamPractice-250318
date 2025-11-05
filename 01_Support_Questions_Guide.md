# Wi-Fi Connectivity Troubleshooting - Support Questions Guide

## Source
- Blog: Route This - 7 Questions Top ISP Support Teams Ask
- URL: https://blog.routethis.com/questions-isp-support-agents-ask-on-home-network-calls/

## Problem Statement
**Device:** Laptop (Windows 10)
**Issue:** Cannot connect to Office_Network Wi-Fi
**Error Message:** "Unable to connect to the network"
**Context:** Other devices (phone, tablet) can connect successfully
 
---

## Essential Support Questions to Ask the End User

### 1. **Device-Specific Diagnosis**
- How many times have you attempted to connect?
- When did this issue first start occurring?
- Has your laptop connected to Office_Network before, or is this the first attempt?
- Are you seeing the network name (SSID) in your available networks list?
- If yes, what happens when you click to connect? (Do you enter a password? What error appears?)

### 2. **Confirm It's Not a Device Problem**
- Since your phone and tablet CAN connect to Office_Network, this suggests the network is functioning
- Have you successfully connected other Windows 10 laptops to this same network?
- Can you test this same laptop on a different Wi-Fi network (like home or personal hotspot)?
- **Purpose:** Determine if issue is network-wide, device-specific, or account-specific

### 3. **Physical Connection & Hardware**
- Is the Wi-Fi adapter turned ON? Check for a physical switch on the laptop or in settings
- Is your laptop in Airplane Mode? 
- Can you see the Wi-Fi icon in your system tray/taskbar?
- How far are you from the router/access point?
- Are there any obstructions between your laptop and the router?

### 4. **Network Credentials & Authentication**
- Do you have the correct Office_Network password?
- Has the password been changed recently?
- Are you using the correct network name (could there be multiple Office_Network options)?
- Are you being prompted for a username and domain (corporate domain)?
- Are your corporate credentials correct if applicable?

### 5. **Router & Access Point Status**
- Are the lights on the router/access point showing normal status?
- Is the router powered on and functioning?
- Have you noticed if other people are having issues connecting at the same time?
- Is there a specific location where the connection fails (or is it everywhere)?

### 6. **Timing & Recent Changes**
- Has anything changed recently? (Windows updates, driver updates, router configuration changes?)
- Did you have an internet outage earlier?
- Did you restart your laptop after connecting to the network?
- Are you connected to a VPN that might be interfering?

### 7. **Security & Firewall**
- Is your Windows Firewall turned on?
- Do you have antivirus software that might be blocking the connection?
- Is there a corporate proxy or security software preventing connections?

---

## Initial Troubleshooting Steps to Provide the User

1. **Restart the device** - Turn off the laptop completely, wait 30 seconds, and turn it back on
2. **Forget and reconnect** - Go to Settings > Network & Internet > Wi-Fi > Manage known networks > Select Office_Network > Forget, then reconnect
3. **Restart the router** - Have them unplug the router for 30 seconds, then power it back on
4. **Move closer to the router** - Eliminate distance/obstruction variables
5. **Check Windows Update** - Ensure network drivers are up to date
6. **Run Network Troubleshooter** - Windows 10: Settings > Network & Internet > Status > Network troubleshooter

---

## When to Escalate

If after these questions and steps the issue persists, escalate to:
- **Level 2 IT Support** - For network infrastructure issues
- **Network Administrator** - To verify router/AP settings and network permissions
- **Vendor Support** - If hardware failure is suspected

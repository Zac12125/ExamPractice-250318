# Basic Network Wi-Fi Connection Troubleshooting

## Research Sources

| Site | URL |
|------|-----|
| Microsoft Support | https://support.microsoft.com/en-us/windows/fix-wi-fi-connection-issues-in-windows-9424a1f7-6a3b-65a6-4d78-7f07eee84d2c |
| AmorServ | https://amorserv.com/insights/how-to-troubleshoot-wireless-network-connectivity-issues-in-10-steps |
| Speedtest Knowledge | https://www.speedtest.net/about/knowledge/simple-wifi-audit |

---

## Quick Fix Summary

### Top 5 Immediate Steps

1. **Restart Router & Modem**
   - Unplug router for 30 seconds
   - Unplug modem for 30 seconds (if separate)
   - Wait 2-3 minutes for full boot
   - Reconnect to network

2. **Check Wi-Fi is Enabled**
   - Click network icon in taskbar
   - Verify Wi-Fi is turned ON
   - Check if Airplane Mode is OFF
   - Look for physical Wi-Fi switch on laptop

3. **Forget and Reconnect**
   - Settings > Network & Internet > Wi-Fi > Manage known networks
   - Select your network > Forget
   - Find and reconnect to the network
   - Enter password if prompted

4. **Check Physical Connections**
   - Ensure all router/modem cables are plugged in
   - Look for loose connections
   - Check if router lights are normal (green = good, red = problem)
   - Move closer to router to eliminate distance issues

5. **Update Network Drivers**
   - Device Manager > Network adapters
   - Right-click adapter > Update driver
   - Or check manufacturer website for latest drivers

---

## Step-by-Step Troubleshooting Process

### Step 1: Identify the Issue Scope
- **Single device or multiple?** If only your device, problem is likely device-specific
- **All times or intermittent?** Intermittent suggests interference or distance issues
- **Works on other networks?** If yes, issue may be specific network settings

**Questions to Ask:**
- Can any other device connect to this network right now?
- Have you successfully connected before, or is this first time?
- Are you the only one experiencing this, or are others too?

### Step 2: Check Basic Hardware
- Is the laptop powered on?
- Is Wi-Fi physically enabled (hardware switch or software toggle)?
- Can you see the network SSID in available networks list?
- Are you in range of the router (typically 150-300 feet)?
- Are there major obstructions between you and router? (walls, metal objects)

### Step 3: Verify Network Settings
- **Network Name (SSID):** Are you selecting the correct network?
- **Password:** Verify you're entering correct password (case-sensitive)
- **DHCP:** Is the router set to automatically assign IP addresses?
- **Frequency Band:** Is your adapter compatible? (Some only support 2.4 GHz)

### Step 4: Perform Power Cycle
1. Turn off Wi-Fi on your device
2. Wait 10 seconds
3. Turn Wi-Fi back ON
4. Select your network and reconnect

If that doesn't work:
1. Restart your computer completely
2. Wait for full startup
3. Attempt connection again

### Step 5: Check for Interference
- Move away from: microwaves, cordless phones, Bluetooth speakers, baby monitors
- These devices use 2.4 GHz frequency and can cause interference
- Use Wi-Fi analyzer apps to check for congested channels
- Consider switching to 5 GHz network if available

### Step 6: Verify Router Functionality
- Are other devices able to connect successfully?
- Can you use an Ethernet cable directly to router to verify internet?
- If Ethernet works but Wi-Fi doesn't, problem is Wi-Fi functionality
- If both fail, problem is internet provider or router hardware

### Step 7: Advanced Network Commands (Windows)

If still not working, open Command Prompt as Administrator and run:


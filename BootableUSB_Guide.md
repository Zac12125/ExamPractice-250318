# How to Create a Bootable Windows 10 USB

## Overview

A bootable USB drive allows you to perform a clean Windows 10 installation, repair your current Windows installation, or upgrade your system conveniently without an optical drive. It's also a portable solution for troubleshooting and system recovery.

## Requirements

- Windows computer
- USB drive with at least 8GB of free space
- Internet connection
- Windows 10 Media Creation Tool (free from Microsoft)

## Step-by-Step Guide

### Step 1: Download the Media Creation Tool

1. Visit the [official Microsoft Windows 10 download website](https://support.microsoft.com/en-us/windows/create-installation-media-for-windows-99a58364-8c02-206f-aa6f-40c3b507420d)
2. Under the "Create Windows 10 installation media" section, click **Download Now**
3. Wait for the `MediaCreationToolxxxx.exe` file to download

### Step 2: Launch the Media Creation Tool

1. Navigate to your Downloads folder
2. Double-click the `MediaCreationToolxxxx.exe` file
3. If prompted by Windows, click **Yes** to allow the application to make changes
4. Wait for the tool to load

### Step 3: Accept License Terms

1. A window will appear saying "Getting a few things ready"
2. Wait for the license terms screen to appear
3. Click the **Accept** button to agree to Microsoft's terms

### Step 4: Select Installation Media Creation

1. You'll see two options:
   - Upgrade this PC now
   - Create installation media for another PC
2. Select **"Create installation media (USB flash drive, DVD, or ISO file) for another PC"**
3. Click **Next**

### Step 5: Choose Your Preferences

1. Select your preferred **Language** (e.g., English)
2. Select the Windows 10 **Edition** (Home, Pro, etc.)
3. Select the **Architecture**:
   - 32-bit (for older systems)
   - 64-bit (recommended for modern systems)
   - Both (if you want compatibility with both)
4. If you're unsure, check the box for **"Use the recommended options for this PC"**
5. Click **Next**

### Step 6: Select USB Flash Drive

1. Choose **"USB flash drive"** as your media option
2. Click **Next**
3. Select your USB drive from the list
   - **Warning:** All content on the selected USB drive will be deleted
   - If you don't see your drive, click **"Refresh drive list"**
4. Click **Next**

### Step 7: Download and Create Bootable Media

1. The Media Creation Tool will now download Windows 10
2. A progress indicator shows the download status
3. Once complete, the tool will copy the files to your USB drive
4. When finished, click **Finish**

## How to Boot from Your USB Drive

1. Insert the bootable USB drive into your target computer
2. Restart/power on the computer
3. Immediately press the boot menu key (varies by manufacturer):
   - **F11** or **F12** (most common)
   - **Esc** or **Delete**
   - **Spacebar** (for some systems)
4. Select your USB drive from the boot menu
5. The Windows 10 setup wizard will start

## Alternative Method: Using Rufus

If the Media Creation Tool doesn't work for you, you can use **Rufus**, a free third-party tool:

1. Download Rufus from [https://rufus.ie/](https://rufus.ie/)
2. Run the application
3. Select your USB drive under **Device**
4. Click **Select** and choose your Windows 10 ISO file
5. Configure settings:
   - Image option: Standard Windows installation
   - Partition scheme: GPT
   - Target system: UEFI (non-CSM)
6. Click **Start** and confirm the format warning

## Troubleshooting

- **USB drive not detected:** Try a different USB port or USB drive
- **Boot menu won't appear:** Restart and press the boot key immediately after powering on
- **Installation stuck:** Ensure your USB drive is at least 8GB and has a stable connection

## Sources

- Microsoft Support: Create installation media for Windows
- TechRadar: How to make a bootable Windows 10 USB
- Windows Central: How to install Windows 10 from USB with UEFI support

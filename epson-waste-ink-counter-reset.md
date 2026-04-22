---
title: "How to Reset the Waste Ink Counter on Epson L-Series Printers"
excerpt: "Replaced your ink pad but still getting the 'Service Required' error? Learn how to use the Adjustment Program (AdjProg) to reset the internal EEPROM counter on your Epson EcoTank."
date: "2026-04-23"
author: "JoeTinnySpace"
tags: ["Guides & Rescues", "Hardware & Networks"]
coverImage: "https://raw.githubusercontent.com/JoeTinnySpace/BrandezBlog/main/assets/epson_waste_reset.png"
---

# Fixing the "End of Service Life" Software Lock

If your Epson L-Series printer (L3110, L3150, L3210, etc.) has suddenly stopped working, flashing alternate red lights and displaying the "A printer's ink pad is at the end of its service life" error on your monitor, you have hit a hard-coded software lock.

As detailed in our **[Physical Ink Pad Replacement Guide](./epson-l-series-ink-pad-replacement.md)**, you should always replace or clean the physical sponges first. However, doing so will not magically fix the error. The printer relies on an internal digital counter (stored on the EEPROM chip) that counts every page printed and every cleaning cycle run. Once that counter hits 100%, it locks the hardware to prevent a physical overflow.

Here is how to reset that digital counter back to 0%.

## Prerequisites

To perform this software reset, you will need:
1. **A Windows PC** (The reset utilities generally do not run on macOS without a virtual machine).
2. **A direct USB connection.** Do not attempt to reset the counter over Wi-Fi. Plug the printer directly into your computer via a USB cable.
3. **The Epson Adjustment Program (AdjProg).** You will need to find and download the specific version of `AdjProg.exe` built for your exact printer model. 

> **Important Security Note:** Because AdjProg is proprietary factory software often leaked online, Windows Defender and other antivirus programs will almost always flag it as a virus, malware, or a trojan. You will likely need to temporarily disable your antivirus to extract and run the utility. Proceed with caution and ensure you are downloading from a trusted repair forum.

## Step-by-Step Reset Guide

### Step 1: Initialize the Utility
1. Ensure your printer is turned **ON** and connected via USB.
2. Extract the downloaded Adjustment Program ZIP file and run `AdjProg.exe` (Run as Administrator).
3. Click the **"Select"** button.
4. Choose your exact printer **Model Name** from the dropdown list.
5. Set the **Port** to "Auto selection" (or manually select the USB port your printer is assigned to). Click **OK**.

### Step 2: Access the Maintenance Menu
1. On the main screen, click the **"Particular adjustment mode"** button.
2. A large menu will appear containing various factory calibration tools. Scroll down to the **Maintenance** section.
3. Select **"Waste ink pad counter"** and click **OK**.

### Step 3: Check and Reset the Counter
1. You will see checkboxes for the **Main pad counter** and (depending on your model) the **Platen pad counter**. 
2. Check both boxes and click the **"Check"** button. The software will communicate with the printer and display the current point values and percentages. If you are locked out, at least one of these will read `100%`.
3. Check the boxes again.
4. This time, click the **"Initialize"** button. 
5. A prompt will appear asking for confirmation to reset the EEPROM. Click **OK**.

### Step 4: Reboot the Printer
The utility will process the request for a few seconds and then display a pop-up message telling you to **"Please turn off the printer."**

1. Press the physical power button on your printer to shut it down.
2. Once the printer is completely off, click **OK** on the computer prompt.
3. Close the Adjustment Program.
4. Turn your printer back on.

If done correctly, the blinking red error lights will disappear, the printhead will cycle normally, and your Epson L-Series printer will be ready to print again!

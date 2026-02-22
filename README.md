LG ULTRAGEAR FULL Cal.icm --> Monitor Color Profile to be used when the Output Control Format (color space) in the Nvidia Control Panel or AMD Radeon Software is RGB FULL.

LG ULTRAGEAR LIMITED Cal.icm --> Monitor Color Profile to be used when the Output Control Format (color space) in the Nvidia Control Panel or AMD Radeon Software is RGB LIMITED or YCbCr444 LIMITED.


The suggested color profile is "LG ULTRAGEAR LIMITED Cal.icm" with Output Control Format (color space) set to RGB LIMITED or YCbCr444 LIMITED.



LG ULTRAGEAR Autodimming fix Tools to generate the color profile

*DisplayCAL
- ZIP archive Download
https://displaycal.net/download/standalone/DisplayCAL-win32.zip
- Installer
https://displaycal.net/download/standalone/DisplayCAL-Setup.exe

*AgyII Color Management Microsoft Windows executables (to embed the new Calibration curves in the baseline color profile .icm file)
https://www.argyllcms.com/Argyll_V3.3.0_win64_exe.zip


*Add vcgt calibration into a ICC profile:
https://argyllcms.com/doc/iccvcgt.html
profile/iccvcgt
Summary
Extract or insert 'vcgt' calibration tag from/into ICC profile.
Usage Summary
usage: -x profile.icm curves.cal

usage: -i inprofile.icm curves.cal outprofile.icm

 -v              Verbose mode
 -x              Extract 'vcgt'
 -i              Insert 'vcgt'
Usage Details and Discussion
The -v flag may give extra information.



Calibration Files
calcurve.cal "Original Calibration File"
calcurve_2.cal "Calibration file to fix autodimming with Output  Color Format YCbCr444"
calcurve_4.cal "Calibration file to fix autodimming with Output  Color Format RGB"



## 🛠️ The Story Behind the Fix

This solution was not a quick discovery—it is the result of over **five months of dedicated testing, data logging, and trial-and-error** by the original creator, **Stuff_Around**.

### The Research Process:
*   **The Problem:** Identifying that the LG 27GS60QC-B suffers from aggressive "Smart Energy Saving" and firmware-level dimming even when the settings are toggled off.
*   **The Discovery:** Finding that specific Gamma curves and luminance data within a custom ICC\ICM profile could "trick" the monitor's internal processing into maintaining consistent brightness.
*   **The Solution:** Designing and refining the **Gamma 2.2** and **Gamma 2.4** profiles provided in this repository to provide a stable, flicker-free experience without sacrificing color accuracy.

### Original Creator
*   **Username:** [Stuff_Around](https://www.reddit.com)
*   **Community:** First shared and vetted within the r/LGUltraGearOfficial and r/buildapcmonitors communities.
*   **Video Documentation:** For a deep dive into how this works, check out the creator's [YouTube Channel](https://www.youtube.com).

> **Note to the Community:**  
> If you find this fix helpful, please support the original creator by providing credit. This project was created for the community to fix a hardware frustration that the manufacturer has yet to address.


## ⚠️ License & Usage Terms

This project is the result of 5 months of research and development by **Stuff_Around**. To prevent further uncredited distribution or unauthorized commercial use, the following terms apply:

### 1. Personal Use Only
You are free to download and use these ICC profiles for your personal monitor setup.

### 2. Software Integration Prohibited
**Strictly Prohibited:** You may **not** bundle, integrate, or embed these profiles into any software, scripts, calibration tools, or firmware without express written permission.

### 3. Attribution Required
If you share or mention this fix on forums, YouTube, or social media, you **must** credit **Stuff_Around** and link back to this repository.

### 4. Commercial Use
Commercial use of these files is strictly forbidden.

---

**Need Permission?**  
If you are a developer looking to integrate this fix into a software utility, please contact the creator directly via [Reddit (Stuff_Around)](https://www.reddit.com) or youtube to obtain a formal agreement.

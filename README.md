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

If you want to use my ICC/ICM profiles you must credit me on your work otherwise the ICC/ICM is not allowed to be used. 

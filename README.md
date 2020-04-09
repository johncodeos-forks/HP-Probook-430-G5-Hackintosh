# HP-Probook-430-G5-Hackintosh
EFI folder for installing macOS on the Probook 430 G5

Use your own SMBIOS - My SMBIOS here is removed for privacy reasons.

Make sure to use a MacBookPro15,2 SMBIOS or your HDMI won't work.

OpenCore version: 0.5.7

Kexts in the "LE" folder go to /Library/Extensions

After copying them, run this in terminal:
`sudo touch /Library/Extensions && sudo kextcache -u /`

aDummyHDA.kext is required for the headphone jack to work! The executable in this kext is a symlink to `/System/Library/Extensions/AppleHDA.kext/Contents/MacOS/AppleHDA`

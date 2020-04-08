# HP-Probook-430-G5-Hackintosh
EFI folder for installing macOS on the Probook 430 G5

Use your own SMBIOS - My SMBIOS here is removed for privacy reasons.

OpenCore version: 0.5.7

Make sure to use a MacBookPro15,2 SMBIOS or your HDMI won't work.

Kexts in the "Library-Extensions" folder go to /Library/Extensions

After putting them, run this in terminal:
`sudo touch /Library/Extensions && sudo kextcache -u /`

aDummyHDA.kext is required for the headphone jack to work!

# HP-Probook-430-G5-Hackintosh
EFI folder for installing macOS on the Probook 430 G5

Big Sur is supported!

Use your own SMBIOS - My SMBIOS here is removed for privacy reasons.

Make sure to use a MacBookPro15,2 SMBIOS or your HDMI won't work.

OpenCore version: 0.6.0

Kexts in the "LE" folder go to /Library/Extensions

After copying them, run this in terminal:
`sudo touch /Library/Extensions && sudo kextcache -i /`

aDummyHDA.kext is required for the headphone jack to work! The executable in this kext is a symlink to `/System/Library/Extensions/AppleHDA.kext/Contents/MacOS/AppleHDA`


IMPORTANT: If you want to use Catalina, remove the AppleAHCIPort.kext from the `EFI/OC/Kexts`, and also don't forget to remove it from the config.plist too.


Credits
------------

Apple for macOS and for streaming WWDC19 to my headphones while I was working on this

RehabMan for the SSDT and for the initial Clover setup - this wouldn't have been possible to complete in such a short time without him!

Acidanthera for the kexts and OpenCore

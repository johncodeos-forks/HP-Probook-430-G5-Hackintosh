# HP-Probook-430-G5-Hackintosh
EFI folder for installing macOS on the Probook 430 G5

Big Sur is supported!

Use your own SMBIOS - My SMBIOS here is removed for privacy reasons.

Make sure to use a MacBookPro15,2 SMBIOS or your HDMI won't work.

OpenCore version: 0.6.0

Kexts in the "LE" folder go to /Library/Extensions

After copying them, run this in terminal if you're still using Catalina:
`sudo touch /Library/Extensions && sudo kextcache -i /`

IMPORTANT: If you want to use Catalina, remove AppleAHCIPort.kext from the `EFI/OC/Kexts`, and also don't forget to remove it from the config.plist too.


Credits
------------

Apple for macOS and for streaming WWDC19 to my headphones while I was working on this

@kreizlie for the ACPI configuration

Acidanthera for the kexts and OpenCore

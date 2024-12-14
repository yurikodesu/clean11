# hyprt-autounattend
My custom autounattend file with tweaks for Windows 11 for a more pleasant experience overall.

# What tweaks?
## OOBE and Windows installer tweaks:
- Bypass Windows 11 requirements (TPM, Secure Boot, etc.)
- Allow Windows 11 to be installed without a network connection (runs OOBE\BYPASSNRO automatically)
- Uses a generic product key, and skips EULA and goes straight to partition setup in the installer.
- Defaults to local account creation during OOBE.
- Prevents automatic device encryption on a fresh install.
- Disables all express settings by default in OOBE.
- Removes all Windows 11 tiles by default after a fresh install.

## Windows 11 tweaks:
- Removes preset icons from the taskbar. (MS Edge, MS Store, Explorer, etc.)
- Icon only search in taskbar by default. (Can be changed of course, it just looks cleaner to me that way.)
- Always show file extensions in Explorer.
- Disables widgets entirely.
- Uses classic context menu.
- Left-aligned taskbar.
- Sets startup page of Windows 11 to "This PC" from "Home".
- Disables Bing in search.
- Disables fast startup.
- Allows execution of PowerShell scripts by default.
- Disables last access time stamp updates in NTFS.
- Prevents Windows Update from doing automatic reboots.
- Disables app suggestions/Content delivery manager.
- Disables Edge's first run experience. (Might show "This browser is managed by your organization" but it's pretty harmless and should be ignored.)
- Disables "Enhance Pointer Precision" mouse setting.

# Windows Defender:
- Use autounattend-no-defender.xml if you also want Defender gone after a fresh Windows install.
- Otherwise stick to the regular autounattend if you want to continue using Windows Defender.

# What is autounattend-hyprt.xml?
- It's same as the regular autounattend with the only difference being that it sets the computer name to "devs11" after a fresh install. It is really only for my personal use.

# Who is this intended for?
- It's intended for intermediate-advanced users and it enables quite for risky stuff like automatically enabling PowerShell scripts, etc.
- It's intended for people who know what they are doing and are aware of the modifications this autounattend script can do.
- It's intended for people who are willing to go out of their comfort zone to make an overall more pleasant Windows experience for them.<br>

**IT IS NOT A HEAVY MODIFICATION TO WINDOWS! It's exactly identical to a fresh Windows 11 install. Comparing it to AtlasOS, ReviOS, Ghost Spectre or memstechtips' UnattendedWinstall doesn't do it justice. It's a bunch of small modifications and registry tweaks to Windows. Each and every thing can be restored to default after the installation and it does not break anything at all.** <br><br>

**Use as your own risk. I am not responsible for any damage caused.** <br>
**I will look out for updates and changes to Windows and try to update it, if it causes anything to break, please make an issue about it.** <br><br>

**I was able to achieve this using [schneegans.de's autounttend.xml generator](https://schneegans.de/windows/unattend-generator/). I just saved some of your time by making a template or a generic config for you to use by compiling settings and configs that most would have done anyway. However if you want to change anything, feel free to import it on the website and make your modifications.**

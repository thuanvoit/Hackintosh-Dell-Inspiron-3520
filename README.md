# How to Install Mac OS High Sierra 10.13.6 on Laptop Dell Inspiron 3520

# Preview:
<p align="center"><img src ="/images/img1.png"  /></p>
<p align="center"><img src ="/images/img2.png"  /></p>

#

### Download: [RELEASES](https://github.com/thuanvoit/Hackintosh-Dell-Inspiron-3520/releases)


# System information
- Processor : Intel(R) Core(TM) i5-3230M CPU @ 2.60GHz (Ivy Bridge)
- Graphics Processor(GPU) : Intel HD4000 1536 MB Graphics
- Hard disk : HDD 500GB
- RAM : 8GB DDR3 / bus 1600
- Wifi + Buetooth: BCM943225HM
- Audio : Cirrus Logic CS4213
- Touchpad : ALPS Touchpad
- Webcam 

### Working
- Graphics HD 4000
- Brightness
- Fn Brightness keys (Use lastest VoodooPS2Controller and set keyboard shortcuts)
- Sleep and wake
- Audio (VoodooHDA 2.8.9 only)
- WIFI + BLUETOOTH
- LAN
- USB
- Touchpad (2 fingers scrolling)
- Webcam
- iMessages, Facetime and iCloud
### Not working
- Microphone
- HDMI (no test)

# INSTALLATION

### Requirement
- Turn off Secure Boot in BIOS
- VMWare to run MACOS or Real Macbook
- USB 8GB or up
- Mac OS High Sierra Installer

### Create High Sierra Installer
Erase and rename your USB to ' install_osx '
Then copy and paste the code below

Code:
```sh
sudo /Applications/Install\ macOS\ High\ Sierra.app/Contents/Resources/createinstallmedia --volume /Volumes/install_osx --applicationpath /Applications/Install\ macOS\ High\ Sierra.app --nointeraction
```

### Keyboard (VoodooPS2Controller and Karabiner Elements)
- F1: Brightness decrease
- F2: Brightness increase
- F3: Mission Control
- F4: Launchpad
- F5: Illumination decrease
- F6: Illumination increase
- F7: Rewind
- F8: Play/Pause
- F9: Fast Forward
- F10: Mute
- F11: Volume decrease
- F12: Volume increase

# Fixing Guide
### ALPS Trackpad
All files in ' ALPS.VoodooPS2.Rev12 ' folder
1. /System/Library/HIDPlugins/IOHIDKeyboardFilter.plugin (Synaptics)
2. /System/Library/PreferencePanes/Trackpad.prefPane
3. /EFI/CLOVER/kexts/10.12/PS2Controller.kext
4. /usr/bin/VoodooPS2Daemons & /Library/LaunchDaemons/org.rehabman.voodoo.driver.Daemon.plist (Synaptics)
5. Jalankan script “Touchpad Settings” (ALPS, ELAN, ...)
6. Fix permission by Kext Utility & Disk Utility

### Keyboard
[Following Rehabman Guide using VooDooPS2Controller](https://github.com/RehabMan/OS-X-Voodoo-PS2-Controller/wiki/How-to-Install)

### Fix function keys
* Download ' Karabiner-Elements-12.1.0.dmg ' in [Tools](/Tools/)
* [Karabiner Elements](https://l.facebook.com/l.php?u=https%3A%2F%2Fgithub.com%2Ftekezo%2FKarabiner-Elements&h=AT2DVoTW5UeSOoi4BrHvv-GmIBFkGGlhkF1BE5dQWnsch4Um7YBcoA9PibJ9d62TyUDVqmhKkh3pKUVHX3s2QdbF76VmeK4t-BGFB_dtrSpY0COjQadRXYOrBHqXilUmcc8bqxd3ojGGo_eNr9ZCgRomPT4)

### Credits:
* [Niemtin007](http://niemtin007.blogspot.com/)
* [Hackintosh - The OS X on PC World](https://www.facebook.com/groups/hackintoshPC/)
* [Hieu - Admin Hackintosh Facebook Page](https://www.facebook.com/cobaohieu)
* [Thang Duong](https://www.facebook.com/thangduong.dev)
* [Rehabman](https://github.com/RehabMan)
* [BADRUZEUS SHAVA - Hackintosh Indonesia](https://www.facebook.com/badruzeus)

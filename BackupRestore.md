# How to Backup & Restore CM7 Pre-Beta #

## Introduction ##

Welcome to the Atrix Dev Team's CM7 Project.

This is a quick guide of how to safely backup and restore your Atrix when moving between CM7 and your Motorola ROM of choice.

**Please read the instructions very carefully**
**If at any point you are not 100% comfortable with the instructions, read through them again and then ask for help**

### Pre-Work ###

Before powering off the phone download the CM7 package and copy to internal SD Card


### Flashing CWM Recovery via Fastboot ###
  1. **Download the latest CWM recovery from Downloads section (**<a href='http://download.clockworkmod.com/recoveries/recovery-clockwork-5.0.2.0-olympus.img'>recovery-clockwork-5.0.2.0-olympus.img</a>)**1. Power off phone
  1. Put phone into fastboot (Power + Vol Down Button)
  1. Press Volume Up button to select Fastboot
  1. Connect phone via USB cable
  1. Open Command Prompt from your fastboot directory
  1. Type "fastboot flash recovery recovery.img" (no quotation marks)
  1. Type "fastboot reboot"
  1. Your phone will reboot normally**

### Flashing CWM via ROM Manager ###
  1. Download ROM Manager from the Market
  1. Open ROM Manager and make sure to allow Root Access
  1. Press Flash ClockworkMod Recovery and select Atrix
  1. Done

### Backup ###
  1. Reboot phone into CWM recovery (Power Button + Vol Down), press Vol Down until you see "Android Recovery" then press Vol Up to enter.
  1. Go to Backup & Restore and create a backup (this may take some time)

### Installing CM7 ###
  1. While in Recovery install CM7 from internal storage
  1. After installation select Data Wipe/Factory Reset
  1. Then Wipe Cache Partition
  1. Reboot system now
  1. Watch awesome boot animation
### Optional Google Apps ###
  1. Download <a href='http://cmw.22aaf3.com/gapps/gapps-gb-20110828-signed.zip'>Google Apps Package</a>
  1. Copy to Internal SD Card
  1. Reboot into Recovery
  1. Install Zip
  1. Reboot when done

### Updating CM7 from older version of CM7 ###
  1. Make sure you're on the latest recovery (refer above)
  1. Copy file to Internal SDCard
  1. Reboot phone into recovery
  1. Flash zip file
  1. Wait for it to complete, then reboot

### Restore ###
  1. Reboot phone into recovery (Power + Vol Up button)
  1. Once in recovery go to Backup & Restore
  1. Select Restore, then restore the most recent one (should be dated)
  1. Allow time for restore, once complete reboot phone

### Restore Workaround ###
If after recovering your phone bootloops, please use this workaround.

  1. Open up the Zip file of your current Blur ROM (Ninja, CherryBlur, Alien, etc.)
  1. extract the boot.img file and copy to the directory where your fastboot is.
  1. Pull phone battery & reinsert
  1. Power on phone and go straight to Fastboot mode (Power + Vol Down)
  1. Type "fastboot flash boot boot.img" (exclude quotation marks)
  1. Once flashed, reboot phone using "fastboot reboot"
  1. **Phone should boot normally**
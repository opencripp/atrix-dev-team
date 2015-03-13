# FAQ #
Here you will find some of the Frequently Asked Questions to get the most out of your Atrix CM7 experience.

Please let me know if you'd like any other instructions in this FAQ.

## <font color='#FF0000'><b>This is not a bug thread, all annoying comments will be deleted by me. You have no forum rules to protect you here.</b></font> ##


---

## GPS ##
There are 2 possible fixes for GPS
### Fix 1: ###
  1. Go to the Android Market
  1. Download GPS Status & Toolbox (https://market.android.com/details?id=com.eclipsim.gpsstatus2)
  1. Open GPS Status & Toolbox and press the menu button
    * ![https://lh6.googleusercontent.com/-BBisD5JoKP8/TnKDOhqVQHI/AAAAAAAABYE/8PT5iCScgQI/s512/screenshot-1316127355457.png](https://lh6.googleusercontent.com/-BBisD5JoKP8/TnKDOhqVQHI/AAAAAAAABYE/8PT5iCScgQI/s512/screenshot-1316127355457.png)
  1. Select Compass Calibration and follow the instructions
    * ![https://lh4.googleusercontent.com/-ZBbipG4Ob54/TnKDQPpB7AI/AAAAAAAABYI/FHRWr5DlpuE/s512/screenshot-1316127375182.png](https://lh4.googleusercontent.com/-ZBbipG4Ob54/TnKDQPpB7AI/AAAAAAAABYI/FHRWr5DlpuE/s512/screenshot-1316127375182.png)
  1. Once that's completed go to Calibrate pitch and roll
    * ![https://lh5.googleusercontent.com/-V9jbzxkM768/TnKDSF6eY4I/AAAAAAAABYM/WS1kuPqx-nw/s512/screenshot-1316127405506.png](https://lh5.googleusercontent.com/-V9jbzxkM768/TnKDSF6eY4I/AAAAAAAABYM/WS1kuPqx-nw/s512/screenshot-1316127405506.png)
  1. Your GPS should work better now.

Try this fix a few times to make sure it's properly calibrated.

**If Fix 1 doesn't do the trick then...**

### Fix 2: ###
I personally experience the GPS problem during Alpha testing and nothing seemed to fix it. So I tried re-flashing the radio and finally have perfect GPS tracking.

  1. Go to Settings
  1. Go to About Phone
  1. Find the Baseband version
    * ![https://lh5.googleusercontent.com/-MrTpnXDQ3I4/TnKJfAGuprI/AAAAAAAABYc/y-erW--Zdkc/s512/screenshot-1316128938181.png](https://lh5.googleusercontent.com/-MrTpnXDQ3I4/TnKJfAGuprI/AAAAAAAABYc/y-erW--Zdkc/s512/screenshot-1316128938181.png)
  1. Download the radio for your phone (Links located below)
  1. Flash with either RSDLite or Recovery (refer to thread instructions)
  1. Reboot phone and


### Radio Links: ###
Chinese Retail - BP\_N\_01.35.00R
  * http://forum.xda-developers.com/showthread.php?t=1235665

AT&T United States - N\_01.77.30P
  * http://forum.xda-developers.com/showthread.php?t=1159505

International - 1.97.00R
  * http://forum.xda-developers.com/showthread.php?t=1222757

South East Asia - N\_01.95.00R & Orange France - N\_01.100.00R
  * http://forum.xda-developers.com/showthread.php?t=1175750

Bell Canada - N\_01.77.33P
  * http://forum.xda-developers.com/showthread.php?t=1260963



---

## SD Card ##
This sections will tell you how to change the default settings in CM7 so the Internal SD Card remains /mnt/sdcard and the External SD Card becomes /mnt/emmc.

  1. Once you have installed CM7
  1. Go through setup wizard (if you've installed GApps)
  1. Once on phone desktop go to Settings
  1. Go to CyanogeMod Settings
    * ![https://lh3.googleusercontent.com/-s64YhKOy9sc/TnKWlY0XCWI/AAAAAAAABY0/opKzbHvmjZA/s512/screenshot-1316130925382.png](https://lh3.googleusercontent.com/-s64YhKOy9sc/TnKWlY0XCWI/AAAAAAAABY0/opKzbHvmjZA/s512/screenshot-1316130925382.png)
  1. Go to Application
    * ![https://lh3.googleusercontent.com/-42fsP6o-rOA/TnKWlm7OzVI/AAAAAAAABY4/lHRMfLkb0EQ/s512/screenshot-1316130933069.png](https://lh3.googleusercontent.com/-42fsP6o-rOA/TnKWlm7OzVI/AAAAAAAABY4/lHRMfLkb0EQ/s512/screenshot-1316130933069.png)
  1. In this menu select Use internal storage
    * ![https://lh6.googleusercontent.com/-SGuOXBWO6So/TnKWluwpzuI/AAAAAAAABY8/BJO2HJDWIJY/s512/screenshot-1316130944494.png](https://lh6.googleusercontent.com/-SGuOXBWO6So/TnKWluwpzuI/AAAAAAAABY8/BJO2HJDWIJY/s512/screenshot-1316130944494.png)
  1. Reboot phone

Your phone should now use the internal SD Card instead of the external as primary storage.

**Differences between CM7 & MotoBlur:**

MotoBlur mounts the internal storage as /mnt/sdcard, which Android will use by default. The external SD Card will be mounted as /mnt/sdcard-ext. Since the naming of the secondary storage on Android devices is immaterial to core operations, this naming is fine.

CyanogenMod however, uses the external SD Card as /mnt/sdcard, this was used as the default set up for in the event of failing storage, you could simply replace it. So if the internal storage ever fails, with CyanogenMod this won't stop you from being able to use your phone normally.

Under CM7, the external SD Card is mounted as /mnt/sdcard and the internal storage is mounted as /mnt/emmc; this is also a more accurate naming, as it easily allows you to differenciate a real, external SDCard (/mnt/sdcard) from internal EMMC storage (/mnt/emmc).

Using the above instructions will just swap the mount points, making /mnt/sdcard your internal EMMC storage, and /mnt/emmc your external SDCard.
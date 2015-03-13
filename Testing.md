
---

# Testing: #

---

---ALWAYS WIPE BEFORE TESTING ANY BUILDS----

Now that we are running CM7 Alpha builds on our phones, it's time to test.
It is important to capture as much information as possible to help us get to the cause of the problems.

### Disclaimer: ###
You were given the opportunity to be the first to use CM7 on the Motorla Atrix because you agreed to test these bugs. Anyone who does not provide regular and detailed Bug feedback (While there are obvious bugs) will be removed from the test group.

**_We are a Community Project that depends on you to do the right thing, this is to benefit all Atrix users around the world._**


## So you discover a bug (at this point everything's a bug). ##
Is the bug already listed in the Issue Tracker?

**Yes:**
  1. Review the already listed bug
  1. If the Bug is the same, then skip adding it
  1. If the Bug is similar but lacks information, add your supplementary notes to the comment of that Issue
  1. Use steps 3 to 6 if no log exist for the bug

**No:**
  1. Try to duplicate the bug.
  1. Note the steps necessary to duplicate it on the phone.
  1. If you can, get a logcat. "adb logcat > logcat.txt" (this will record the log into a text file)
  1. While logcat is running, reproduce the bug.
  1. Once bug is reproduced (allow couple of seconds), in command prompt, press Ctrl + C to stop the log recording.
  1. Find logcat.txt saved on your computer & rename it to align with type of bug. (Example: bluetooth.txt)
  1. Go to the Issue Tab on the site and create a New Issue
  1. Write the problem and the steps clearly on your post. Use the below example to help construct your description.
  1. Attach log using "Attach a file" link below the Description box.



---

## Example Bug Report: ##

---

**Phone (Int/AT&T/etc.):** ATT Atrix

**Radio:** OTA Stock (N\_01.77.30P)

**Hacks/Mods used:** Battery fix, webtop on HDMI, Gtalk on 3g

**Kernel:** Stock



**What is the expected behavior?**

When the google navigation app is started the GPS should lock on within a reasonable amount of time and should remain locked on. Should it lose a lock, it should re-lock within a reasonable amount of time. The "maps" app should operate within the same limits.


**What is the actual behavior?**

When the GPS app is started, the initial lock takes anywhere between 3-5 minutes to get a lock. Once a lock occurs it will remain locked for a short while. It does not lose the lock at the same time intervals, it is sporadic. I've seen it take anywhere from 10-15 minutes. Once a lock is lost and you hear the audible warning... the phone will reboot itself every time. The same issue occurs if you use the "maps" app. You are able to get gps data, but once you lose a lock the phone reboots itself.


**What steps will reproduce the problem?**

  1. Make sure GPS radio is on.
  1. Initiate "navigation app" or "maps"
  1. Wait for a GPS lock
  1. Wait for GPS signal loss


**Possible workarounds:**

None, that I could find.

---

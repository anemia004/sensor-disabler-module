# Sensor Disabler

This Xposed module allows you to modify and disable various sensors on your device. It supports Tasker and filtering which apps will be able to bypass Sensor Disabler.

It has been tested and confirmed working from SDK 21 (Lollipop) to SDK 29 (Pie).

## Installation

### Method 1 – Xposed (APK)
1. Download and install the [Xposed Framework](http://repo.xposed.info/module/de.robv.android.xposed.installer).
2. Install the Sensor Disabler APK:
   - From [IzzyOnDroid](https://apt.izzysoft.de/fdroid/index/apk/com.mrchandler.disableprox) (unofficial F‑Droid repo), or
   - Download the APK from the [Releases page](https://github.com/wardellbagby/sensor-disabler/releases), or
   - Build it from source.
3. Activate the module in Xposed Installer → **Modules**.
4. Reboot.

### Method 2 – Magisk (system app + Xposed)
1. Make sure you have [Magisk](https://github.com/topjohnwu/Magisk) installed.
2. Download the latest **SensorDisabler-Magisk.zip** from the [Releases page](https://github.com/anemia004/sensor-disabler-module/releases/tag/latest-module) of this fork.
3. Open Magisk → **Modules** → **Install from storage** → select the zip.
4. Reboot. The app will appear in your app drawer.
5. Open Xposed Installer → **Modules** → enable **Sensor Disabler**.
6. Reboot once more.

The Magisk module installs Sensor Disabler as a system app systemlessly – no changes to your `/system` partition. It can be easily removed by disabling/removing the module in Magisk and rebooting.

## Automatic Magisk Module Builds
This fork automatically packages the latest APK from the upstream repository into a flashable Magisk module. The build runs daily and is triggered manually as well.  
If you want the latest module, just grab the zip from the `latest-module` release.

## Credits
- Original module by [wardellbagby](https://github.com/wardellbagby)
- Magisk module template and automation added in this fork.

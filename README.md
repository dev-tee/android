# CM for HTC Myst
What works:
- Triple Buffering
- Calls Ingoing/Outgoing
- USB Tethering/Wi-fi Hotspot :) 
- NFC
- Gps
- Camera/Camcorder/Panorama
- etc

What doesn't work:
- Speaker DSP is broken.  The init sequences required to turn the tfa9887 dsp on is different than the open source hal drivers.  Need to do further debugging. (NOT HIGH PRIORITY)
- ???

For all bugs, please open a new issue on github with a logcat and/or dmesg of your issue.

To init this repo:

    repo init -u git://github.com/CyanogenMod/android.git -b cm-11.0
    mkdir -p .repo/local_manifests
    wget https://github.com/CMyst/android/raw/cm-11.0/local_manifest.xml -O .repo/local_manifests/local_manifest.xml

To sync source:

    repo sync

To build:

    . build/envsetup.sh && lunch cm_mystul-userdebug
    mka

Please see the [CyanogenMod Wiki](http://wiki.cyanogenmod.org/) for building instructions.

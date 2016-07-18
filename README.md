# CM12.1 for HTC Myst
What works:
- ?

What doesn't work:
- ?

For all bugs, please open a new issue on github with a logcat and/or dmesg of your issue.

To init this repo:

    repo init -u git://github.com/CyanogenMod/android.git -b cm-12.1
    mkdir -p .repo/local_manifests
    wget https://github.com/CMyst/android/raw/cm-12.1/local_manifest.xml -O .repo/local_manifests/local_manifest.xml

To sync source:

    repo sync

To build:

    . build/envsetup.sh && lunch cm_mystul-userdebug
    mka

Please see the [CyanogenMod Wiki](http://wiki.cyanogenmod.org/) for building instructions.

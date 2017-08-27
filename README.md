# Lineage for HTC Myst

Experimental check-in.
Some files might still need to be organized correctly.
(See [OPA device tree](https://github.com/dev-tee/android_device_htc_opa)).

What works:
- WiFi
- Bluetooth
- NFC

What doesn't work:
- SIM Detection/Cellular Network
- Sound (New HAL required)
- Camera
- more...

For all bugs, please open a new issue on github with a logcat and/or dmesg of your issue.
Additionally if you happen to know how to fix it, shoot me a message or pull request.

To init this repo:

    repo init -u https://github.com/LineageOS/android.git -b cm-14.1
    mkdir -p .repo/local_manifests
    wget https://raw.githubusercontent.com/dev-tee/android/port/local_manifest.xml -O .repo/local_manifests/local_manifest.xml

To sync source:

    repo sync

To build:

    . build/envsetup.sh && lunch lineage_mystul-userdebug
    mka

Please see the [LineageOS Wiki](https://wiki.lineageos.org/devices/) for building instructions.

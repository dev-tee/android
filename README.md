# CM for HTC Myst
What works:
- Triple Buffering
- Calls Ingoing/Outgoing
- Gps
- etc

What doesn't work:
-Speaker DSP is broken.  The init sequences required to turn the tfa9887 dsp on is different than the open source hal drivers.  Need to do further debugging.
- Graphics glitch on right edge of photos taken from camera
- Microphone for camcorder doesn't work
- etc?

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

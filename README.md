# CM for HTC Myst
What doesn't work:
-Camera
-NFC? dma timeout for mdp (graphics glitch in recovery offmode charging animation), possibly caused by dsi_esc_clk and dsi_byte_clk clocks stuck at "on".  Need to do further debugging.

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

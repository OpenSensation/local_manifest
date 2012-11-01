OpenSensation
=========================

Getting Started
---------------

Please see the [Android source page](http://source.android.com/source/index.html) for building instructions.

To initialize your local repository using my trees, use the following command:

    repo init -u git://github.com/CyanogenMod/android.git -b jellybean

Then download our local_manifest.xml

For OS (CM9/ICS) on the Sensation:

    wget -O .repo/local_manifest.xml https://raw.github.com/OpenSensation/local_manifest/pyramid-os/local_manifest.xml

For OS2 (CM10/JB) on the Sensation:

    wget -O .repo/local_manifest.xml https://raw.github.com/OpenSensation/local_manifest/pyramid-os2/local_manifest.xml

For OS2 (CM10/JB) on the Nexus 7:

    wget -O .repo/local_manifest.xml https://raw.github.com/OpenSensation/local_manifest/grouper-os2/local_manifest.xml

Then to sync up:

    repo sync

Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build.

Once you've read that, you can build with

    mka

This will compile everything and use the correct "-j#" flag.

You can also build a flashable zip with

    mka otapackage

Special Thanks
--------------
[@Vorbeth](https://twitter.com/Vorbeth) for all what he has done for our Sensations.

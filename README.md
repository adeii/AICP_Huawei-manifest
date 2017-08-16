[Android Ice Cold Project](http://aicp-rom.com)
====================================


Download the Source
===================

Please read the [AOSP building instructions](http://source.android.com/source/index.html) before proceeding.

Initializing Repository
-----------------------

Repo initialization:

    $ repo init -u https://github.com/adeii/AICP_Huawei-manifest.git -b kitkat


sync repo :

    $ repo sync

***

Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build. This brunch is 4.4.4_r2, newer that kitkat-caf (4.4.2_r2) and working one. Kitkat-caf have blackscreen after bootanimation.

    . build/envsetup.sh
    brunch u8951


You can also build (and see how long it took) for specific devices like this:

    . build/envsetup.sh
    time brunch u8833

Remember to `make clobber` every now and then!

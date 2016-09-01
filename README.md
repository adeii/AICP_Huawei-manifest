[Android Ice Cold Project](http://aicp-rom.com)
====================================


Download the Source
===================

Please read the [AOSP building instructions](http://source.android.com/source/index.html) before proceeding.

Initializing Repository
-----------------------

Repo initialization:
    $ repo init -u https://github.com/adeii/AICP_Huawei-manifest.git -b lp5.1

Sync repo :

    $ repo sync

OR speed-up sync repo as:
    
    $ repo sync --force-sync --no-tags --no-clone-bundle 

Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build.

    . build/envsetup.sh
    time brunch u8833

Remember to `make clobber` every now and then!

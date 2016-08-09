[Android Ice Cold Project](http://aicp-rom.com)
====================================


Download the Source
===================

Please read the [AOSP building instructions](http://source.android.com/source/index.html) before proceeding.

Initializing Repository
-----------------------

Repo initialization:
    $ repo init -u https://github.com/AICP/platform_manifest.git -b lp5.1

Add local manifest:
    mkdir .repo/local_manifests
       
Copy aicp_huawei.xml to .repo/local_manifests and sync repo :

    $ repo sync

***

Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build.

    . build/envsetup.sh
    brunch u8833

Remember to `make clobber` every now and then!

[Another Ice Cold Project](http://aicp-rom.com)
====================================


Download the Source
===================

Please read the [AOSP building instructions](http://source.android.com/source/index.html) before proceeding.

Initializing Repository
-----------------------

Please take note that we have two main line branches depending on which hardware base your phone is working.

If you have a qcom powered device which needs CodeAuroraForum (CAF) BT trees please use the kitkat-caf branch which pulls for the effected packages the correct caf version for you.


To initialize your local repository using the AICP trees, use one of the following commands (without any device/kernel/vendor):

Init core trees for google, exynos and non CodeAuroraForum devices OLD LINK:

    $ repo init -u https://github.com/AICP/platform_manifest.git -b kitkat

for devices which are using CodeAuroraForum trees - HUAWEI Y300, G510, G330:

    original: $ repo init -u https://github.com/AICP/platform_manifest.git -b kitkat-caf
    modded:   $ repo init -u https://github.com/adeii/AICP_Huawei-manifest.git -b kitkat-caf

sync repo :

    $ repo sync

***

Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build. 
*** Maybe /vendor/aicp/product/u8833.mk and u8825.mk and u8951.mk should be made from /device/huawei/u8xx/cm.mk 

    . build/envsetup.sh
For Y300:
    brunch u8833
    
For G510:
    brunch u8951
    
For G330:
    brunch u8825

Remember to `make clobber` every now and then!

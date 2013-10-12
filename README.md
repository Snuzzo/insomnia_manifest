codekill_manifest
=================

InsomniaROM 4.3 is based on (VanirAOSP,AOKP,XenonHD,ParanoidAndroid,Cyanogenmod,CodefireXexperiment,and Linaro!)


Thanks all credits to Team vanir for initial base source......

Getting Started
---------------

INITIALIZING REPOSITORY
=======================

Init core trees without any device/kernel/vendor :

    $  repo init -u git://github.com/InsomniaROM/insomnia_manifest.git -b jb43

Init repo with all devices, kernels and vendors supported by InsomniaROM :

    $ repo init -u git://github.com/InsomniaROM/insomnia_manifest.git -b -g all,kernel,device,vendor

Init repo only for a particular device :

    $ repo init -u git://github.com/InsomniaROM/insomnia_manifest.git -b jb43 -g all,-notdefault,<devicename>,<vendorname>

for example, to init only trees needed to build mako :

    $ repo init -u git://github.com/InsomniaROM/insomnia_manifest.git -b jb43 -g all,-notdefault,mako,lge

Init repo for multiple devices :

    $ repo init -u git://github.com/InsomniaROM/insomnia_manifest.git -b jb43 -g all,-notdefault,<devicename1>,<devicename2>,<devicename3>,<vendorname1>,<vendorname2>,<vendorname3>

for example, to init trees needed to build mako and grouper :

    $ repo init -u git://github.com/InsomniaROM/insomnia_manifest.git -b jb43 -g all,-notdefault,mako,grouper,lge,asus


sync repo :

    $ repo sync


















To initialize your local repository using trees, use the following command:

    repo init -u git://github.com/InsomniaROM/insomnia_manifest.git -b jb43

Then to sync up:

    repo sync -j32
    
    


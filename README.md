TWRP Device Tree for Realme 1
===========================================

The Realme 1 (codenamed _"CPH1861"_) is a mid-range smartphone from Realme, announced in May 2018.

## Status

**Working**:

1. MTP
2. Backup and Restore
3. Flash Stock ROM
4. Flash GSI or Custom ROMs
5. Screenshots now renders correct color
6. OTG Works

**Not working**:

1. Decryption

## Downloads

https://github.com/buddi56/dummy_CPH1859_TWRP/releases

## Device specifications

Basic   | Spec Sheet
-------:|:-------------------------
OS	| Android 8.1 (Oreo), upgradable to Android 9.0 (Pie)	
CPU     | Octa-core (4x2.0 GHz Cortex-A73 & 4x2.0 GHz Cortex-A53)
Chipset | Mediatek MT6771 Helio P60 (12 nm)
GPU     | Mali-G72 MP3
Memory  | 3GB/4GB/6GB RAM
Storage | 32GB/64GB/128GB
MicroSD | up to 256 GB (dedicated slot)
Battery | Non-removable Li-Ion 3410 mAh battery
Resolution | 1080 x 2160 pixels, 18:9 ratio (~402 ppi density)
Camera (Rear)  | 13 MP, f/2.2, PDAF
Rear Camera Features | LED flash, HDR, panorama
Video	| 1080p@30fps	
Camera (Front)  | 8 MP, f/2.2
Features| Accelerometer, gyro, proximity, compass	

## Device picture

![Realme 1](https://images-na.ssl-images-amazon.com/images/I/61lb8GlUZ6L._SL1000_.jpg "Realme 1")



## Getting Started ##
---------------

To get started with OMNI sources to build TWRP, you'll need to get
familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

# repo init

To initialize your local repository using the OMNIROM trees to build TWRP, use a command like this:

    repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0

To initialize a shallow clone, which will save even more space, use a command like this:

    repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0

# repo sync

If you are a first time builder then do check Imp_for_first_time_builders.txt file.
 Then to sync up:

    repo sync -j(nproc) -c

## To Build ##
---------------

Build the TWRP recovery using below command.

    cd <source-dir>; export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch omni_CPH1861-eng; mka recoveryimage

## NOTE

Most of the work here is from internet. Thanks to all the members involved in TWRP project, example DTs and testers.

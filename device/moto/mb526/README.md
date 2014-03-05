Kit Kat for the Motorola Defy/Motorola Defy+


Download:
=========

repo init -u git://github.com/Quarx2k/android.git -b cm-11.0

repo sync


Download RomManager (DELETED BY OUR BUILD SYSTEM)
=================================================

mkdir -p vendor/cm/proprietary
cd vendor/cm && ./get-prebuilts

Build:
======

rm -rf out/target

For CM11 branch :
  source build/envsetup.sh && brunch mb526

or for AOSP :
  source build/envsetup.sh && lunch full_mb526-eng
  mka bacon

Use the signed zip to update the defy with the bootmenu recovery, not the ota package !

Links:
======

XDA ICS Thread : http://forum.xda-developers.com/showthread.php?t=1353003

XDA JB Thread : http://forum.xda-developers.com/showthread.php?t=1768702

XDA KK Thread : http://forum.xda-developers.com/showthread.php?t=2515036
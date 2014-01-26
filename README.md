Device tree for Samsung Galaxy Reverb for CM10 and PAC,
Started by Jimmyk422, continuation by dark_samus 

to start building setup your computer according to:
http://source.android.com/source/initializing.html

then

$ repo init -u https://github.com/CyanogenMod/android.git -b jellybean

after finishing that

$ repo sync <- this will take awhile the source is ~10GB

then

$ cd .repo/local_manifests && cd .repo/local_manifests && wget https://raw2.github.com/dark-samus/android/Jellybean/local_manifest.xml

$ . build/envsetup.sh

$ lunch cm_iconvmu-userdebug

$ make -j# bacon <- # being the number of cores your CPU has +1 

OR

$ mka bacon <- mka = make automatic, you'll have to install an extra package for it


Device tree for Samsung Galaxy Reverb for CM10 and PAC, 

to start building setup your computer according to:
http://source.android.com/source/initializing.html

then $ repo init -u https://github.com/CyanogenMod/android.git -b jellybean

after finishing that

$ repo sync <- this will take awhile the source is ~10GB

then $ cd device 

$ mkdir samsung

$ cd samsung

$ git clone https://github.com/dark-samus/android_device_iconvmu_jb -b master iconvmu

$ cd ../../../vendor

$ mkdir samsung <- this may already exist

$ cd samsung

$ git clone https://github.com/dark-samus/android_vendor_iconvmu_jb -b master iconvmu

$ cd ../..

$ . build/envsetup.sh

$ lunch cm_iconvmu-userdebug

$ make -j# bacon <- # being the number of cores your CPU has +1 

OR

$ mka bacon

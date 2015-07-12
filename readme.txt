$ mkdir -p ~/android/system
$ cd ~/android/system/
$ repo init -u https://github.com/CyanogenMod/android.git -b cm-12.1 --depth=1
$ cd .repo
$ mkdir -p local_manifests
$ cd local_manifests
$ wget https://raw.githubusercontent.com/cix1/manifest/cm-12.1/roomservice.xml

$ cd ~/android/system/
$ source build/envsetup.sh
$ croot
$ repo sync

$ breakfast i9300
$ mka bacon -j1

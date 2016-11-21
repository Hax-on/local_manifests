Building for ZTE Axon 7
=======================

1.) Sync CyanogenMod 13.0

    https://github.com/CyanogenMod/android/tree/cm-13.0

2.) Copy ailsa_ii.xml to .repo/local_manifests/ailsa_ii.xml

    repo sync


2.5) Not really familiar with manifest so you'll have to manually clone and replace
     audio , display, and media HAL from Hax-on to the correct msm8996 paths

     for ex hardware/qcom/media-caf/msm8996 the same goes for audio and display


3.) Initialize build environment

    . build/envsetup.sh


4.) Lunch target device

    lunch cm_ailsa_ii-userdebug or lunch cm_ailsa_ii-eng (For engineering build)


5.) Make that bacon...hmmmmmmmmmmmmmmmmmmmm!!!!

     make bacon -j# (#Number of cpu threads ex: -j4)

# linux-image-5.5.0-rc4-
linux-image-5.5.0-rc4+ kernel ubuntu linux gvt type-c

Deb amd64 https://drive.google.com/open?id=1-1PoJsdQIpkKESxFWvjPlXo5FL-DCC5e

Включено много чего в том числе и проброс видеокарты в виртуальные машины , но не проверено будет ли заводится flatpak , snapd и другие подобные вещи хотя когда эти вещи не работают система быстрее работает. Ядро имеет такие включенные опции как показано ниже это будут как прототипные пути

    /dev/binder
    /dev/hwbinder
    /dev/vndbinder

Материал https://brauner.github.io/2019/01/09/android-binderfs.html


#
# Android
#
CONFIG_ASHMEM=y
CONFIG_ANDROID_VSOC=y
CONFIG_ION=y
CONFIG_ION_SYSTEM_HEAP=y
# end of Android
#
# Android
#
CONFIG_ANDROID=y
CONFIG_ANDROID_BINDER_IPC=y
CONFIG_ANDROID_BINDERFS=y
CONFIG_ANDROID_BINDER_DEVICES="binder,hwbinder,vndbinder"
CONFIG_ANDROID_BINDER_IPC_SELFTEST=y
# end of Android



# Root access on Tinker OS android

Before carrying out these steps you need to install Android on the tinker board and conect required peripherals to it like a keyboard, mouse, screen and connect it to a network where your computer is also connected to.

,,,
This documentation is for windows systems. Linux users need to do the linux equivalent tasks on a linux machine.
,,,

## Preparing the tinker board for root

* Download [termux.apk](https://termux-api.apk.gold/android-6.0.1) and install it on the tinker board

* Enable developer options on the tinker board's android OS by selecting the about phone/tinker board in settings and clickiing on the build number at the bottom repeatedly untill it tells you that you are a developer.

* Go into developer options inside settings and turn on USB debugging.


## Preparing the PC for rooting

* Download [android platform tools](https://developer.android.com/studio/releases/platform-tools) for your operating system and extract it somewhere in your computer which can be easily accessed.

* Download the rootandroid.bat file and paste it in "android platform tools" directory.

* Download flashable Super SU zip file - [Recovery V2.79 Flashable.zip](https://supersuroot.org/download/) and extract it inside "android platform tools" directory, **not** within another directory.

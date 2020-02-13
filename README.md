# Root access on Tinker OS android

>Before carrying out these steps you need to install Android on the tinker board and conect required peripherals to it like a keyboard, mouse, screen and connect it to a network where your computer is also connected to.


> This documentation is for windows systems. Linux users need to do the linux equivalent tasks on a linux machine.

## Preparing the tinker board for root:

* Download [termux.apk](https://termux-api.apk.gold/android-6.0.1) and install it on the tinker board

* Download [SuperSU V2.79.apk](https://supersuroot.org/download/) and install it on the tinker board

* Enable developer options on the tinker board's android OS by selecting the about phone/tinker board in settings and clicking on the build number at the bottom repeatedly untill it tells you that you are a developer

* Go into developer options inside settings and turn on USB debugging


## Preparing the PC for rooting:

* Download [android platform tools](https://developer.android.com/studio/releases/platform-tools) for your operating system and extract it somewhere in your computer which can be easily accessed.

* Download the rootandroid.bat file and paste it in "android platform tools" directory.

* Download flashable Super SU zip file - [Recovery V2.79 Flashable.zip](https://supersuroot.org/download/) and extract it inside "android platform tools" directory, **not** within another directory.

* Make sure that the tinker board and the PC are connected to the same network or prefferably connected to each other via USB or ethernet.

## Rooting tinker board:

> on certain systems youmight have to use ./ before the powershell commands

* Open the "android platform tools" directory and right click while pressing L-shift.

* Select "open power shell wndow here" (the option name might vary) or open CMD/Powershell and cd into the "android platform tools" directory.

* Find the IP address of the tinker board by running "ip a" in termux on the android OS.
```
ip a
```
or go into "about phone" and into "status", here you will find the IP addr also.

* on the powershell run 
```
> adb connect 192.168.xxx.xxx:5555     (replace the tinke rboard IP address in place of the 'x')
```
```
> adb root
```
```
> adb connect 192.168.xxx.xxx:5555     (again)
```
```
> adb shell
```

* Now you will get a root shell of the android system, in the root shell run
```
# mount -o remount,rw /system
```
```
# exit
```

* Now you have to run the rootandroid.bat file
```
> rootandroid.bat
```

* Open the SuperSU app on the android and update the binary

* After the reboot rooting is successfully done

* Now you can open termux in android and get root shell by typing "su" or "tsu"

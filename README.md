# GoldenEye: Source

## The official video trailer

[![IMAGE ALT TEXT HERE](http://i3.ytimg.com/vi/-E4XtdEnWx4/maxresdefault.jpg)](https://www.youtube.com/watch?v=-E4XtdEnWx4)

>## What one needs to play [GES](https://www.geshl2.com)

- A **GOOD PING RESPONSE** internet connection : <50 ms

(then your experience will depend on how far you will be from the server you connect to)

- A **Windows OS** partition (it works well with [bootcamp](https://support.apple.com/fr-fr/HT201468) for macOS users)

==> Download official windows 10 iso image [here](https://www.microsoft.com/fr-fr/software-download/windows10ISO) <==

[Tuto créer clé usb bootable avec rufus](https://lecrabeinfo.net/creer-une-cle-usb-dinstallation-uefi-de-windows-10-8-ou-7.html)

- The game you can download [here](https://geshl2.com/go/5-0-6-full-installer-torrent) in torrent

- [Steam](http://store.steampowered.com/about) and a Steam account

- Source SDK Base 2007 but steam will install this for you if you don't have it

- The [PS4 DualShock Controller](https://www.playstation.com/en-us/explore/accessories/gaming-controllers/dualshock-4)

- [DS4 Windows](http://ds4windows.com) that will let you use a PS4 controller on your pc (even in bluetooth)

___

:bulb: Here is also the "official" [installation guide](http://wiki.geshl2.com/goldeneye/installation)

## How to check if players are online without ~~launching the game~~

>Tested on macOS 10.14 (mojave)

```bash
git clone https://github.com/multiplay/qstat.git
cd qstat
./autogen.sh
./configure && make
make install
qstat -raw "$(printf '\t')" -stm,game=gesource hl2master.steampowered.com:27011 | column -t -s"$(printf '\t')"
```

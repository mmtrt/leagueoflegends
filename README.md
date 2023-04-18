<h1 align="center">
  <img src="snap/gui/leagueoflegends.png" alt="Project">
  <br />
  League of Legends
</h1>

<p align="center"><b>This is the snap for leagueoflegends</b>, <i>"leagueoflegends is a MOBA game developed by Riot Games"</i>. It works on Ubuntu, Fedora, Debian, and other major Linux
distributions.</p>

## Mandatory

**Note:** Game update `13.7+` needed only for old users & not needed for first time install of this snap users.

* You have to install `Vulkan Drivers` and `Vulkan Loader` for both `amd64,i386|lib32` depending on your distro.

* `WINEPREFIX` needs to be refreshed prior to wine 7 migration from 5.

* Move `Riot Games` from `$HOME/snap/leagueoflegends/common/.wine/drive_c` (Skip if redownloading game anyways)

* `snap remove --purge leagueoflegends` when its done check if any old snapshots saved for this snap `snap saved` if yes remove them.

* Remove old runtime snaps `snap remove --purge wine-platform-5-staging` `snap remove --purge wine-platform-runtime` (saves disk space & avoid download updates of these snaps)

* Install league snap again.

* Relaunch snap don't install from region selection dialog close that & then move `Riot Games` back to `$HOME/snap/leagueoflegends/common/.wine/drive_c` (Skip if redownloading game anyways)

## Install

    snap install --edge leagueoflegends
    snap refresh --candidate wine-platform-7-staging

([Don't have snapd installed?](https://snapcraft.io/docs/core/install))

![leagueoflegends](https://res.cloudinary.com/canonical/image/fetch/q_auto,f_auto,w_860/https://dashboard.snapcraft.io/site_media/appmedia/2018/09/lol.png "leagueoflegends")

<p align="center">Published for <img src="http://anything.codes/slack-emoji-for-techies/emoji/tux.png" align="top" width="24" /> with :gift_heart: by Snapcrafters</p>

<h1 align="center">
  <img src="snap/gui/leagueoflegends.png" alt="Project">
  <br />
  League of Legends
</h1>

<p align="center"><b>This is the snap for leagueoflegends</b>, <i>"leagueoflegends is a MOBA game developed by Riot Games"</i>. It works on Ubuntu, Fedora, Debian, and other major Linux
distributions.</p>

## Mandatory

**Note:** Game update `11.17+` .

* You have to install `Vulkan Drivers` and `Vulkan Loader` for both `amd64,i386|lib32` depending on your distro.

* Create fresh `WINEPREFIX` in case you still have issues and see issue `Important Notice` for guide.

## Install

    snap install --edge leagueoflegends
    snap refresh --candidate wine-platform-runtime
    snap refresh --candidate wine-platform-5-staging

## Optional
Users can update `wine-platform-runtime` snap which has updated pkgs like `mesa`,` llvm`, `amd`,`intel`, drivers from `obif` ppa that can support newer `AMD` gpus and newer changes.

	snap refresh --beta wine-platform-runtime

([Don't have snapd installed?](https://snapcraft.io/docs/core/install))

 ## Known Issues and fixes for them:

 ### Game client all black (lol ver 11.17):
1. Install `dxvk` in wineprefix `leagueoflegends.winetricks dxvk`
2. If it is still black doing above create fresh `wineprefix` if this was old snap install before `11.17` game update.
3. Also check for logs from terminal after `snap run leagueoflegends` command.

### Game crashing after character select (lol ver 11.17):
1. Check for logs from terminal after `snap run leagueoflegends` command.
2. If your gpu has low fps with `Vulkan` OR It doesn't support `Vulkan` then dlloverride `dxvk` on main game exe file see ([#182](https://github.com/mmtrt/leagueoflegends/issues/182#issuecomment-907661970)) to run game on `opengl`.

### Game won't install (and will crash instead):
Fresh install snap make sure you have current version of  `snaps` and follow these instructions after installing region of choice.

Wait for both downloads to finish. There are two downloads one after  the other: the client download (`~180MB`) and the game download (`~2.9GB`).

`Do NOT` enter your login details and login or click play, instead just quit the launcher when the two downloads have finished. Then usually start game in login your account.



![leagueoflegends](https://res.cloudinary.com/canonical/image/fetch/q_auto,f_auto,w_860/https://dashboard.snapcraft.io/site_media/appmedia/2018/09/lol.png "leagueoflegends")

<p align="center">Published for <img src="http://anything.codes/slack-emoji-for-techies/emoji/tux.png" align="top" width="24" /> with :gift_heart: by Snapcrafters</p>

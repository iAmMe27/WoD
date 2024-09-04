![Common Issues](img/headers/CommonIssues.png)

## Navigation
1. [Getting Started](README.MD)
2. [Installation](Installation.md)
3. [After Install](PostInstall.md)
4. [Mod Setup](ModSetup.md)
5. [Controls](Controls.md)
6. **[[Common Issues]](CommonIssues.md)**

## Contents
- [Navigation](#navigation)
- [Contents](#contents)
- [Preface](#preface)
- [Download Issues](#download-issues)
    - [Commonly Failing Downloads](#commonly-failing-downloads)
    - [Nexus Login Expired](#nexus-login-expired)
    - [Nexus Server Issue](#nexus-server-issue)
    - [Incorrect Game Files](#incorrect-game-files)
    - [File/Mod not Available](#filemod-not-available)
- [Installation Issues](#installation-issues)
- [Game Crashes](#game-crashes)
  - [Common Crashes](#common-crashes)
    - [1. Overlay Software](#1-overlay-software)
    - [2. Rusty Face Fix](#2-rusty-face-fix)
    - [3. Equip Crash](#3-equip-crash)
    - [4. Crash caused by `XAudio2_7.dll`](#4-crash-caused-by-xaudio2_7dll)
- [Other Post-Install Issues](#other-post-install-issues)
  - [Blurry Textures](#blurry-textures)
  - [I can't move my mouse cursor around the whole area of my screen](#i-cant-move-my-mouse-cursor-around-the-whole-area-of-my-screen)
  - [My game performance sucks!](#my-game-performance-sucks)

## Preface
Please help me to help yourself here. Search this page and the [FAQ](FAQ.md) if you are having issues. Please also use the Discord search function in the WoD channels as your issue may already be solved. Do not just post a question in the support channel without doing your own research first.

## Download Issues

#### Commonly Failing Downloads
It's one of the files on the commonly failing downloads list. Wabbajack even gives you report now, please read that to know exactly what files you missed. [All commonly failing downloads can be found on the Wiki page here.](https://github.com/iAmMe27/WoD/wiki)

#### Nexus Login Expired
Your Nexus login expired. In the Wabbajack settings, log out of Nexus and then re-login.

![Nexus Relog](img/NexusRelog.png)

#### Nexus Server Issue
The Nexus server you are downloading from is having issues, try switching your preferred Nexus download server to something close to your location in the account settings. You can access this area by clicking on your account in the top right, and selecting site preferences.

#### Incorrect Game Files
Your game files are wrong - this will give a clear error in the Wabbajack log, like so:

![Game file error](img/GameFileError.png)

To fix this, you need to ensure your game is set to English in Steam and then verify your game files with Steam.

#### File/Mod not Available
You'll need to wait for a modlist update.

## Installation Issues
1. Hashes don't match for texture files (files that end in `.DDS`) - Your Wabbajack version is outdated, make sure you are using v3.7.0.0 or later.

2. File is corrupt (usually `.ba2` files) - Wabbajack will tell you what file the error is with in its log as well as to delete it and retry the install. Follow the steps given to you by Wabbajack.

3. Your storage drives are full - both the installation drive and the drive you have Wabbajack on need a free space for the installation to be possible.

4. You didn't setup antivirus exclusions.

## Game Crashes
Heavily modded Bethesda games are prone to crashing at times. Generally speaking, the following is true:

1 crash is a fluke, 2 crashes is weird but not impossible, 3 is a repeatable crash worth reporting and/or investigating.

Before you report a crash, consider these rules and also read below to see if your issue is already known about.

### Common Crashes

#### 1. Overlay Software
Software such as **Medal**, **EVGA Precision** and **MSI Afterburner** are the most common causes of this - anything that hooks the display to show or record stuff on screen. Close the software and test again.

#### 2. Rusty Face Fix
This shows up in crash logs with the following things in the stack: `hclClothInstance`, `hclClothData` and hair parts named, like so:

![RFF Log](img/RFFLog1.png)

![RFF Log](img/RFFLog2.png)

The crashes are random and seem to appear more often in areas where lower end PC's performance suffers, which will be different between different PC's. You can turn the active portion of Rusty Face Fix Redux off by opening the INI found in `Rusty Face Fix - WoD INI` and setting the `streaming_mode` to 0. If there is a version of these settings named `Rusty Face Fix - iAm’s Settings` enabled, disable it. *Note: with the active portion switched off, you may see more rust face NPCs as you play.*

#### 3. Equip Crash
This shows up in crash logs with the following things in the stack: `JobListManager::ServingThread` and `PipBoyMapData`, like so:

![Equip Crash](img/EquipCrashLog.png)

This is a very rare crash that WoD has custom mitigations against. To fix, type the following commands into the console:

`player.unequipall`

Followed by:

`player.equipitem 21b3b`

#### 4. Crash caused by `XAudio2_7.dll`
Make sure your WoD folder is added to your antivirus exclusions. If it is, [download Microsoft Redist (June 2010) from here.](https://www.microsoft.com/en-us/download/details.aspx?id=8109)

## Other Post-Install Issues

### Blurry Textures
The low resolution textures you are seeing after playing for a time is caused by Long Loading Times Fix.

This mod aims to reduce loading times, especially when fast travelling or travelling through loading screens but can sometimes remove the loading screen a touch too early, before textures have fully loaded in.

If this behaviour bothers you, it should be safe to switch off mid-save.

### I can't move my mouse cursor around the whole area of my screen
In MO2, under the Essentials separator, find `High Physics FPS Fix - WoD INI` and double click it. In the window that opens, head to INI Files and click the only option in the left column. Find the line:

`Fullscreen=false`

and change it to:

`Fullscreen=true`

### My game performance sucks!
This could be caused by a few things:
  1. You didn't setup a Pagefile as described earlier in this readme or,
  2. You didn't install on an SSD or,
  3. Your hardware doesn't meet the minimum recommended specs.

If you genuinely have followed the above steps then ensure the following:
  1. When setting the pagefile up, you have enough space left on the selected SSD for Windows to allocate the full pagefile size - not having the 20 to 40GB free on the SSD is the same as not having a big enough pagefile in the first place.
  2. You have added your entire WoD installation folder to your antivirus exceptions/allow list - you want the whole folder, not just the Mod Organizer exe.
  3. You have your motherboards XMP/DOCP/EXPO setting switch on - without this setting on, your RAM will be running at the default 2400MHz standard, not the speed you paid for. Enabling this will give a good boost in performance across everything you do but especially games. Of course, not all RAM is capable of clocking higher than the standard 2400MHz but most "gaming" prebuilts and "gaming" level RAM should clock higher if allowed.

*Note: if you did buy a prebuilt PC, the XMP setting is worth a double check - not all system builders enable this setting before shipping you your PC for some reason.*

If you have ensured all of the above is right, try lowering settings in BethINI, [following this guide in the modifications channel on the Discord.](https://discord.com/channels/719714673431150627/1095988679463424000/1096709202052915250)



---

<span style="float:left">

:arrow_backward: [CONTROLS](Controls.md)

</span>

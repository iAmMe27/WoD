![WoD Banner](img/WoDBanner.png)

First things first: **this list contains adult content and you must be of legal age in your country. This means 18+ in most countries, 21+ in others. It is up to you to be sure of the age requirement in your country.**

**Support and general talk about Wasteland of Depravity resides on the Jolly Co-operators Discord:**

[![DiscordButton](img/DiscordButton.png)](https://discord.gg/jolly-coop)

# What is Wasteland of Depravity?
A NSFW Fallout 4 list that's mid-tier compared to previous NSFW lists for Fallout 4. If anything, its more me trying to to get back into modding Fallout 4 for the sake of it!

# Quick Links
- [What is Wasteland of Depravity?](#what-is-wasteland-of-depravity)
- [Quick Links](#quick-links)
- [Before You Start](#before-you-start)
  - [Hardware Requirements](#hardware-requirements)
  - [Accounts](#accounts)
  - [DLC \& Creation Club Content](#dlc--creation-club-content)
- [Installation](#installation)
  - [Preparation](#preparation)
    - [Install Microsoft Visual C++ Redistributable Packages](#install-microsoft-visual-c-redistributable-packages)
    - [Setup your Page File](#setup-your-page-file)
    - [Setup your Shader Cache](#setup-your-shader-cache)
    - [Disable Steam Overlay](#disable-steam-overlay)
    - [Set game language to English](#set-game-language-to-english)
    - [Change Steam's Updating Behavior](#change-steams-updating-behavior)
    - [Clean current Fallout 4 installation](#clean-current-fallout-4-installation)
    - [Install Fallout 4](#install-fallout-4)
    - [Start Fallout 4](#start-fallout-4)
  - [Wabbajack](#wabbajack)
- [Post-Installation](#post-installation)
  - [Stock Game](#stock-game)
  - [Creating a desktop shortcut](#creating-a-desktop-shortcut)
  - [Ultrawide Support](#ultrawide-support)
  - [Optional Mods](#optional-mods)
    - [Essentials Category](#essentials-category)
    - [Character Presets Category](#character-presets-category)
    - [YOUR CHOICES Category](#your-choices-category)
  - [Modifications \& Performance Improvement](#modifications--performance-improvement)
- [Mod Setup](#mod-setup)
- [Controls](#controls)
- [Updating Wasteland of Depravity](#updating-wasteland-of-depravity)
- [Uninstalling Wasteland of Depravity](#uninstalling-wasteland-of-depravity)


# Before You Start
Before you dive in, there's a couple things you need to be sure of first:

## Hardware Requirements
I run a relatively powerful PC with the following specs:
  * CPU: Ryzen 7 5800X3D
  * RAM: 32GB DDR4 @ 3600MHz
  * GPU: RTX 3090

I have not built this list to be as graphically intensive as possible but I have installed some nice texture overhauls and a real nice ENB so, with that in mind, I'd say you would need at least the following specs to run WoD:
  * CPU: Intel 7th gen *OR* AMD Ryzen 3000 series 
  * RAM: 16GB of DDR4
  * GPU: RTX 2060 *or the AMD equivalent with at least 6GB of VRAM*

This could be completely out of field though as I don't have any lower end hardware to test it on.

You will need at least `146GB` of disk space on an SSD for the installation. For the downloads, you will need an extra `96GB`- ideally you want *at least* `250GB` for temporary Wabbajack work space. It doesn't have to be an NVMe SSD, but a HDD of any kind will make the list painfully unplayable. 

## Accounts
In terms of accounts you will need:
  * Nexus Premium Account
  * LoversLab Account
  * [Moddingham Account](https://www.moddingham.com/) - *you need this for the latest version of AAF*

## DLC & Creation Club Content
You will need *all* of the DLC for Fallout 4 ***except*** the official HD texture pack. Seriously, do not download it. 

Creation Club content is not currently supported as I don't own any of it.

# Installation
Please follow all of steps below if it is your first time installing this modlist, if you're updating you can [jump straight there](#updating-WoD).

## Preparation

### Install Microsoft Visual C++ Redistributable Packages
This package is a must as it is needed by MO2 - you may already have it if you've used MO2 before. If you do not have it, you want to download the x64 version under "Visual Studio 2015, 2017 and 2019".

[Download Visual C++ Redistributable Package.](https://docs.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170)

### Setup your Page File
Fallout 4 modlists need a large amount of memory purely because of the amount of *stuff* in them - especially modlists on the larger side or with a lot going on. For the best experience, you should setup a pagefile of at least **20GB** - yes, even if you have a million GB of RAM. To setup your pagefile;

1. Hold down the *LEFT* Windows key and press **R**
2. Type in `systempropertiesadvanced` in the run box and then press ENTER
3. Under the "Performance" option, click the "Settings..." button
4. Switch to the "Advanced" tab
5. Under "Virtual Memory", click the "Change..." button
6. Uncheck `Automatically manage...` if it's checked
7. Select your *fastest* SSD in the list of drives
8. Check "Custom Size"
9. Set `Initial Size` to 20480
10. Set `Maximum Size` to 20480 also
    1.  *Note: you can set this up to 40000 if you have the space, this will let the pagefile expand to as large as 40GB*
11. Press the "Set" button
12. Press OK
13. Press APPLY and then OK
14. Restart your PC to apply the pagefile setting

### Setup your Shader Cache
Driver defaults from Nvidia and AMD for shader cache size is limited to 4GB. Being this small can lead to rare crashes in heavily modified Fallout 4 installs. Increasing the shader cache size is done via the Nvidia Control Panel (I assume the same for AMD users is true also but I don't have AMD hardware to check with). 

*These instructions are Nvidia specific as it is the hardware I have.*

1. Open the NVidia Control Panel
2. Head to `Manage 3D Settings`
3. Scroll down in `Global Settings` to find the `Shader Cache Size` option
4. Set the Shader Cache to *at least* 10GB
5. Done

![Shader Cache](img/ShaderCache.png)

### Disable Steam Overlay
The Steam overlay is known to cause issues when using ENBs. I recommend you turn it off to be sure that it doesn't interfere in any way and you can do so by heading into Steam, right clicking on Fallout 4 in your game library and clicking **Properties** > **General** > **Deselect "Enable Steam Overlay while in-game"**.

### Set game language to English
Wabbajack and some/most of the modding tools out there only support English language versions of games. Setting the language to English in Steam will stop issues like Wabbajack file verification failures when installing. As with disabling the overlay, right click on Fallout 4 in your game library and click **Properties** > **Language** > **Select English**.

### Change Steam's Updating Behavior
If for some reason Bethesda decide to release an update for Fallout 4, everything will probably break. Well, not *everything* but something will definitely break until mods can be updated to suit. To stop this from happening, you need to tell Steam that you only want to update when you tell it to. You can do this by right clicking on Fallout 4 in your game library and clicking **Properties** > **Updates** > **Change Automatic Updates to "Only update this game when I launch it"**. Whilst you're in here, it's also recommended to disable Steam Cloud too.

### Clean current Fallout 4 installation
If you have not yet installed Fallout 4, you can skip this part.

1. Right click on Fallout 4 in your game library and click **Properties** > **Local Files** > **Browse**. 
2. Uninstall the game via Steam - right click on Fallout 4 in your game library and click **Manage** > **Uninstall**.
3. Check the explorer window for any left over files - if there are any, delete them.
4. Open Windows start menu/search and type in `%LOCALAPPDATA%`.
5. Delete the Fallout 4 folder.
6. Head to `Documents\My Games` and delete the Fallout 4 folder.

### Install Fallout 4
Once you've done the steps above, you can now set Steam to download Fallout 4 again but ***do not*** install Fallout 4 to a protected folder, such as `Desktop`, `Downloads` or `Program Files` of any kind. It's best to create a new, dedicated folder for it using the Steam Library function somewhere on the root of your drive such as `C:\SteamLibrary`. A lot of people have a dedicated secondary drive for their games, keeping the OS install separate; using this secondary drive will also work.

### Start Fallout 4
That's right - start the game. You need to let the game do its initial start up jobs such as creating registry entries and generating default config files. Once you've gotten to the main menu you can close the game again.

## Wabbajack
Installing the list is straight forward, Wabbajack will do most of the heavy lifting for you - you only have to tell it where to put stuff. Grab the WoD from the Wabbajack UI, once its downloaded the initial stuff it needs, Wabbajack will have 2 things for you to do - fill in the installation location and the download location. 

Set the installation location to a folder on the root of a drive, something like `C:\WoD`. Do not install it to one of the protected folders as mentioned earlier. The download location will have likely been filled in for you too - ensure it matches the directory you set for the installation location, or if you have multiple Fallout 4 modlists installed, use a common download folder - this will stop you from having to redownload common mods across multiple modlists. 

Before you hit **GO**, a quick tip:

*To get the best performance with Wabbajack, it is recommended that you have the install folder for Wabbajack, the modlist folder and the downloads folder on an SSD; ideally the same SSD.* After the installation is complete, you can move the downloads folder to a storage HDD or other storage medium to save space on your game installation drive. It's not recommended to allow your drive to exceed 90% of its storage space used - Windows Explorer will show a red bar under your drive if you do go over 90% so you need to be sure that you have enough space on your installation drive so that you won't exceed this 90% storage level.

Once you have everything set in Wabbajack, hit **GO** and let it do its thing. It might take a while as there is a fair bit to download and the speed of this will depend on your internet performance as well as your CPU in the later stages for hashing and unpacking the downloads.


# Post-Installation
Almost there but we're not out of the woods yet! After Wabbajack has given you the installation successful screen, you're free to close it. Navigate to the WoD installation folder and run MO2 by double-clicking `ModOrganizer.exe`.

***DO NOT UNDER ANY CIRCUMSTANCES RUN LOOT. The load order is exactly as intended out of the box and you do not need to change it.***

## Stock Game
WoD utilises the stock game feature offered by Wabbajack, meaning that Wabbajack will make a local copy of your Fallout 4 game files during the installation process. This means that your Steam installation of Fallout 4 is completely untouched, even by files that go in the game folder such as ENB files.

## Creating a desktop shortcut
Nobody wants to be launching their game via multiple clicks, they want to be able to do it from the desktop! This is simple to do - open MO2, ensure **WoD** is selected in the dropdown and click the "Shortcut" button. From the small dropdown menu, click "Desktop". Of course, you can always run from inside of MO2 by clicking the "Run" button instead.

![Desktop Shortcut Creation](img/DesktopShortcut00.png)

Done! You should now have a shortcut on your desktop which you can now run the modlist from. Don't run Fallout 4 from within Steam as it won't launch MO2's virtual file system to make a modded game instance.

## Ultrawide Support

My thanks for Swagmeister for figuring this out!

There are a couple of UI mods that allow for Ultrawide resolution support. I don't have an Ultrawide monitor myself, so I can't be 100% sure if this fixes every UI element. To enable Ultrawide support, open the `UI` separator in MO2, and activate `TruBy9 Ultrawide Fallout 4` and `No Rainbox - 21-0 Rainbox Fix`.

![Ultrawide](img/UWMO2.png)

When in game, you will likely need to head into the Mod Config menu > FallUI and tweak some of the widgets to fit your screen space properly.

You will also need to head down the Weapons Overhaul MCM and move the ammo switcher widget to somewhere you prefer.

## Optional Mods
In Wasteland of Depravity, there are a few optional mods that you can toggle on/off for your playthrough.

### Essentials Category
1. Rusty Face Fix - you can toggle this on if you consistently run into the dreaded Fallout 4 rusty face issue, provided you have checked things such as resolution of face textures and tint masks match. Having this enable can cause an issue with the mod forcing the rear head texture to revert back to vanilla textures but it's often very difficult to notice this issue.

### Character Presets Category
1. Maya - Custom Race Female Preset + AAF patch - you should only enable this if you plan on using the Maya character preset for your playthrough. **Do not enable this on an existing save!**

### YOUR CHOICES Category
1. Non-Skimpy Bodyslide Output - I feel as if this is pretty self-explanatory.
2. Skimpy Bodyslide Output - ditto.
3. Discord Rich Presence (F4SE) - this gives you a card in Discord when you are playing WoD. It lists your character name, level and location. *It does not hook into the NSFW mods, don't worry, your secrets are safe.*
4. LOD Hiding Fog for NAC X - adds a small amount of fog to the clear and sunny weathers to help hide those nasty Fallout 4 LODs.
5. Be Afraid - Honest Difficulty Overhaul - YOU MUST START A NEW GAME FOR THIS TO TAKE EFFECT! This mod delevels the Commonwealth to make it dangerous.

## Modifications & Performance Improvement
If you wish to modify the list, even for performance improvements, refer to the `#wod-mods` channel in the Discord server as there you will find guides in the pins that others in the community have already written. You can also use those channels to discuss your changes to the list freely.

**Please don't request help in the official support channel for modifications or modified lists!** It's not because I dislike modifications or anything, it's just impossible to provide support for the thousands of mods and mod combinations available out there.


# Mod Setup

**New advice: For some weird reason, after character creation finishes the game appears to freeze but not crash. A weird, but consistent fix, is to ensure that you open the Body menu when in character creation (default key is B). No idea why but this stops the game from freezing after character creation.**

When starting a new game, create your character and once done, *DO NOTHING ELSE* and allow the mods to initialise. Once the notifications stop appearing in the top left of your screen, proceed to open the door to the bathroom and make your choice as to how you'd like to start the game. 

**DO NOT TRY TO ACTIVATE THE "CLOTHES" OPTION IN LOOKSMENU - IT WILL CRASH YOUR GAME TO DESKTOP AND YOU WILL LOSE YOUR CURRENT CHARACTER CREATION!**
  
* When LIF gives you a pop-up at the start of the game, click `INJECT`
  
* When ECO gives you a pop-up at the start of the game, click `Keep Everything Enabled (Default)`


**Do not touch MCM menus until you are either out of Vault 111 or you have loaded into the Commonwealth.**

The MCM setup is a one-click solution and will run when you tell it to. To do that;

1. Navigate to the Mod Config menu -> `-= MCM Settings Manager =-`
2. Click the `[Apply]` button.

![MCM](img/MCMSettings.jpg)

3. Scroll down and navigate to the `Immersive HUD` menu and then click `Immersive HUD Enabled`.

![iHUD](img/ImmersiveHUDMCM.jpg)

4. Exit the Mod Config menu

5. One that is done, make a new full save from the pause menu.

Done!

# Controls

![](img/keyboard-layout.png)

# Updating Wasteland of Depravity
When an update is released, please always check the [changelog](Changelog.md) first. You may not need to update your modlist but if there is anything that resolves game breaking issues, it'll be noted in the changelog. Backup your saves before you commit to any updates, Wabbajack doesn't usually touch save files, it does has the ability to delete them if it wanted to.

If you have added anything to this modlist at all, Wabbajack will also delete those. You should know how to stop it from doing this if you're going to add stuff to modlists but if you don't, you have to prepend your mod name with `[NoDelete]` - this will make Wabbajack ignore these files. You will need to reinstall these mods and re-sort their load order after an update though, so I hope you kept backup information on where they went in the load order!

All that aside, updates are basically the same as an installation except you have to ensure that you have the "Overwrite" checkbox ticked in Wabbajack.

# Uninstalling Wasteland of Depravity
No fancy uninstallation needed, you can just delete the WoD folder and it'll be gone. There'll be no files left inside your Steam installation folder because WoD uses the stock game feature of Wabbajack.

# WoD Gameplay FAQ

## Contents
- [Contents](#contents)
- [Preface](#before-you-ask-questions-and-look-for-support-in-discord)
    - [Asking in Discord](#asking-for-support-in-discord)
- [Gameplay Questions and Problems](#gameplay-questions-and-problems)
    - [Automatron not starting](#automatron-is-not-starting)
    - [Interior cells too dark](#all-interior-cells-are-way-too-dark)
    - [Too many perk points per level](#im-getting-too-many-perk-points-per-level)

## Before you ask questions and look for support in Discord...
... please read this file and look if you find the answer to your question here.  

If you don't find what you are looking for in here, please use the search function in Discord. There is a good possiblity someone already asked the same or a similar question and you may find what you are looking for in there.

### Asking for support in Discord
If you want to ask for support in Discord, grab the "Wasteland of Depravity" role in onboarding or in "Channels & Roles" at the top of the channel list.  
Please make sure to ask your question in the appropriate channel  

- wod-general -> General discussion about the list or included mods.
- wod-modified -> Support-Channel for non-vanilla WoD installs (if you changed files, added or deleted mods in your WoD install, ask for support here).
- wod-support -> Support-Channel for vanilla (unchanged) WoD installs.

You can find the link to the WoD Discord [here](README.md).

## Gameplay questions and problems

### Automatron is not starting!
WoD uses [Integrated Automatron](https://www.nexusmods.com/fallout4/mods/85317).  
It imposes some delays and requirements before the quest may be started.  
For more information look at the mod page linked above.

> [!TIP]
> There is a known bug in the currently integrated version of the mod that can make it really hard to start Automatron.  
> Resolving the issue includes waiting about a week more than is needed according to the mod page and may include travelling away and to [Wattz](https://fallout.fandom.com/wiki/Wattz_Consumer_Electronics) a few times.  
>   
> This issue will be resolved in the next update of WoD with an updated version of Integrated Automatron.

### All interior cells are way too dark!
Open the ENB menu by pressing SHIFT+ENTER (default keybind).  
MAKE SURE THE Night/Interior preset is set to DEFAULT and not "Bright" under enbadaptation  
under enbadaption, Night> Adapt Max Bightness. lower = brighter
![enb menu](img/GameplayFAQ/enb_interiors.png)

You can also enable the "Interior Lighting Overhaul" in NAC.X  
Open MCM -> NACX -> Settings and enable the setting.
Below is a comparison between the Off and On.

> [!TIP]
> If the settings seemingly does nothing, make a full save, quit to main menu, and reload the save.  
> This seems to happen if you start bilding lights in an interior cell, without reloading the cell, the setting doesn't always work.

![NacX setting comparison](img/GameplayFAQ/nacx.png)

### I'm getting too many perk points per level!
You can adjust how many perk points you get per level.  

In MO2, search for pppl (see screenshot below), right click on it and select "Open in Explorer".  
Then navigate through the folder structure as follows: F4SE -> Plugins.  
There you will find the file pppl.ini  
In the green text at the top of the file you'll find a manual about how the file works. If you just want the default (1 perk point per level), just put 2=1 and delete the rest (see screenshot below).  
Save the file and close the explorer window.  

> [!WARNING]
> If you edit one of the files included in the mod, you should ask for support in the wod-modified channel in discord, as this is now a modified modlist.

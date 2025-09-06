# FAQ

- [FAQ](#faq)
  - [Preface](#preface)
  - [Additions](#additions)
    - [Can I add xyz?](#can-i-add-xyz)
    - [Can I merge profiles?](#can-i-merge-profiles)
  - [Gameplay](#gameplay)
    - [Can I play the vanilla intro?](#can-i-play-the-vanilla-intro)
    - [Where all the crafting recipes?](#where-all-the-crafting-recipes)
    - [How do I acquire *volunteers* for my settlements?](#how-do-i-acquire-volunteers-for-my-settlements)
    - [How do I cure trauma or reset attributes?](#how-do-i-cure-trauma-or-reset-attributes)
    - [Automatron is not starting](#automatron-is-not-starting)
    - [Interior cells are too dark](#all-interior-cells-are-too-dark)
    - [I'm getting too many perk points per level](#im-getting-too-many-perk-points-per-level)
  - [Character Creation \& NPCs](#character-creation--npcs)
    - [Rotating the PC in LooksMenu](#rotating-the-pc-in-looksmenu)
    - [I have/an NPC has a neck seam](#i-havean-npc-has-a-neck-seam)
    - [Do I need to use Bodyslide?](#do-i-need-to-use-bodyslide)
    - [How do I edit my body?](#how-do-i-edit-my-body)
    - [Can I play as a male PC?](#can-i-play-as-a-male-pc)
    - [How do I add/remove tattoo's?](#how-do-i-addremove-tattoos)
  
## Preface
Please help me to help yourself here. Search this page and the [Common Issues page](CommonIssues.md) if you are having issues. Please also use the Discord search function in the WoD channels as your issue may already be solved. Do not just post a question in the support channel without doing your own research first.

## Additions

### Can I add xyz?
If you have to ask, probably not.

### Can I merge profiles?
Refer to the point above.

## Gameplay

### Can I play the vanilla intro?
No. It sucks and the game has been out since like, 2015. If you haven't played it by now, vanilla FO4 still exists.

### Where all the crafting recipes?
I know the mod pages say that they are all in the Chem Station *but* we have ECO and Complex Sorter.

That means, all recipes will have been moved to their appropriate work station in the Universal Workbench. You can follow the quest to grab a portable one by the entrance to Vault 111 or you can make static ones from a settlement build menu.

### How do I acquire *volunteers* for my settlements?
You need to craft a couple things at the Universal Workbench;

1. The Baton - find it in the `Weapon - Create` menu > Human Resources
2. A Kit - find it in the `Utility Station` menu > Human Resources

When an enemy gives up in combat, you can hit them with the baton to get started. Take them back to your settlement and then process them using the Human Resources Terminal.

### How do I cure trauma or reset attributes?
See the nurse in the Memory Den.

### Automatron is not starting
WoD uses [Integrated Automatron](https://www.nexusmods.com/fallout4/mods/85317).  
It imposes some delays and requirements before the quest may be started.  
For more information look at the mod page linked above.

### All interior cells are too dark
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

### I'm getting too many perk points per level
You can adjust how many perk points you get per level.  

In MO2, search for pppl (see screenshot below), right click on it and select "Open in Explorer".  
Then navigate through the folder structure as follows: F4SE -> Plugins.  
There you will find the file pppl.ini  
In the green text at the top of the file you'll find a manual about how the file works.  

If you just want the default (1 perk point per level), just put 2=1 and delete the rest (see screenshot below).  
Save the file and close the explorer window.  

> [!WARNING]
> If you edit one of the files included in the mod, you should ask for support in the wod-modified channel in discord, as this is now a modified modlist.

![pppl search in mo2](/img/GameplayFAQ/pppl_mo2.png)
![pppl file edit](/img/GameplayFAQ/pppl_file.png)


## Character Creation & NPCs

### Rotating the PC in LooksMenu
We have a mod for that.

- Right Mouse Button enables rotation;
- Middle Mouse Button enables movement of the character up, down, left and right;
- Shift + Mouse Wheel to zoom in and out.

### I have/an NPC has a neck seam
A lot of FO4 skin mods don't come with matching face textures, therefore leaving an obvious seam between the neck and body. Head into the High Poly Faces REDUX MCM and enable the `Seamless High Poly Head` for the player and then follow its instructions to fix it.

### Do I need to use Bodyslide?
No. See below.

### How do I edit my body?
2 ways;

1. In LooksMenu > Body > Advanced - play with the sliders to your hearts content.
2. Press F3 to open the Screen Archer Menu > Looks > Body Morphs > Load and pick a body preset.

### Can I play as a male PC?
You can if you want.

### How do I add/remove tattoo's?
In LooksMenu, Body sub-menu > Overlays.

If they are tattoos added on defeat, you can't remove them this way, go see the guy in the Dugout Inn.
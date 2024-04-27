![Common Issues](img/headers/CommonIssues.png)

## I get download errors when installing WoD!
I bet it's one of the files on the commonly failing downloads list. [All commonly failing downloads can be found on the Wiki page here.](https://github.com/iAmMe27/WoD/wiki)

## My game crashes on startup!
Software such as **Medal**, **EVGA Precision** and **MSI Afterburner** are the most common causes of this - anything that hooks the display to show or record stuff on screen. Close the software and test again.

## I can't move my mouse cursor around the whole area of my screen!
In MO2, under the Essentials separator, find `High Physics FPS Fix - WoD INI` and double click it. In the window that opens, head to INI Files and click the only option in the left column. Find the line:

`Fullscreen=false`

and change it to:

`Fullscreen=true`

## My game performance sucks!
This could be caused by a few things:
  1. You didn't setup a Pagefile as described earlier in this readme or,
  2. You didn't setup your shader cache as described earlier in this readme or,
  3. You didn't install on an SSD or,
  4. Your hardware doesn't meet the minimum recommended specs.

If you genuinely have followed the above steps then ensure the following:
  1. When setting the pagefile up, you have enough space left on the selected SSD for Windows to allocate the full pagefile size - not having the 20 to 40GB free on the SSD is the same as not having a big enough pagefile in the first place.
  2. You have added your entire WoD installation folder to your antivirus exceptions/allow list - you want the whole folder, not just the Mod Organizer exe.
  3. You have your motherboards XMP/DOCP/EXPO setting switch on - without this setting on, your RAM will be running at the default 2400MHz standard, not the speed you paid for. Enabling this will give a good boost in performance across everything you do but especially games. Of course, not all RAM is capable of clocking higher than the standard 2400MHz but most "gaming" prebuilts and "gaming" level RAM should clock higher if allowed.

*Note: if you did buy a prebuilt PC, the XMP setting is worth a double check - not all system builders enable this setting before shipping you your PC for some reason.*

If you have ensured all of the above is right, try lowering settings in BethINI, [following this guide in the modifications channel on the Discord.](https://discord.com/channels/719714673431150627/1095988679463424000/1096709202052915250)

## I get a crash caused by XAudio2_7.dll!
Make sure your WoD folder is added to your antivirus exclusions. If it is, [download Microsoft Redist (June 2010) from here.](https://www.microsoft.com/en-us/download/details.aspx?id=8109)

---

<span style="float:left">

### :arrow_backward: [CONTROLS](Controls.md)

</span>
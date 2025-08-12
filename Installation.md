![Installation](img/headers/Installation.png)

<p align="center">
[ <a href="https://github.com/iAmMe27/WoD/blob/main/README.md">Getting Started</a> ]
[ Installation ]
[ <a href="https://github.com/iAmMe27/WoD/blob/main/PostInstall.md">After Install</a> ]
[ <a href="https://github.com/iAmMe27/WoD/blob/main/ModSetup.md">Mod Setup</a> ]
[ <a href="https://github.com/iAmMe27/WoD/blob/main/Controls.md">Controls</a> ]
[ <a href="https://github.com/iAmMe27/WoD/blob/main/CommonIssues.md">Common Issues</a> ] 
</p>

&nbsp;

>[!WARNING]
> I recommend that you setup 2 folders for your installation. For example, use `C:\WoD` for your installation folder and `C:\WoD Downloads` for your downloads folder.


## Preparation

> [!CAUTION]
> **The steps listed here are not optional and must be followed.**

### Setup your Page File
You should setup a pagefile of at least **20GB** - yes, even if you have a million GB of RAM. To setup your pagefile;

1. Hold down the *LEFT* Windows key and press **R**
2. Type in `systempropertiesadvanced` in the run box and then press ENTER
3. Under the "Performance" option, click the "Settings..." button
4. Switch to the "Advanced" tab
5. Under "Virtual Memory", click the "Change..." button
6. Uncheck `Automatically manage...` if it's checked
7. Select your *fastest* SSD in the list of drives
8. Check "Custom Size"
9. Set `Initial Size` to 20480
10. Set `Maximum Size` to 40000
11. Press the "Set" button
12. Press `OK`
13. Press `APPLY` and then `OK`
14. Restart your PC to apply the pagefile setting

### Setup your Antivirus
Before you go down the route of "I don't have an antivirus" - you do, it's built into Windows. You need to exclude your Wabbajack folder and your WoD installation folder from your antivirus' real-time protection stuff as it will likely interfere with your install and worst case, it can remove files, ruining your install. It can and will interfere whilst you are playing too, causing poor performance and obvious stuttering.

> [!TIP]
> How do I do this, you ask? [Click here to find out how.](https://support.microsoft.com/en-gb/windows/add-an-exclusion-to-windows-security-811816c0-4dfd-af4a-47e4-c301afe13b26)


**Note:** If you're using Webroot or any other free 3rd party antivirus it's likely that adding the folders to exclusions will not be enough and you'll need to disable or uninstall your 3rd party AV as they can incorrectly mark `usvfs_proxy_x86.exe`, among other files, as a virus, a file needed for Mod Organizer 2 to work. We recommend doing so anyway in case it's a free one, as Windows Defender is likely much better at stopping threats than that is (according to data from av-test.org https://www.av-test.org/en/antivirus/home-windows/).

### Disable Steam Overlay
Head into Steam, right clicking on Fallout 4 in your game library and clicking **Properties** > **General** > **Deselect "Enable Steam Overlay while in-game"**.

### Set game language to English
Right click on Fallout 4 in your game library and click **Properties** > **Language** > **Select English**.

### Change Steam's Updating Behavior
Right click on Fallout 4 in your game library and clicking **Properties** > **Updates** > **Change Automatic Updates to "Only update this game when I launch it"**. Whilst you're in here, it's also recommended to disable Steam Cloud too.

### Install Fallout 4
Once you've done the steps above, you can now set Steam to download Fallout 4 but ***do not*** install Fallout 4 to a protected folder, such as `Desktop`, `Downloads` or `Program Files` of any kind. It's best to create a new, dedicated folder for it using the Steam Library function somewhere on the root of your drive such as `C:\SteamLibrary`. A lot of people have a dedicated secondary drive for their games, keeping the OS install separate; using this secondary drive will also work.

### Start Fallout 4
Yup - start the game. ಠ_ಠ

## Download non-Nexus mods
It is required that you download all non-Nexus mods in your browser prior to running Wabbajack. All links to mods not hosted on Nexus Mods can be [found here](https://github.com/iAmMe27/WoD/wiki/).

> [!WARNING]
> Currently, downloading Loverslab mods through wabbajack does not work. Even though it shows the mod page and you can click the download button, it will not pass the file check at the end and Wabbajack will throw an error. Don't skip this step, even if you successfully downloaded LL mods through wabbajack in the past.

## Wabbajack
Installing the list is straight forward, Wabbajack will do most of the heavy lifting for you - you only have to tell it where to put stuff.

### Installation Folder
Set the installation location to a folder on the root of a drive, something like `C:\WoD`. If you have multiple Fallout 4 modlists installed, use a common download folder - this will stop you from having to redownload common mods across multiple modlists. 

> [!CAUTION]
> Do not install WoD to your game folder or in any protected folders such as your Documents or Program Files.

Once you have everything set in Wabbajack, hit **GO** and let it do its thing.

### Wabbajack errors
If you encounter any errors during the installation process, have a look at our [FAQ](FAQ.md#common-wabbajack-errors). 

# Continuing
If Wabbajack was able to install the modlist without any errors, you can continue with the [After Installation steps](PostInstall.md).

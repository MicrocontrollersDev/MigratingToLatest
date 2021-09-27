# Migrating to 1.17

# Note

[Join my Discord for news regarding the development of this repository!](https://discord.gg/eXkMKCqtfQ)

If you would like to contribute, please make a PR.  
Some notes:
- Leave your name and GitHub link in the credits section in alphabetical order, even for a tiny change
- Please try to use Modrinth/GitHub over Curseforge when applicable
- Please use a GitHub link instead of a Modrinth link for Author credit and avoid using Curseforge as best you can, and use the modder organization when applicable
- Make sure that the option to allow me to make changes to your PR is enabled

## Introduction

### The Situation

So, you've been playing on 1.8 for the past [5.5 years](https://howoldisminecraft189.today/) and are ready to see what 1.17 has to offer. Your first thought may be to download and install Forge and then add OptiFine as a mod, but this could not be further from the best choice. As Mojang have been been rolling out releases, they've also been decreasing performance with every version, and neither Forge nor OptiFine are really able to bring back even a speck of that performance that we see in 1.12 and below. However, another mod loader, Fabric, which is lightweight and easier to develop for, has created an amazing community in which many of its members focus on helping optimize the game to its greatest potential.

### Why no longer OptiFine?

OptiFine no longer provides the benefit that it once did on older versions of the game. As the years have gone by and Minecraft's code has changed, OptiFine has been continuing to completely overwrite major parts of Minecraft's code. Because OptiFine is closed source, it has become increasingly harder for modders to provide OptiFine compatibility. OptiFine also uses outdated formats for many of its features, including MCPatcher and its confusing and outdated settings menu. Many members in the Fabric community have taken it upon themselves to create better performance enhancing mods which surpass OptiFine, as well as provide alternatives to many of OptiFine's iconic features.

While there is a Fabric compatibility layer for OptiFine known as OptiFabric, it is unsupported by many of the mods on the list, with some outright preventing the game from loading if OptiFabric is present. Therefore, consider all mods in this list to be incompatible with OptiFabric.

### Why no longer Forge?

Forge has always been less than ideal for performance due to its large overhead for server-sided modding, which is not necessary for users wishing for a vanilla compatible experience. Fabric on the other hand is extremely lightweight and is practically identical to vanilla. It's also considered to be much easier to make mods for and is being used as the stepping tool for [Quilt](https://quiltmc.org/faq), an in-progress mod loader which will provide many more benefits to modders.

## Installing Fabric

TODO: add images

0. Make sure you close Minecraft and the Minecraft launcher before installing Fabric, otherwise unexpected things can happen.
1. Download the [Fabric installer](https://fabricmc.net/use).
    - If you are on Windows, use the `.EXE` version of the installer on the right.
    - If you are on any other operating system or the `.EXE` version is not working for you, then use the `.JAR` version on the left.
2. Run the installer.
    - If you are using the `.EXE` version of the installer, simply double click the file. You may get a popup blocking you from running the installer and saying that "Windows protected your PC"; if so, then click on `More info` and then `Run anyway`.
    - If you are using the `.JAR` version, you will need to have Java installed on your device. If you have Java installed, then double click the downloaded file to run the installer. If you don't, then follow these steps:
        1. Go to the [Java downloads page](https://adoptium.net/?variant=openjdk17&jvmVariant=hotspot) and download the version of Java corresponding to your device.
        2. Run the Java installer by double clicking it.
        3. Do whatever the installer tells you to do.
        4. After installing Java, you should be able to run the Fabric installer by double clicking it. If you still can't for some reason, try running the program [Jarfix](https://johann.loefflmann.net/downloads/jarfix.exe).
3. Now that you have opened the installer, you will see two tabs at the top of the window: `Client` and `Server`. Make sure you are on the `Client` tab. Then, open the `Minecraft Version:` dropdown and select the version of Minecraft you want (most likely the latest version of Minecraft). The rest of the settings can be left with their defaults (unless you store your Minecraft version files in a different folder; if you want to use a different directory for this installation, that should be changed in the Minecraft launcher, not here). Click on `Install` when you are ready to install Fabric.
4. Once Fabric is finished installing, open your Minecraft launcher and click on the profiles button at the bottom left corner. Select the Fabric profile, it should be called something like `fabric-loader-1.17.x`. Then hit `PLAY` to start playing!
    - If you do not see the profile, try exiting and reopening the Minecraft launcher. If this also does not work, go to the `Installations` tab in the Minecraft launcher and make sure the `Modded` option is ticked on the rop right corner. If it still does not show up, create your own installation by clicking the `New installation` button, and selecting your desired fabric version in the `Version` dropdown. Then press `Create` and launch this installation.

## Installing Mods on Fabric

TODO: note about custom directories

0. Make sure you close Minecraft before installing mods, otherwise unexpected things can happen.
1. Open your Minecraft folder:
    - Windows: Click on the Start button at the bottom left corner of your screen. Then type in `%appdata%` and hit enter. Open the folder called `.minecraft`.
    - Mac: On the bar at the top of your screen in Finder, click `Go`, then click `Go to Folder` and type `~/Library/Application Support/Minecraft`, then hit enter.
    - Linux: Open `~/.minecraft`.
2. In your Minecraft folder, open the folder called `mods`.
    - If this folder does not exist, create it.
3. Place all of the mods you want to use into this folder (note that all mods you install must be for Fabric 1.17 or they will not work).

## Mods

### Dependencies

These are essential mods that are pretty much required for most fabric mods as dependencies.

| Mod | Description | Author |
| --- | --- | --- |
| [Fabric API](https://modrinth.com/mod/fabric-api) | Required for most Fabric mods. | [Fabric Team](https://github.com/FabricMC) |
| [Fabric Language Kotlin](https://www.curseforge.com/minecraft/mc-mods/fabric-language-kotlin) | Required for mods that use Kotlin. | [Fabric Team](https://github.com/FabricMC) |
| [Mod Menu](https://modrinth.com/mod/modmenu) | Allows the user to see all installed mods ingame, as well as access the config for most. | [Terraformers](https://github.com/TerraformersMC) |
| [Essential](https://essential.gg)| Essential allows you to customize your character, chat with friends, and invite them to your worlds. It also adds a few quality of life features, such as zoom. | [Sk1erLLC](https://sk1er.club/) + [SparkUniverse](https://sparkuniverse.com/) |

### Performance

These are mods that are needed for playing the latest versions of Minecraft at a reasonable FPS. These will also help decrease frame times, hopefully eliminating spikes or stuttering.

| Mod | Description | Author | Incompatibilities |
| --- | --- | --- | --- |
| [Sodium](https://irisshaders.github.io "https://modrinth.com/mod/sodium") | **Currently comes bundled with Iris!** An all around performance mod, Sodium allows users to play the latest versions of Minecraft with high FPS, completely outperforming OptiFine, with some users seeing up to 8x their vanilla frames. Sodium also drastically improve visuals, providing a much better gameplay experience. | [CaffeineMC](https://github.com/CaffeineMC) | DashLoader |
| [Iris](https://irisshaders.github.io) | Iris is a shader loader that allows users to load up their favorite OptiFine shaderpacks, but with much higher FPS. Iris also provides performance enhancements when not using shaders, making it great for all users. | [IrisShaders](https://github.com/IrisShaders) | DashLoader |
| [Indium](https://modrinth.com/mod/indium) | Indium adds FRAPI support to Sodium, making it necessary to use for some of the mods on this list to work. This mod is merely temporary and will be removed once Sodium adds FRAPI support itself. | [comp500](https://github.com/comp500) |
| [Hydrogen](https://modrinth.com/mod/hydrogen) | Hydrogen helps reduce the amount of memory the game takes up. While this is mostly meant for large modpacks, it does not hurt using it for a vanilla experience. | [CaffeineMC](https://github.com/CaffeineMC) | DashLoader |
| [Lithium](https://modrinth.com/mod/lithium) | Lithium helps improve the performance of many vanilla systems without changing their mechanics. | [CaffeineMC](https://github.com/CaffeineMC) |
| [Starlight](https://www.modrinth.com/mod/starlight) | Starlight completely rewrites the light engine to make loading chunks much quicker. | [SpottedLeaf](https://github.com/Spottedleaf) |
| [LazyDFU](https://modrinth.com/mod/lazydfu) | LazyDFU prevents the DataFixerUpper from doing anything until it is required, improving your Minecraft start times. | [astei](https://github.com/astei) |
| [Enhanced Block Entities](https://modrinth.com/mod/ebe) | Enhanced Block Entities improves block entities by making them used baked models instead, allowing for better performance, visuals (via better smoothlighting), and better resource pack customizability. | [FoundationGames](https://github.com/FoundationGames) |
| [FerriteCore](https://modrinth.com/mod/ferrite-core/versions) | FerriteCore further reduces memory usage and should be used in conjunction with Hydrogen. | [malte0811](https://github.com/malte0811) |
| [Entity Culling](https://www.curseforge.com/minecraft/mc-mods/entityculling) | EntityCulling culls entities that you cannot see, increasing FPS. | [tr9zw](https://github.com/tr7zw) |
| [Dynamic FPS](https://modrinth.com/mod/dynamic-fps) | Dynamic FPS reduces your FPS, and therefore reduces your system load, when tabbed out of the game. | [juliand665](https://github.com/juliand665) |

### Recommended

These are mods that I recommend you to use at all times. While they may not boost performance, they are mostly quality of life mods meant to better your experience.

| Mod | Description | Author | Incompatibilities |
| --- | --- | --- | --- |
| [Mod Manager](https://modrinth.com/mod/modmanager) | An extension of Mod Menu, Mod Manager allows the user to download and install mods in game in the Mod Menu screen, as well as update outdated mod. | [DeathsGun](https://github.com/DeathsGun) |
| [Item Model Fix](https://www.curseforge.com/minecraft/mc-mods/item-model-fix) | Item Model Fix fixes the gaps you see on items when holding them. This makes for a much more pleasant experience for most texturepacks. | [Pepper_Bell](https://github.com/PepperCode1) |
| [Borderless Mining](https://www.curseforge.com/minecraft/mc-mods/borderless-mining) | **No 1.17.1 Yet** Borderless Fullscreen for Minecraft. Instructions on how to manually update it to 1.17.1 can be found [here](https://www.curseforge.com/minecraft/mc-mods/borderless-mining?comment=65) | [comp500](https://github.com/comp500) |
| [Not Enough Crashes](https://modrinth.com/mod/notenoughcrashes) | Not Enough Crashes takes you to the main screen instead of exiting the game when you crash. | [natanfudge](https://github.com/natanfudge) |
| [CleanView](https://www.curseforge.com/minecraft/mc-mods/cleanview-fabric) | CleanView prevents self particles from appearing on your screen. | [LianMI](https://github.com/zlainsama) |
| [Smooth Scrolling Everywhere](https://www.curseforge.com/minecraft/mc-mods/smooth-scrolling-everywhere-fabric) | Smooth Scrolling Everywhere makes the scrolling in all menus smoother. | [Shedaniel](https://github.com/shedaniel) |
| [No Potion Offset](https://www.curseforge.com/minecraft/mc-mods/no-potion-offset/) | **No 1.17.1 Yet.** No Potion Offset prevents your inventory from getting shifted over when you have an active potion effect. | [Shedaniel](https://github.com/shedaniel) |
| [Controlling](https://www.curseforge.com/minecraft/mc-mods/controlling-for-fabric) | Controlling completely revamps Minecraft's controls menu, making it much easier to navigate and change keys. | [Jaredllll08](https://github.com/jaredlll08) |
| [Wyvtils](https://github.com/Qalcyo/Wyvtils/releases/tag/v1.2.0-beta9) | **1.17.1 Version in beta** Wyvtils adds many useful utilities to the game, such as nametags, bossbar, action bar, sidebar, hitbox customization and more. | [Qalcyo](https://github.com/Qalcyo)
| [KronHUD](https://www.curseforge.com/minecraft/mc-mods/kronhud) | KronHUD adds many useful HUD elements to your screen with an easy to use in game config. | [DarkKronicle](https://github.com/DarkKronicle) |

### Other Cool Mods

These are mods that are more dependant on personal preferance than importance.

| Mod | Description | Author | Incompatibilities |
| --- | --- | --- | --- |
| [Custom Selection Box](https://github.com/NKID00/CustomSelectionBox-New/releases/latest) | **Currently using an updated fork.** Custom Selection Box is equivalent to 1.8's block overlay, allowing you to customize the outline when highlighting blocks. | [LordDeatHunter](https://github.com/LordDeatHunter) |
| [No View Bobbing Screen Shake](https://modrinth.com/mod/viewbobbingmod) | No View Bobbing Screen Shake removes the screen shaking when view bobbing is turned on, leaving only the swaying hand. | [InboundBark](https://github.com/InboundBark) |
| [Slight GUI Modifications](https://www.curseforge.com/minecraft/mc-mods/slight-gui-modifications) | Slight GUI Modifications adds animations to many GUI elements. | [Shedaniel](https://github.com/shedaniel) |
| [Colored Lights](https://modrinth.com/mod/colored-lights) | Colored Lights adds colored lighting to Minecraft with its colors completely customizable via resource pack. | [Gegy](https://github.com/Gegy) | Iris/Sodium |
| [Blur](https://modrinth.com/mod/blur-fabric) | Blur creates a nice blur effect when in menus and is completely customizable. | [Motschen](https://github.com/Motschen) | Rainbowify |
| [Rainbowify](https://modrinth.com/mod/rainbowify) | Replaces the dark gui backrounds with a smooth rainbow one. | [Lennox](https://github.com/officialLennox) | Blur |
| [No Fade](https://github.com/UltimateBoomer/mc-no-fade/releases/latest) | No Fade removes the fading animation that Mojang added between their splash screens. | [UltimateBoomer](https://github.com/UltimateBoomer) |
| [WaveyCapes](https://www.curseforge.com/minecraft/mc-mods/waveycapes/files) | WaveyCapes breaks your cape into smaller sections to make its movement more fluid. Looks great with the new migration capes. | [tr9zw](https://github.com/tr7zw) |
| [Mojangster](https://www.curseforge.com/minecraft/mc-mods/mojangster/files) | Mojangster allows an animated loading screen. Looks pretty cool. | [cal6541](https://github.com/cal6541) |

### OptiFine Replacements

As OptiFine is no longer recommended, here are some replacements for many of it's features that have not already been listed above.

| Mod | Description | Author | Incompatibilities |
| --- | --- | --- | --- |
| [Sodium Extra](https://modrinth.com/mod/sodium-extra) | OptiFine extra settings toggles. Adds most of OptiFine's such as animations, particles, rain/snow, clouds, sky and biome colors, and more, as well as some custom ones. | [FlashyReese](https://github.com/FlashyReese) | DashLoader |
| [Essential](https://essential.gg) | Zoom. More customizable than OptiFine's. | [Sk1erLLC](https://sk1er.club/) |
| [Bobby](https://modrinth.com/mod/bobby) | Higher render distances. More customizable than OptiFine's. | [Johni0702](https://github.com/Johni0702) | Starlight |
| [LambDynamicLights](https://modrinth.com/mod/lambdynamiclights) | Dynamic lights. More customizable than OptiFine's. | [LambdAurora](https://modrinth.com/user/rRnTb0fG) |
| [LambdaBetterGrass](https://modrinth.com/mod/lambdabettergrass) | Better grass and better snow. More customizable than OptiFine's. | [LambdAurora](https://modrinth.com/user/rRnTb0fG) | DashLoader |
| [Cull Leaves](https://modrinth.com/mod/cull-leaves) | Smart leaves. | [MidnightDust](https://github.com/TeamMidnightDust) |
| [Fabrishot](https://modrinth.com/mod/fabrishot) | Higher resolution Screenshots. | [ramidzkh](https://modrinth.com/user/z0r5biKh) |
| [Clear Skies](https://www.curseforge.com/minecraft/mc-mods/clear-skies) | Removes fog color banding on skybox. | [grondag](https://github.com/grondag) |
| [Custom Splash Screen](https://modrinth.com/mod/custom-splash-screen) | Custom loading screen colors. Does not support OptiFine format. | [MidnightDust](https://github.com/TeamMidnightDust) |
| [FabricSkyboxes](https://modrinth.com/mod/fabricskyboxes) | Custom sky. Does not support OptiFine format. | [AMereBagatelle](https://modrinth.com/user/ifLBWnLs) |
| [Continuity](https://modrinth.com/mod/continuity) | CTM. Supports OptiFine format. | [Pepper_Bell](https://github.com/PepperCode1) | DashLoader |
| [Chime](https://modrinth.com/mod/chime) | **No 1.17.1 Yet.** CIT. Does not support OptiFine format. | [Emi](https://modrinth.com/user/R6WsWKy9) |
| [Colormatic](https://github.com/kvverti/colormatic/releases/latest) | Custom colors. Does not support OptiFine format. | [Thalia](https://github.com/kvverti) |
| [Transparent](https://www.curseforge.com/minecraft/mc-mods/transparent-fabric) | **No 1.17.1 Yet.** Transparent textures. Does not support OptiFine format. | [Trikzon](https://github.com/Trikzon) |
| [Varied Mob Textures](https://www.curseforge.com/minecraft/mc-mods/varied-mob-textures) | **No 1.17.1 Yet.** Varied mob textures. Does not support OptiFine format. | [Digifox03](https://github.com/Digifox03/variedMobs) |
| [Custom Entity Models](https://www.curseforge.com/minecraft/mc-mods/custom-entity-models-cem) | Custom entity models. Supports OptiFine format. | [dorianpb](https://github.com/dorianpb) |

## Contributors

- [BobIsMyManager](https://github.com/BobIsMyManager)
- [karmette](https://github.com/karmette)
- [nacrt](https://github.com/nacrt)
- [NoPro2024](https://github.com/NoPro2024)
- [lis](https://github.com/Lisenaaaa)

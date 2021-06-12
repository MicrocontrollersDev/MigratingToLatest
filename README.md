# Switching to 1.17

# Note

If you would like to contribute, please make a PR (and please add your name to credits, even if you didn't do much). You can also make an issue listing any mods you would like to add to the list or any you think should be replaced with a better alternative.

## Introduction

So, you've been playing on 1.8 for the past 5 years and are ready to see what 1.17 has to offer. Your first thought may be to download and install Forge and then add OptiFine as a mod, but this could not be further from the best choice. As Mojang have been been rolling out releases, they've also been rolling out slower performance (bad sentence, needs fixing, i cba rn), and neither Forge nor OptiFine are really able to bring back even a speck of that performance that we see in 1.12 and below. However, another mod loader, Fabric, which is lightweight and easier to develop for, has created an amazing community in which many of its members focus on helping optimize the game to its greatest potential.

## Installing Fabric

TODO: Add instructions for MultiMC, also maybe add images because images are pog

1. Download the [Fabric installer](https://fabricmc.net/use/).
    - If you are on Windows, use the `.EXE` version of the installer on the right.
    - If you are on any other OS or the `.EXE` version is not working for you, then use the `.JAR` version on the left.
2. Run the installer.
    - If you are using the `.EXE` version of the installer, simply double click the file. You may get a popup blocking you from running the installer and saying that "Windows protected your PC"; if so, then click on `More info` and then `Run anyway`.
    - If you are using the `.JAR` version, you will need to have Java installed on your device. If you have Java installed, then double click the downloaded file to run the installer. If you don't, then follow these steps:
        1. Go to the [Java downloads page](https://java.com/en/download/manual.jsp) and download the version of Java corresponding to your device.
        2. Run the Java installer by double clicking it.
        3. Do whatever the installer tells you to do.
        4. After installing Java, you should be able to run the Fabric installer by double clicking it. If you still can't for some reason, try running the program [Jarfix](https://johann.loefflmann.net/downloads/jarfix.exe).
3. Now that you have opened the installer, you will see two tabs at the top of the window: `Client` and `Server`. Make sure you are on the `Client` tab. Then, open the `Minecraft Version:` dropdown and select the version of Minecraft you want (most likely the latest version of Minecraft). The rest of the settings can be left with their defaults (though if you want the profile to be in a different folder from `.minecraft` you can change that here). Click on `Install` when you are ready to install Fabric.
4. Once Fabric is finished installing, open your Minecraft launcher and click on the profiles button at the bottom left corner. Select the Fabric profile, it should be called something like `fabric-loader-1.17.x`. Then hit `PLAY` to start playing!

## Installing Mods on Fabric

0. Make sure you close Minecraft before installing mods, otherwise unexpected things can happen.
1. Open your Minecraft folder:
    - Windows: Click on the Start button at the bottom left corner of your screen. Then type in `%appdata%` and hit enter. Open the folder called `.minecraft`.
    - Mac: On the bar at the top of your screen in Finder, click `Go`, then click `Go to Folder` and type `~/Library/Application Support/Minecraft`, then hit enter.
    - Linux: Open `~/.minecraft`.
2. In your Minecraft folder, open the folder called `mods`.
3. Place all of the mods you want to use into this folder. (Note that all mods you install must be for Fabric 1.17 or they will not work.)

## Mods (waiting on many mods to update, no links yet)

_Essential_

These are essential mods that are pretty much required for every Fabric installation.

| Mod | Description | Dependencies | Author |
| --- | --- | ---| ---|
| [Fabric API](https://modrinth.com/mod/fabric-api) | Required for most Fabric mods | N/A | [Fabric Team](https://fabricmc.net/) |
| [Mod Menu](https://modrinth.com/mod/modmenu) | Allows the user to see all installed mods, as well as access the config for most | N/A | [Prospector](https://modrinth.com/user/Dc7EYhxG) |

_Performance_
| Mod | Description | Dependencies | Author |
| --- | --- | ---| ---|
| [Sodium](https://modrinth.com/mod/sodium) | no 1.17 yet | N/A | [Caffeine](https://github.com/CaffeineMC/) |
| [Hydrogen](https://modrinth.com/mod/hydrogen) | no 1.17 yet | N/A | [Caffeine](https://github.com/CaffeineMC/) |
| [Lithium](https://modrinth.com/mod/lithium) | desc | N/A | [Caffeine](https://github.com/CaffeineMC/) |
| [Starlight](https://github.com/Spottedleaf/Starlight) | desc | N/A | [SpottedLeaf](https://github.com/Spottedleaf) |
| [LazyDFU](https://modrinth.com/mod/lazydfu) | desc | dont think so | [astei](https://modrinth.com/user/y0WF9UR5) |
| [Enhanced Block Entities](https://modrinth.com/mod/ebe) | no 1.17 yet, not gonna add betterbeds since ebe should replace that soon | [Indium](https://github.com/comp500/Indium) | [FoundationGames](https://modrinth.com/user/WH9NfS5R) |
| [FerriteCore](https://www.curseforge.com/minecraft/mc-mods/ferritecore-fabric) | no 1.17 yet | N/A | [malte0811](https://github.com/malte0811) |
| [Entity Culling](https://www.curseforge.com/minecraft/mc-mods/entityculling) | desc | N/A | [tr9zw](https://github.com/tr7zw)
| [Dynamic FPS](https://modrinth.com/mod/dynamic-fps) | no 1.17 yet | N/A | [juliand665](https://modrinth.com/user/HLI9Dbyv) |

_OptiFine Replacements_
- ok zoomer (no 1.17 yet)
- lambdynlights https://modrinth.com/mod/lambdynamiclights
- lambdbettergrass (has better snow too) https://modrinth.com/mod/lambdabettergrass
- iris https://irisshaders.github.io/
- fabricskyboxes https://modrinth.com/mod/fabricskyboxes/
- fabrishot https://modrinth.com/mod/fabrishot
- fabric ctm
- chime (cit)
- cull leaves https://modrinth.com/mod/cull-leaves
- colormatic
- transparent
- soaring clouds
- splash

other
- item model fix https://github.com/PepperCode1/Item-Model-Fix/releases/tag/v1.0.2+1.17
- borderless mining
- not enough crashes (no 1.17 yet)
- cleanview (no 1.17 yet)
- smooth scrolling everywhere (no 1.17 yet)
- no potion offset (no 1.17 yet)
- controlling (no 1.17 yet)
- no view bobbing screen (no 1.17 yet)
- kronhud (probably not gonna get a 1.17 but lets see)

## Credits

- [Zordlan](https://github.com/Zordlan)
- [NoPro2024](https://github.com/NoPro2024)

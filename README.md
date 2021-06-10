# Switching to 1.17

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

## Mods (this isnt how it will look, will add cool markdown boxes and shit)

essential
- fabric api
- mod menu
- fabric language kotlin?

performance
- sodium
  - indium
- lithium
- starlight (has 1.17) / phosphor (no 1.17 yet)
- lazydfu
- ebe (no 1.17 yet)
- ferritecore (no 1.17 yet)
- entity culling
- hydrogen (no 1.17 yet)
- dynamicfps (has 21w18a but no 1.17 specific yet)

optifine features
- ok zoomer (no 1.17 yet)
- lambdynlights
- lambdbettergrass (has better snow too)
- iris
- fabricskyboxes

(not sure if any of these remaining have 1.17 yet)
- fabric ctm
- chime (cit)
- cull leaves
- colormatic
- transparent
- soaring clouds
- splash
- fabrishot

other
- item model fix
- borderless mining
- not enough crashes (no 1.17 yet)
- cleanview (no 1.17 yet)
- smooth scrolling everywhere (no 1.17 yet)
- no potion offset (no 1.17 yet)
- controlling (no 1.17 yet)
- no view bobbing screen (no 1.17 yet)

# Note

If you would like to contribute, please make a PR (and please add your name to credits, even if you didn't do much).

## Credits

- [Zordlan](https://github.com/Zordlan)
- [NoPro2024](https://github.com/NoPro2024)

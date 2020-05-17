# Anubis [![C](https://img.shields.io/badge/language-C-%23f34b7d.svg)](https://en.wikipedia.org/wiki/C) [![CS:GO](https://img.shields.io/badge/game-CS%3AGO-yellow.svg)](https://store.steampowered.com/app/730/CounterStrike_Global_Offensive/) [![Windows](https://img.shields.io/badge/platform-Windows-0078d7.svg)](https://en.wikipedia.org/wiki/Microsoft_Windows) [![x86](https://img.shields.io/badge/arch-x86-red.svg)](https://en.wikipedia.org/wiki/X86) [![License](https://img.shields.io/github/license/danielkrupinski/Anubis.svg)](LICENSE)

Free open-source training software / cheat for **Counter-Strike: Global Offensive** game. Designed as internal cheat - [Dynamic-link library](https://en.wikipedia.org/wiki/Dynamic-link_library) (DLL) loadable into game process. Compatible with the latest version of the game on Steam.

## Features

* **Glow** - render glow effect on entities
* **Misc** - miscellaneous features
* **Config** - JSON-based configuration system

<details>
<summary>Features in depth</summary>

* **Glow** - render glow effect on entities

    *Allies, Enemies, Planting (player planting bomb), Defusing (player defusing bomb), Local player, Weapons (dropped weapons), C4, Planted C4, Chickens* **/** *All, Visible, Occluded*

    * **Enabled** - on / off master switch
    * **Health based** - color is based on player's hp
    * **Rainbow** - change color frequently
    * **Thickness** - outline thickness
    * **Alpha** - outline alpha
    * **Style** - glow style [*0*-*3*]

* **Misc** - miscellaneous features
    * **Auto strafe** - automatically strafe in air following mouse movement
    * **Bunny hop** - automatically simulate space bar press / release while jump button is being held; increases movement speed
    * **Moonwalk** - break walking animation

* **Config** - JSON-based configuration system
    * **Create config** - create new configuration file
    * **Reset config** - restore default configuration settings (does not touch saved configuration)
    * **Load selected** - load selected configuration file
    * **Save selected** - save selected configuration file
    * **Delete selected** - delete selected configuration file
</details>

## Getting started

### Prerequisites
Microsoft Visual Studio 2019 (preferably latest version i.e. 16.0.3), platform toolset v142 and Windows SDK 10.0 are required in order to compile Anubis. If you don't have ones, you can download VS [here](https://visualstudio.microsoft.com/) (Windows SDK is installed during Visual Studio Setup).

### Cloning
The very first step in order to compile Anubis is to clone this repo from GitHub to your local computer. Git is required to step futher, if not installed download it [here](https://git-scm.com). Open git bash / git cmd / cmd and enter following command:
```
git clone https://github.com/5R33CH4/Anubis.git
```
`Anubis` folder should have been succesfully created, containing all the source files.

### Compiling from source

If everything went right you should receive `Anubis.dll`  binary file.

### Loading / Injecting into game process

Open your favorite [DLL injector](https://en.wikipedia.org/wiki/DLL_injection) and just inject `Anubis.dll` into `csgo.exe` process.

When injected, menu is openable under `INSERT` key.

Ultimate All-in-One Injector Compilation can be found @ https://github.com/5R33CH4/Ultimate-Injector-Compilation.


﻿## How to install

Download the latest release from https://github.com/mindphluxnet/TaleOfToastPlugin/releases and unpack it to your Tale of Toast directory.

## How to build from source (Windows)

```
git clone https://github.com/mindphluxnet/TaleOfToastPlugin
```

Create a folder called "Libs" in the cloned directory, then copy the following files into it:

From ToT_Data\Managed:

- Assembly-CSharp.dll
- Facepunch.Steamworks.dll
- InControl.dll
- Nethereum.*.dll
- uLink.dll
- UnityEngine.dll
- UnityEngine.CoreModule.dll
- UnityEngine.UI.dll

From Libs-Shipping:

- MMHOOK_Assembly-CSharp.dll

Download https://github.com/BepInEx/BepInEx/releases/tag/v5.4.11 unpack and copy the following files to the Libs folder:

- BepInEx.dll
- BepInEx.Harmony.dll
- MonoMod.RuntimeDetour.dll
- MonoMod.Utils.dll

Then open TalesOfToastPlugin.sln using Visual Studio and press F6 to build.
 
 ## Bug Fixes

* Re-implements broken Discord Presence implementation
* Adds missing Alt+Click to crafting recipe item preview
* Fixes broken Back button on Mailbox Compose view
* Fixes item 3675 ("Dusty Tome") having no icon because the assigned item atlas doesn't exist (neither does the assigned icon)
* Fixes item 2488 ("Cooked Enriched Delicious Meat") having no icon because the icon assigned doesn't exist
* Fixes items 3047 and 3048 (Mana Potion III and IV) to have matching icons instead of looking like Health Potions
* Enemy name plates are now positioned relative to the enemy model's height to prevent them from clipping into larger enemies

## Quality of Life Features

* Adds a free bag space display next to the button menu. Press F3 to toggle it on/off
* Adds the ability to use the Enter/Return key to log in and enter the world
* Stores and automatically resummons the last summoned pet after logging in or taking a flight path
* Stores and automatically restores the pinned trade skill, also adding the skill level to the display
* Removes the ability to right-click the player avatar to prevent combat targeting issues
* Adds the ability to change the threshold for displaying ?? as level to an user defined value instead of 6 (defaults to 10)
* Scales the minimap icons down by about 30% on the highest zoom setting
* Removes the 10 second timer after moving before the player can log out
* Action bars can now be locked/unlocked by pressing F2, saving the player the hassle to go through the options menu
* Incoming friend requests are now announced via chat message
* Trying to buy Crumbs when the game was not started via Steam (or the Steam Overlay is not ready) now shows an error message.
* Removes the "HPB death cloud" effect on loot/kill
* Crafting recipe tooltips now also show the resulting item
* All potions now have their effect listed on the tooltip
* You can now toggle the fullscreen sharpening effect with F4 while in-game
* A combat log is now written to the Logs sub directory of the game directory. This can be disabled in the configuration file.

## Work in Progress

* Campfire items now have their effects listed on the tooltip. Mostly working fine already, just not for every campfire item.

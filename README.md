# Initial
Whilst everything in this config is green lighted and allowed to be used as of 27/05/2023 if anything does happen to your account due to the use of this config, that is not my responsibility.

# Install

Go into `APB Reloaded\Binaries` and right click APB.exe (`APB if you don't have File Extensions shown`) and create a shortcut placing it wherever you desire, then right click the newly created APB shortcut and go to properties, from there at the end of the `Target` field add whichever launch arguments you require from below.

All of the folders are laid out in such a way that you can just open them up until you see one of the folders matching those that are within APB by default to be able to just `Drag & Drop` them in. For example, when you get to a folder with the name `APBGame` you can just drag that into `APB Reloaded` and it should ask you to overwrite existing files. If you do not get a prompt to overwrite files then you have not copied the folder correctly and will likely have to repair the game using the launcher.

When the game updates you will have to reapply most of the config as the launcher overwrites modifications to most of the files, if something major changes it's recommended to also run the `Repair` option within the launcher to ensure all files are up to date, if there are files that change that are within the config I will be sure to update them as soon as possible.

# Launch Arguments

- `-language=1031`                  - Sets game to load with custom localization
- `-nosteam`                        - Disables Steam integration so you will have to manually login
- `-nomovies` / `-nomoviesstartup`  - Removes loading screens
- `-nosplash`                       - Removes initial splash screen upon boot

Target Field Example
`"G:\APB Reloaded\Binaries\APB.exe" -language=1031 -nomovies -nosplash`

# FPS Boost
- Engine Tweaks (Unstream On + Diskcache Off + Streaming Off) - This disables disk cache so if your system has a low amount of RAM (Below 16GB) this is not recommended.
- Disables the games ability to smoothly transition between LOD states as it can cause slowdown
- Gained FPS varies per system
- With this on if you swap between graphics presets whilst ingame you will have to swap district in order for them to apply, the exception being if you swap to low poly character models

# Command Changes (If using localization)

- /exit -> /rq
- /abandonmission -> /a
- /dance variants without the word dance -> /urban /michael /techno etc.
- /groupinvitemodedefault -> /gimd (When not in a group type, "/gimd true" to allow all members of group to be able to invite everytime)

# Graphics
### High Graphics Options

- MINIMAL		- High Env, High Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off, Fog Off
- LOW 		- High Env, HQ Low Poly Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Cirlces Off, Fog Off
- MEDIUM 		- High Env, High Character, High Car, High Weapon, High Prop, High VFX, Obj Cirlces Off, Fog Off
- HIGH 		- High Env, HQ Low Poly Character, High Car, High Weapon, High Prop, High VFX, Obj Cirlces Off, Fog Off
- MAXIMUM 	- High Env, High Character, High Car, High Weapon, High Prop, High VFX, Obj Cirlces On, Fog Off

### Low Graphics Options

- MINIMAL		- Low Env, High Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off, Fog Off
- LOW 		- Low Env, HQ Low Poly Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off, Fog Off
- MEDIUM 		- Low Env, High Character, Clay Car, Low Weapon, Mid Prop, Low VFX, Obj Circles Off, Fog Off
- HIGH 		- Low Env, HQ Low Poly Character, Clay Car, Low Weapon, Mid Prop, Low VFX, Obj Circles Off, Fog Off
- MAXIMUM 	- Low Env, LQ Low Poly Character, Clay Car, Low Weapon, Low Prop, Low VFX, Obj Circles Off, Fog Off

# Keybinds
All of the binds listed below are there as additions to the original keybinds so you have the choice rather than being forced to use one or the other. This just means that you will have to go to the respective keybind category and set which options you prefer.

By default your game will be using the binds you had previously or if you're on a fresh account some binds will now be completely blank, simply go into Options > Controls and set them manually.

*Category listed at beginning*

   - Interface | Abandon Mission - Lets you abandon an unopposed mission by pressing a key
   - Interface | Social Designers - This will only work in social but lets you bind a key to open the Clothing, Character, Vehicle, Symbol and Theme studios
   - Movement  | Always Sprint - Works exactly the same as the old Always sprint, just bind it, press it once when entering a district and you will always be running
   - Movement  | Crouch (Hold) - The same as previous hold to crouch except now ingame!
   - Combat    | Lean (Hold) - Hold down the lean key rather than have it toggle
   - Combat    | Primary/Secondary weapon - Allows you to set keys to select which weapon you want rather than cycle between them which is the default behaviour
   - Music     | Music Player Volume - Controls the volume of the music player in steps of 20
   - Camera    | Camera look up/down - Extremely fast but there if you really need it

*The default Xbox input should disabled with this file or at least partly so most functionality from a controller should no longer work with this.*

# Disabling UI Elements
As this is something that can be quite customised I'm not going to create presets for it however a quick rundown for how to do it can be found here: [Inteface](https://github.com/lvzxr/apb-reloaded/blob/main/UI.md)

## Features

- Engine Tweaks - This sets the fps limit to 0, if you would like to make it your monitors refresh rate open this file and change MaxClientFramerate. Also sets smooth framerate to 128.
- FPS Boost - All information above.
- Keybinds - All information above.
- Remove Vivox - Blanks the Vivox.exe file causing it to not load, fixes Steam sometimes getting stuck on APB due to Vivox not closing. If you get EAC issues using this just repair and leave the file stock.

## Interface

- Faster UI - Changes what file the UI is read from causing there to be parking signs throughout the inventory, can help to improve fps when changing mods quickly. Jeshua is more broken than Adam but also includes the white mission timer.
- Localization - My custom take on APB's localization a lot of stuff has been shortened and or removed.

## Visual

- No Login Screen - Sets login screen to a black scene, still allows character creation.
- No Ragdolls - Removes player/pedestrian ragdolls.
- Graphics - Preset settings listed above. Shadows should work on all presets, if you want them just enable it under advanced after selecting the preset you like, if it doesn't work go into APBMachineOptions and remove the DynamicShadows and LightEnvironmentShadows lines, save, restart the game then re-enable shadows again. When switching between clay vehicles and standard your game may crash therefore I recommend you do this on the login screen. I recommend trying to use double buffering if you do not feel input lag with it on, as it is essentially free FPS.
- Emitter Fix - Set's priorties of emitters and npcs to 1 so they are only played when really close to you, this also have the effect of making them quieter, included as different variants with ragdolls and muzzle flash.

## Audio

- Remove Ambient Sounds - Removes a large majority of ambient sounds.
- Remove Dialogue - Removes all speech and screams from your character and other npcs.
- Vehicle Amp Levels - Sets vehicle amp levels to a very low value so you shouldn't hear music out of cars, doesn't affect open world music points (including boom boxes) / when someone is playing music created in the studio out of a car you are sat in.

# Credits

- Flaws - Older Keybinds, File Structure, No Ragdolls
- rooq - Mission Stages
- Esurient - Engine Tweaks
- Leefekyn - Alt Mission Titles
- mewpri - Studio Keybinds
- Kyouki - Amibient Sound Removal
- ApollyoNite - RTW Vegas
- jmilos - Texture Streaming, Extra Keybinds

# [Changelog](https://github.com/lvzxr/apb-reloaded/blob/main/Changelog.md) 

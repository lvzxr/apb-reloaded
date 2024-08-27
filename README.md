# Initial
Whilst everything in this config is green lighted and allowed to be used as of 26/08/2024 if anything does happen to your account due to the use of this config, that is not my responsibility.

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

# GC On + Streaming Off  (Do not mix with 'GC Off Stutter Fix')
- All of the social kiosks e.g clothing, vehicle and character work fine with these files
- Disables the texture streaming system forcing whichever graphics you start with to be the maximum you'll see without restarting
- Gained FPS varies per system

# GC Off Stutter Fix (Do not mix with 'GC On + Streaming Off')
- Some of the social kiosks e.g clothing, vehicle and character will not load with these files
- These files completely disable the garbage collection system so is absolutely not recommended for systems with ~8GB RAM free at idle state
- This includes Streaming off as there is no downside to using it and will provide free fps the the large majority of systems
- Gained FPS varies per system
- You may experience large stutters on the respawn screen after a long time of being alive due to this now being when the garbage dump will happen

# Misc Changes

- **If you wish to have a semi-transparent inventory screen once you've applied the config, go to `Engine/Config/BaseEngine.ini`, put a `;` before `DefaultPostProcessName=APBPostEffectMaterials.APBPostEffect_Process` and turn on bloom ingame**
- If you are using the GC Off files and want to go and modify your outfits then go to `Engine/Config/BaseEngine.ini`, set TimeBetweenPurgingPendingKillObjects -> 60, restart the game and then once you're done designing set this back to 0 and restart your game again to continue having no stuttering during fights
- If you aren't already using them I recommend using the Emitters fix as it stops props such as AC Units, Gas Station Pumps and Car Spawners from emitting an ear piercing sound when standing near them after playing for a longer period of time

# Command Changes (If using localization)

- /exit -> /rq
- /dance variants -> /urban /michael /techno etc.
- /strikeapose1/2 -> /pose1 /pose2
- /groupinvitemodedefault -> /gimd (When not in a group type, "/gimd true" to allow all members of group to be able to invite everytime)

# Graphics
### Mixed

- MINIMAL	- High Env, High Character, High Car, High Weapon, Mid Prop, Mid VFX, Obj Circles Off, Fog Off
- LOW 		- High Env, HQ Low Poly Character, High Car, High Weapon, Mid Prop, Mid VFX, Obj Circles Off, Fog Off
- MEDIUM 	- Mid Env, High Character, High Car, High Weapon, Mid Prop, Mid VFX, Obj Circles Off, Fog Off
- HIGH 		- Mid Env, HQ Low Poly Character, High Car, High Weapon, Mid Prop, Mid VFX, Obj Circles Off, Fog Off
- MAXIMUM 	- High Env, High Character, High Car, High Weapon, High Prop, High VFX, Obj Circles Off, Fog Off

### High

- MINIMAL	- High Env, High Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off, Fog Off
- LOW 		- High Env, HQ Low Poly Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off, Fog Off
- MEDIUM 	- High Env, High Character, High Car, High Weapon, High Prop, High VFX, Obj Circles Off, Fog Off
- HIGH 		- High Env, HQ Low Poly Character, High Car, High Weapon, High Prop, High VFX, Obj Circles Off, Fog Off
- MAXIMUM 	- High Env, High Character, High Car, High Weapon, High Prop, High VFX, Obj Circles On, Fog Off

### Mid

- MINIMAL	- Mid Env, High Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off, Fog Off
- LOW 		- Mid Env, HQ Low Poly Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off, Fog Off
- MEDIUM 	- Mid Env, High Character, High Car, High Weapon, High Prop, High VFX, Obj Circles On, Fog Off
- HIGH 		- Mid Env, HQ Low Poly Character, High Car, High Weapon, High Prop, High VFX, Obj Circles On, Fog Off
- MAXIMUM 	- Mid Env, High Character, High Car, High Weapon, High Prop, High VFX, Obj Circles On, Fog Off

### Low

- MINIMAL	- Low Env, High Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off, Fog Off
- LOW 		- Low Env, HQ Low Poly Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off, Fog Off
- MEDIUM 	- Low Env, High Character, Clay Car, Low Weapon, Low Prop, Low VFX, Obj Circles Off, Fog Off
- HIGH 		- Low Env, HQ Low Poly Character, Clay Car, Low Weapon, Low Prop, Low VFX, Obj Circles Off, Fog Off
- MAXIMUM 	- Low Env, LQ Low Poly Character, Clay Car, Low Weapon, Low Prop, Low VFX, Obj Circles Off, Fog Off

# Keybinds
All of the binds listed below are there as additions to the original keybinds so you have the choice rather than being forced to use one or the other. This just means that you will have to go to the respective keybind category and set which options you prefer.

By default your game will be using the binds you had previously or if you're on a fresh account some binds will now be completely blank, simply go into Options > Controls and set them manually.

*Category listed at beginning*

   - Interface | Social Designers - This will only work in social but lets you bind a key to open the Clothing, Character, Vehicle, Symbol and Theme studios
   - Movement  | Always Sprint - Works exactly the same as the old Always sprint, just bind it, press it once spawned into a district and you will always be running
   - Movement  | Crouch (Old Hold) - The same hold to crouch we've had for years that can get stuck with jump + crouch/sprint + crouch
   - Movement  | Crouch (New Hold) - Alternative method for hold to crouch that doesn't get stuck as it implements a jump before crouching
   - Driving   | Vehicle Special Function (Hold) - This allows you to hold the siren on rather than have it toggle, if it gets stuck hold the button whilst getting out of the car to reset it 
   - Combat    | Lean (Hold) - Hold down the lean key rather than have it toggle
   - Combat    | Primary/Secondary weapon - Allows you to set keys to select which weapon you want rather than cycle between them which is the default behaviour
   - Music     | Music Player Volume - Controls the volume of the music player in steps of 20
   - Camera    | Camera look up/down - Extremely fast but there if you really need it

*The default Xbox input should disabled with this file or at least partly so most functionality from a controller should no longer work with this.*
*If you experience issues such as keybinds being reset, be sure to use any version after v2.8, this should only affect those using a French keyboard layout*

# Disabling UI Elements
As this is something that can be quite customised I'm not going to create presets for it however a quick rundown for how to do it can be found here: [Interface](https://github.com/lvzxr/apb-reloaded/blob/main/UI.md)

## Features

- GC On + Streaming Off  - All information above.
- GC Off Stutter Fix - All information above.
- Keybinds - All information above.

## Interface

- Faster UI - Changes what file the UI is read from causing there to be parking signs throughout the inventory, can help to improve fps when changing mods quickly. Jeshua includes a white mission timer however completely breaks the UI in editors so a lot of text will be missing.
- Localization - My custom take on APB's localization a lot of stuff has been shortened and or removed.

## Visual

- No Ragdolls - Removes player/pedestrian ragdolls.
- Graphics - Preset settings listed above. Shadows should work on all presets, if you want them just enable it under advanced after selecting the preset you like, if it doesn't work go into APBMachineOptions and remove the DynamicShadows and LightEnvironmentShadows lines, save, restart the game then re-enable shadows again. When switching between clay vehicles and standard your game may crash therefore I recommend you do this on the login screen.
- Emitter Fix - Set's priorties of emitters and npcs to 1 so they are only played when really close to you, this also have the effect of making them quieter, included as different variants with ragdolls and muzzle flash.

## Audio

- Vehicle Amp Levels - Sets vehicle amp levels to a very low value so you shouldn't hear music out of cars, doesn't affect open world music points (including boom boxes) / when someone is playing music created in the studio out of a car you are sat in.
- Remove Default Music - Removes the default music that comes with the game (previously a part of Vehicle Amp Levels)

# Remove / Uninstall

If you wish to uninstall the config it is recommended that you run the `Repair` within the APB Launcher to get back to stock. Other than that all you should need to do is **Delete DefaultCompat.ini** from `APBGame\Config` and **Delete GER** from `APBGame\Localization`. Once both of those are deleted and the launcher has repaired, the config should be completely removed.

# Credits

- Flaws - No Ragdolls
- rooq - Mission Descriptions
- Esurient - Engine Related Changes
- Leefekyn - Alt Mission Titles
- mewpri - Studio Keybinds
- Kyouki - Ambient Sound Removal, GC Related Stuff
- ApollyoNite - RTW Vegas / Bishada
- jmilos - Combat / Vehicle Keybinds
- vestice - Fixing bad grammer :-)

# [Flaws APB Config](https://github.com/flawsv/apb)
# [xaizone APB Config](https://github.com/xaizone/apb-reloaded)

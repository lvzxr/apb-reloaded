# Initial
Everything within this config is typically kept up to date with what LO will allow/disallow when it comes to modifying files so when I provide an update it's always recommended to download it and ensure you're up to date, older versions whilst still available shouldn't be used unless you know what you want out of them is allowed.

> [!IMPORTANT]
> Whilst everything within the latest version of the config will be safe to use and what LO allows if anything were to happen to your account due to use of modifed game files that is not my responsibility.

# Install

Go into `APB Reloaded\Binaries` and right click APB.exe (`APB if you don't have File Extensions shown`) and create a shortcut placing it wherever you desire, then right click the newly created APB shortcut and go to properties, from there at the end of the `Target` field add whichever launch arguments you require from below.

Everything is laid out in such a way to where you can just `Drag & Drop` the config into the game without you having to go fishing through folders. So if you see `APBGame` or `Engine` that is all you will need to copy into your game.
> [!CAUTION]
> If you do not get the prompt for replacing files then you haven't correctly installed the config and will likely have to repair the game using the Launcher.

>[!NOTE]
> When the game updates you will have to reapply most of the config as the launcher overwrites modifications to most of the files, if something major changes it's recommended to also run the `Repair` option within the launcher to ensure all files are up to date, if there are files that change that are within the config I will be sure to update them as soon as possible.

> [!IMPORTANT]
> Due to the new way the login screen removal works if you want to make a new character then you will need to make sure that `TimeBetweenPurgingPendingKillObjects=60` within `BaseEngine.ini` alongside having both the `Map` and `LocalMap` values located within `DefaultEngine.ini` to be set to `APBLoginLevel.apb` instead of the configs `UIDistrict_DistrictSelect.apb`. You can set this back afterwards but until there is a more fleshed out way to remove the login screen you will have to do this or run no config when making a new character.

# Launch Arguments

- `-language=1031`                  - Sets game to load with custom localization
- `-nosteam`                        - Disables Steam integration so you'll have no overlay and no Steam login
- `-nomovies` / `-nomoviesstartup`  - Removes loading screens
- `-nosplash`                       - Removes initial splash screen upon boot

Target Field Example
`"G:\APB Reloaded\Binaries\APB.exe" -language=1031 -nomovies -nosplash`

# GC On + Streaming Off
- All of the social kiosks e.g clothing, vehicle, character, theme and symbol work fine with these files
- Disables the texture streaming system forcing whichever graphics you start with to be the maximum you'll see without restarting (on most objects)
- Gained FPS varies per system
- If you want an easy way of re-enabling the kiosks you can drag these files in to overwrite the stutter fix, just remember to put stutter fix back in afterwards

# GC Off Stutter Fix
- Some of the social kiosks e.g clothing, vehicle and character will not load with these files, the remaining studios, theme and symbol do work however 
- Disables the texture streaming system forcing whichever graphics you start with to be the maximum you'll see without restarting (on most objects)
- Gained FPS varies per system
- You may experience large stutters on the respawn screen after a long time of being alive due to this now being when the garbage dump will happen

> [!IMPORTANT]
> If you find yourself frozen on the repsawn screen for an extended period of time and either your team or the enemy progresses to the next stage of a mission you will not be able to see the new objective(s) when you respawn, this is a bug and there is no way around it without re-enabling garbage collection. 

# Misc
> [!NOTE]
> If you wish to have a semi-transparent inventory screen once you've applied the config, go to `Engine/Config/BaseEngine.ini`, put a `;` before `DefaultPostProcessName=APBPostEffectMaterials.APBPostEffect_Process` and turn on bloom ingame

> [!IMPORTANT]
> If you are using the GC Off files and want to go and modify your outfits then go to `Engine/Config/BaseEngine.ini`, set TimeBetweenPurgingPendingKillObjects -> 60, restart the game and then once you're done designing set this back to 0 and restart your game again to continue having no stuttering during fights

> [!NOTE]
> If you aren't already using them I recommend using the Emitters fix as it stops props such as AC Units, Gas Station Pumps and Car Spawners from emitting an ear piercing sound when standing near them after playing for a longer period of time

# Command Changes (If using localization)

- /exit -> /rq
- /dance variants -> /urban /michael /techno etc.
- /strikeapose1/2 -> /pose1 /pose2
- /groupinvitemodedefault -> /gimd (When not in a group type, "/gimd true" to allow all members of group to be able to invite everytime)

# Graphics
> [!NOTE]
> Shadows should work on all presets, if you want them just enable it under advanced after selecting the preset you like. If it doesn't work however go into `APBMachineOptions` and remove the `DynamicShadows` and `LightEnvironmentShadows` lines, save, restart the game then re-enable shadows again.

> [!IMPORTANT]
> When switching between clay vehicles and standard your game may crash therefore I recommend you do this on the login screen.

### Mixed (Recommended for most people)

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

> [!IMPORTANT]
> By default your game will be using the binds you had previously or if you're on a fresh account some binds will now be completely blank, simply go into Options > Controls and set them manually.

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

*Default Xbox controller related keybinds are removed with this file*

# Disabling UI Elements
As this is something that can be quite customised I'm not going to create presets for it however a quick rundown for how to do it can be found here: [Interface](https://github.com/lvzxr/apb-reloaded/blob/main/UI.md)

## Features

- GC On + Streaming Off  - All information above.
- GC Off Stutter Fix - All information above.
- Keybinds - All information above.

## Interface

- Localization - My custom take on APB's localization. A lot of the localization has been rewritten and made to, for most presets NOT appear in ORANGE :triumph:

## Visual

- No Ragdolls - Removes player/pedestrian ragdolls.
- Graphics - Preset settings listed above.
- Emitter Fix - Set's priorties of emitters and npcs to 1 so they are only played when really close to you, this also have the effect of making them quieter, included as different variants with ragdolls and muzzle flash.

## Audio

- Vehicle Amp Levels - Sets vehicle amp levels to a very low value so you shouldn't hear music out of cars, doesn't affect open world music points (including boom boxes) / when someone is playing music created in the studio out of a car you are sat in.
- Remove Default Music - Removes the default music that comes with the game (previously a part of Vehicle Amp Levels).

# Remove / Uninstall

> [!IMPORTANT]
> If you wish to uninstall the config it is recommended that you run the `Repair` within the APB Launcher to get back to stock. Other than that all you should need to do is **Delete DefaultCompat.ini** from `APBGame\Config` and **Delete GER** from `APBGame\Localization`. Once both of those are deleted and the launcher has repaired, the config should be completely removed.

# Credits

- Flaws :clown_face: - No ragdolls
- rooq :skull: - Mission descriptions
- Esurient :robot: - Engine related changes
- Leefekyn :sunglasses: - Alt mission titles
- mewpri :alien: - Studio keybinds
- Kyouki :nerd_face: - Garbage collection settings
- ApollyoNite :smiley: - RTW Vegas / Bishada (No longer included)
- jmilos :japanese_goblin: - Combat / Vehicle keybinds
- myamai :space_invader: - Creating localization resources

# [Flaws APB Config](https://github.com/flawsv/apb)
# [xaizone APB Config](https://github.com/xaizone/apb-reloaded)
# [myamai APB Localization Resources](https://myamai.neocities.org/apb/localization)

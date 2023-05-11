# Initial

Create a shortcut of APB.exe from the binaries folder and use whichever launch arguments apply to how you install the config.
If the game were to update be sure to reinstall everything as they will most likely have been overwritten, the outlier for that being localization as no German translation of the game exists currently.

For ease of installing the entire config, I recommend making a folder either here or in the game directory and just copy paste all the different tweaks you use so it will just be an easy copy paste of everything all at once whenever you update your game.

# DISABLE MUZZLE FLASH
- It should go without saying but if you use no ragdolls or the temp emitters fix do this after those files are in your game.
- To do this go to APBGame/Config then open DefaultGame.ini, scroll to the bottom and there you can set "m_bEnableMuzzleFlash=true" to "m_bEnableMuzzleFlash=false" along with "m_bEnableMagazineCasings=true" to "m_bEnableMagazineCasings=false" if you wish. 

# Launch Arguments

- -language=1031 - Sets game to load with custom localization
- -nosteam       - Disables Steam integration so you will have to manually login
- -nomovies      - Removes loading screens, if this for whatever reason doesn't work try -nomoviesstartup
- -nosplash      - Removes initial splash screen upon boot

# Command Changes (If using localization)

- /exit -> /rq
- /abandonmission -> /a
- /dance variants without the word dance -> /urban /michael /techno etc.
- /groupinvitemodedefault -> /gimd (When not in a group type, "/gimd true" to allow all members of group to be able to invite everytime)

# Graphics
### High Graphics Options - FOG OFF BY DEFAULT

- MINIMAL		- High Env, High Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off
- LOW 		- High Env, HQ Low Poly Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Cirlces Off
- MEDIUM 		- High Env, High Character, High Car, High Weapon, High Prop, High VFX, Obj Cirlces Off
- HIGH 		- High Env, HQ Low Poly Character, High Car, High Weapon, High Prop, High VFX, Obj Cirlces Off
- MAXIMUM 	- High Env, High Character, High Car, High Weapon, High Prop, High VFX, Obj Cirlces On

### Low Graphics Options - FOG OFF BY DEFAULT

- MINIMAL		- Low Env, High Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off
- LOW 		- Low Env, HQ Low Poly Character, High Car, High Weapon, Mid Prop, Low VFX, Obj Circles Off
- MEDIUM 		- Low Env, High Character, Clay Car, Low Weapon, Mid Prop, Low VFX, Obj Circles Off
- HIGH 		- Low Env, HQ Low Poly Character, Clay Car, Low Weapon, Mid Prop, Low VFX, Obj Circles Off
- MAXIMUM 	- Low Env, LQ Low Poly Character, Clay Car, Low Weapon, Low Prop, Low VFX, Obj Circles Off


# Features

- Auto Sprint / Hold Crouch - Always sprint without holding shift, just hit it once upon entering a district and spawning. Hold the crouch key rather than having it toggle.

- Engine Tweaks - This sets the fps limit to 0, if you would like to make it your monitors refresh rate open this file and change MaxClientFramerate. Also sets smooth framerate to 128.

- Engine Tweaks (Unstream On + Diskcache Off) - This does everything the same as the other file whilst also disabling texture streaming. This also disables disk cache so if your system has a low amount of RAM e.g 8GB total this is not recommended. **USE STREAMING OFF GRAPHICS FILES WITH THIS OPTION**

- Faster UI - Changes what file the UI is to read from causing there to be parking signs throughout the inventory, can help to improve fps when changing mods quickly. Jeshua is more broken than Adam.

- Graphics - Preset settings listed above. Shadows should work on all presets, if you want them just enable it under advanced after selecting the preset you like, if it doesn't work go into APBMachineOptions and remove the DynamicShadows and LightEnvironmentShadows lines, save, restart the game then re-enable shadows again. When switching between clay vehicles and standard your game may crash therefore I recommend you do this on the login screen. I recommend trying to use double buffering if you do not feel input lag with it on as it is essentially free FPS. **DON'T USE ADVANCED LAUNCHER ON MY PRESETS AND SAVE YOUR OWN SETTINGS, EVERYTHING OTHER THAN MINIMAL WILL BE MODIFIED**

- Graphics (Streaming Disabled) - Needed for "Engine Tweaks (Unstream On + Diskcache Off)

- No Login Screen - Sets login screen to a black scene, still allows character creation.

- No Notifications - Removes the district notification popups on the left of the screen for bounty, medals etc.

- No Ragdolls - Removes player/pedestrian ragdolls.

- Remove Vivox - Blanks the Vivox.exe file causing it to not load, fixes Steam sometimes getting stuck on APB due to Vivox not closing.

- Vehicle Amp Levels - Sets vehicle amp levels to a very low value so you shouldn't hear music out of cars, doesn't affect open world music points (including boom boxes) / when someone is playing music created in the studio out of a car you are sat in.

- TEMP EMITTERS FIX - SETS THE PRIORTY OF EMITTERS VERY LOW (WILL OVERWRITE NO RAGDOLLS, TO MANUALLY DO THIS WITH NO RAGDOLLS SCROLL TO THE BOTTOM OF THE FILE AND SET THE EMITTER / NPC PRIORITIES TO 1)

Anything that happens to your account due to using this config is not my responsibility. >=^w^=<

lazer :>

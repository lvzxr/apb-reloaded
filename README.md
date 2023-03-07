# Initial

Create a shortcut of APB.exe from the binaries folder and use whichever launch arguments apply to how you install the config.
If the game were to update be sure to reinstall everything as they will most likely have been overwritten, the outlier for that being localization as no German translation of the game exists currently.

For ease of installing the entire config, I recommend making a folder either here or in the game directory and just copy paste all the different tweaks you use so it will just be an easy copy paste of everything all at once whenever you update your game.

# Launch Arguments
- language=1031 - Sets game to load with custom localization
- nosteam       - Disables Steam integration so you will have to manually login
- nomovies      - Removes loading screens, if this for whatever reason doesn't work try -nomoviesstartup
- nosplash      - Removes initial splash screen upon boot

# Command Changes (If using localization)

- /exit -> /rq
- /abandonmission -> /a
- /dance variants without the word dance -> /urban /michael /techno etc.
- /groupinvitemodedefault -> /gimd (When not in a group type, "/gimd true" to allow all members of group to be able to invite everytime)

# Graphics Presets

- Minimal - High Characters, High Cars, Low Environment, Low Peds, High Props, High Weapons, Low VFX
- Low 	- Low Poly Characters, High Cars, Low Environment, Low Peds, Mid Props, Low Weapons, Low VFX
- Medium 	- High Characters, Clay Cars, Low Environment, Low Peds, Mid Props, Low Weapons, Low VFX
- High 	- High Characters, High Cars, High Environment, High Peds, High Props, High Weapons, Low VFX
- Max 	- High characters, High cars, High environment, High Peds, High Props, High Weapons, High VFX


# Features

- Auto Sprint / Hold Crouch - Always sprint without holding shift, just hit it once upon entering a district and spawning. Hold the crouch key rather than having it toggle.

- Engine Tweaks - Some values tweaked to help (maybe) improve fps. This also sets the fps limit to 0, if you would like to make it your monitors refresh rate open this file and set MaxClientFramerate to that.

- Engine Font - Removes a lot of the games stock Helvetica font depending on which variant you choose.

- Faster UI - Changes what file the UI is to read from causing there to be parking signs throughout the inventory, can help to improve fps when changing mods quickly. Jeshua is more broken than Adam.

- Graphics - Preset settings listed above. Shadows should work on all presets, if you want them just enable it under advanced after selecting the preset you like, if not go into APBMachineOptions and remove the DynamicShadows and LightEnvironmentShadows lines, save, restart the game then re-enable shadows again. When switching between clay vehicles and standard your game may crash therefore I recommend you do this on the login screen. !!DON'T USE ADVANCED LAUNCHER ON MY PRESETS AND SAVE YOUR OWN SETTINGS, EVERYTHING OTHER THAN MINIMAL WILL BE MODIFIED!!

- Localization - A variant of my localization that I use with a small variety of different colour presets. To have mission titles with equipment that Leefekyn made use "Alt Mission Titles". !!REQUIRES -language=1031 TO WORK!!

- No Bloom - Removes the pipline for the bloom within the game but still allows for the blurred background of the inventory screen, just enable bloom with the shader in game and you will be able to see what is going on around you whilst changing weapon.

- No Fog - Removes distance fog.

- No Login Screen - Sets login screen to a black scene, still allows character creation.

- No Notifications - Removes the district notification popups on the left of the screen for bounty, medals etc.

- No Ragdolls - Removes player/pedestrian ragdolls.

- Remove Vivox - Blanks the Vivox.exe file causing it to not load, fixes Steam sometimes getting stuck on APB due to Vivox not closing.

- Vehicle Amp Levels - Sets vehicle amp levels to a very low value so you shouldn't hear music out of cars, doesn't affect open world music points (including boom boxes) / when someone is playing music created in the studio out of a car you are sat in.


Anything that happens to your account due to using disallowed portions of this config is not my responsibility. USE AT YOUR OWN RISK =^w^=

lazer :>

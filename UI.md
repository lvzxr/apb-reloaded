#Located within APBGame/Config/DefaultEngine.ini

##All of the elements of the UI you wish to disable can be done by putting ; before any of these GlobalDataStores. Not all are listed here but that's due to either crashing your game or disabling a core part of the game.

- Crosshair
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Reticule"

- Weapon ammo top right, also disables Reload and Resupply text
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_WeaponInfo"

- Character list top left
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Group"

- Hitmarkers
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_HitIndicators"

- Health indication
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Health"

- Progress circle for objectives
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_CSAProgressBars"

- Radar
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Radar"

- Player modifications right
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Usables"

- Cash top right
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Cash"

- Bounty/Killstreak/Winstreak popup
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Ceremony"

- Kill/Assist/Arrest/Stun/Objective popup bottom of the screen
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_CombatMsgs"

- Player held items/Car stored items, also disables grenades
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Cargo"

- Clock bottom right
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Clock"

- Contact progression top left
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Contact"

- Notoriety/Prestige meter
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Heat"

- Tutorial, you will have no indication as to whether you are completing this on a new character
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Tutorial"

- Dirty money top left
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_OpenWorld"

- Fight Club challenges top left, crashes in baylan if you try to skip activity
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Challenges"

- Daily activities top left
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_DailyActivities"

- Minigame top middle, untested but will likely crash if disabled
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Minigame"

- Rank Icons/Money + Joker Ticket Icons/Weapon Icons (Killfeed)
+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_APBImages"
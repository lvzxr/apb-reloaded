# Located within APBGame/Config/DefaultEngine.ini

### All of the elements of the UI you wish to disable can be done by putting ; before any of these +GlobalDataStores
### Example of correctly disabling a UI element
 ;+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Clock"

### Examples of incorrectly disabling a UI element
 +;GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Clock"
 +GlobalDataStoreClasses=;"APBUserInterface.cUIDataStore_HUD_Clock"

### Crosshair
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Reticule"

### Weapon ammo top right, also disables Reload and Resupply text
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_WeaponInfo"

### Character list top left
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Group"

### Killfeed
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_ActionMessage"

### Radial hit circle (Tells you where you're being hit from)
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_HitIndicators"

### Health indication
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Health"

### Progress circle for objectives
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_CSAProgressBars"

### Radar
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Radar"

### Player modifications right
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Usables"

### Cash top right
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Cash"

### Bounty/Killstreak/Winstreak popup
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Ceremony"

### Kill/Assist/Arrest/Stun/Objective popup bottom of the screen
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_CombatMsgs"

### Player held items/Car stored items, also disables grenades
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Cargo"

### Clock bottom right
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Clock"

### Contact progression top left
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Contact"

### Notoriety/Prestige meter
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Heat"

### Tutorial
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Tutorial"

### Dirty money top left
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_OpenWorld"

### Fight Club challenges top left
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Challenges"

### Daily activities top left
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_DailyActivities"

### Minigame top middle
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Minigame"

### Rank Icons/Money + Joker Ticket Icons/Weapon Icons (Killfeed)
 +GlobalDataStoreClasses="APBUserInterface.cUIDataStore_APBImages"

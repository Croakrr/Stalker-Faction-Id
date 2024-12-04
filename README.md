# Pamplemousse's Stalker Faction Id

Simple mod to help identify the faction to whom a stalker belongs. Upon looking at or targeting a stalker in the world, a small icon representing their faction will appear in the left side of the screen. This is mostly for people who want to play without the crosshair reticule. Still a work in progress as it doesn't work on unique characters (traders, techs, story NPCs, etc.), but for now it should _at least_ help you identify if want to engage a group of stalker, or walk past them.  

# Disclaimer
This is very much an early early version for testing more than anything. I've barely played the game with this and there are scenarios where it's inaccurate. If you want to provide feedback, let me know which NPCs display an inaccurate icon.

**Known issues:** 
 - Spark faction is very hit and miss
 - Special / unique characters don't show an icon yet 
 - Zombies displays a faction icon most of the time
 - Some NPCs may display an innacurate faction (i.e. Duty dude showing up with a Freedom icon).

# Install

 - Extract into your ~mods folder. 
 - Launch the game; open up the console and enter the following command: 
	 - `mod add /Game/Mods/StalkerId/BP_StalkerIdentification.BP_StalkerIdentification_C`

### Optional - Help improve this mod!
There is a Debug mode you can use if you wish to help improve the accuracy of the identification.
To use it, enter the following commands in the console:
- `mod del /Game/Mods/StalkerId/BP_StalkerIdentification.BP_StalkerIdentification_C`
- `mod add /Game/Mods/StalkerId/BP_StalkerIdentification_Debug.BP_StalkerIdentification_Debug_C'`

This debug mode behaves exactly the same, except it will print some text in the top left of your screen when you target an NPC.
When you spot an NPC that doesn't identify as the right faction, please take a screenshot and send it may way (it's that text at the top that matters)

# Contribute
Since this project is available on GitHub, feel free to submit PRs or fork this off.
The way I'm currently going about identifying is by looking at meshes and materials that NPCs are made out of. It's not pretty, but I couldn't figure out another reasonable way of doing it without the SDK.

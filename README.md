# XaeroPlus

This is a Forge 1.12.2 mod that depends on and modifies Xaero's WorldMap and Minimap.

# Download

Download the latest build in the Github actions here: [https://github.com/rfresh2/XaeroPlus/actions](https://github.com/rfresh2/XaeroPlus/actions)

# Xaero Versions

Xaero WorldMap version: [1.26.2](https://www.curseforge.com/minecraft/mc-mods/xaeros-world-map/files/3907327)

Xaero Minimap version: [22.13.0](https://www.curseforge.com/minecraft/mc-mods/xaeros-minimap/files/3907306)

Both mods must be downloaded and included by you in your Forge mods folder. 

Using any version other than these two may cause crashes. 

# Modifications

* WorldMap and Waypoint directories are indexed by Multiplayer server name instead of IP. 
  * e.g. "Multiplayer_connect.2b2t.org" -> "Multiplayer_2b2t"
  * **You will need to manually change the name of any existing folder.** 
    * In both `.minecraft/XaeroWaypoints/` and `.minecraft/XaeroWorldMap/`
* Overworld dimension is stored in the "DIM0" directory instead of "null"
  * **You will need to manually change the name of any existing folder in** `.minecraft/XaeroWorldMap/Multiplayer_<server name>/`
* WorldMap zoom unlocked
* Increased region loading performance for large worlds. Fixes "hangs" on joining a server or switching dimensions.
  * Most noticeable when you have 50k+ regions per dimension.
* GUI on WorldMap to pan the map to user entered coordinates.
* Display distance to waypoints on Waypoints GUI (like JourneyMap)

# Work In Progress

* Improve WorldMap performance with very small zooms
  * With the unlocked zoom, loading many regions in view is very time (and VRAM) intensive.


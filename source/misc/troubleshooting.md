---
title: Minecolonies Wiki
layout: default
---


# Troubleshooting

## Before we start:
  Please always check if updates for [MineColonies](https://www.curseforge.com/minecraft/mc-mods/minecolonies/files/all) and [Structurize](https://www.curseforge.com/minecraft/mc-mods/structurize/files/all) are available and upgrade to the latest alpha if you are not running the latest.
  (Please note that alpha does not mean it's unstable, it just means it's a minor release.)
  

## CHECKLIST: Identifying why a citizen is not working

  1. Is it daytime? Citizens do not work after sunset.
  2. Is it raining? Citizens do not work in the rain.
  3. Did a citizen die yesterday? Citizens will mourn the next day and not work if one of them died the day before.
  4. Are there Barbarians or Pirates still around? Citizens will hide during raids until all attackers are killed.
  5. Is their workhut of low level? Does worker have low XP at their career? Then they will often idle in between actually working until their personal XP improves and /or their workhut is upgraded.
  6. Is their hut PAUSED? Work huts now have a pause button. Sometimes players forget to unpause.
  7. Is their hunger level low? Citizens won't work while hungry. Give them food and if you have a Restaurant check that it is stocked. If they are hungry but won't eat the food they have, fire them until they eat then rehire them.
  8. Do they have any open requests? They might need a tool or other material to continue their work.
  9. Does their workhut have any open requests? They might be waiting for materials to continue their work.
  10. Do they have tools of the correct [level](../../source/systems/worker)? 
  11. Is their inventory or their hut inventory full? They will get stuck if they have no room to move things in or out.
  
**Note**  If none of these apply, go on to the next Troubleshooting checklists.  

## CHECKLIST: Troubleshooting a Citizen not working by Career
  1. [Builder](../../source/workers/builder): Remember to click the Build Building button inside the hut block you want to be built, then wait for the Builder to announce they have begun building.
  2. [Lumberjack](../../source/workers/lumberjack): Set which type of tree they are allowed to cut and if they should replant them. Make sure that your trees are at ground level, or if you place them one block higher, place slabs next to them.
  3. [Miner](../../source/workers/miner): Is there an ore they cannot mine in their way? Break it for them or assign them to a new mining level.
  4. [Cook](../../source/workers/cook): Set which fuel you want them to use.
  5. [Baker](../../source/workers/baker): Set which fuel you want them to use and which recipe you want them to bake.
  6. [Smelter](../../source/workers/smelter): Set which fuel you want them to use.
  7. [Farmer](../../source/workers/farmer): Make sure each scarecrow has a seed and make sure all tilled soil is hydrated.
  8. [Composter](../../source/workers/composter): Set which items you want them to convert into compost.
  9. Crafter: The request for materials must be made after the crafter is hired and the colony must have a Delivery person. Cancel the request at the original NPC to generate a new request, or make a new request from the PostBox.
  10. Crafter: Teach them the recipes they're allowed to craft and make sure afterwards that the recipes were saved.
  11. [Blacksmith](../../source/workers/blacksmith): Set which fuel you want them to use.
  12. [Stone Smelter](../../source/workers/stonesmelter): Set which fuel you want them to use. (They know their recipes already.)  

## CHECKLIST: Troubleshooting a Citizen not working for unknown reason
  1. Log out of the game. Open the (your game location)/config/minecolonies-common.toml file.
      * Go to the line<br> 
      `#Should in development features be enabled (might be buggy). [Default: false]`<br>
      `enableInDevelopmentFeatures=false`
      * Change the false to true
      * Restart your game
      * Watch the name area above the workers head, the information at the end will be important for devs to troubleshoot issues or assist you on the discord #help channel
  2. Nudge worker by walking into them, off the block they are standing on or out a door.
  3. Recall worker to their workhut.
  4. Is the path to the worksite clear of obstructions? Recall worker to their workhut then follow them to see where they stop.
  5. Bug: They will get stuck if walking over a slab in the "top" position without another slab underneath. Check your slabs.
  6. Recall all Citizens to the TownHall.
  7. Pause the problem workhut, wait a few minutes, unpause the workhut and recall the worker.
  8. Fire worker, wait a few minutes, hire the same worker.
  9. Empty out worker's personal and workhut inventories, then only give them what they request in the amount requested until they have no more requests.
  10. Fire worker, empty out their personal and workhut inventories, wait for them to actually get into bed at night, after sunrise, hire the same worker.
  11. Punch them with empty hand (taking damage resynchronizes them with world). Never punch a guard, fire them first then punch then rehire.
  12. Use the /mc rs reset [Command](../../source/systems/commands)
  13. Repair their workhut. Some buildings will stop working if required elements are not present. Only the BuilderNPC can place beds, crafting tables, furnaces, chests, racks, compost bins. If you broke any of those, break all of them and let the BuilderNPC repair the building.
  14. Fire worker, wait a few minutes, hire a different worker (You will lose advantage of the experience the first worker had accumulated at this career).

## Missing Graphics and issues with Build Tool Preview
  If you experience missing textures for hut blocks and your previews are messed up, check if you have Optifine installed as the current version is not stable.
  As there is nothing that we can do, you can either live with missing graphics, or you will have to deactivate Optifine.

## Crashes when Placing Structures
  If your game crashes placing a structure (e.g. a supply camp), your Minecolonies and Structurize versions are probably incompatible. Update both to the latest alphas.

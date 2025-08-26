# Wand_DBG Patch: 
Fixes the ui not working, for some reason with quants.ew calling EntityGetTag causes a check to fail, the fix is one liner.
In Short it just swaps line 632 to check for a table rather than nil or not. i think some other mod is using a older version of the mod API. but the issue is easily patched

## Help needed
Most mods are loaded in by the time the game starts loading the world in, so there is a short window before original mods start calling/Using scripts we want to patch, Unless the mod is in the mods folder in notia i simply cant overwrite some scripts
Load order seems useless, putting the patcher mod before or after makes no difference when it works or not. The 2 main issues are Scripts load before i can apply the overwrite AND i cant overwrite steam mods it seems

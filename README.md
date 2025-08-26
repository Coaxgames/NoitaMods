# NoitaMods
A collection of mods and patches to mods i have made for noita



## Current Patch Mods for Noita
Wand_DBG Patch: Fixes the ui not working, for some reason with quants.ew calling EntityGetTag causes a check to fail, the fix is one liner.\n
In Short it just swaps line 632 to check for a table rather than nil or not. i think some other mod is using a older version of the mod API. but the issue is easily patched

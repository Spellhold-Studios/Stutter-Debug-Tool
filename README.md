# Stutter Debug Tool
A help to identify looping scripts in IE games.

The Stutter Debug Tool is to help debug script malfunctions in the game. For example, if an NPC "stutters", i.e. only walks a few steps and constantly terminates any actions, or if the NPC's PID (player initiated dialogue) pops up repeatedly.
Also, if the game experiences a lag which could be caused by a looping script.

The Stutter Debug Tool will patch every script block with a text stating which script and script block number is running. The text is shown in the textbox ingame and also right above the entity executing the script.

## HOW TO DEBUG A SCRIPT STUTTER

1. If you encounter an issue that could be because of a repeating script action, save your game.
2. Install the Stutter Debug Tool onto your game.
3. Load the save and identify which script block of which script keeps repeating. There might be a lot of scripts being mentioned in the dialogue box, try to identify the one that leads to the issue. 
4. The output will be something like "Running block 54 of scriptxy.bcs". Note this down.
5. Close the game.
6. Open Near Infinity. Browse to the bcs files. Open the script file that was mentioned ("scriptxy" in our example).
7. Inside the script, search for the textline you noted down, e.g. "Running block 54 of scriptxy.bcs" (without the quotion marks). The block with this text inside is the script block you are looking for.
8. I'll stress this again: the number given in the "Running block 54 of scriptxy.bcs" is NOT the line number. It refers to the BLOCK containing this text.
9. Copy the whole script block and ask in the forums for help with the stutter if you need help.
10. Deinstall the Stutter Debug Tool to continue your playthrough.


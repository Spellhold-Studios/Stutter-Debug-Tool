				    STUTTER DEBUG TOOL

                                         
ABOUT

The Stutter Debug Tool is to help debug script malfunctions in the game. For example, if an NPC "stutters", i.e. only walks a few steps and constantly terminates any actions, or if the NPC's PID (player initiated dialogue) pops up repeatedly. 
Also, if the game experiences a lag which could be caused by a looping script.

The Stutter Debug Tool will patch every script block with a text stating which script and script block number is running. The text is shown in the textbox ingame and also right above Player1's head.


The tool has two install choices. The first one leaves out all script blocks containing NoAction() that have a tendency to loop and clutter the message window. Use this if you are unsure. Use the second install choice only if you are sure it is what you need.

For debugging as a player, install the first choice [1] of the tool and load the savegame with the stutter. Note or screenshot all displayed messages until you can be sure that the stutter was called at least twice. Foreward the script names and block numbers to the mod's author or a helping modder. To be able to identify the script block(s) in question, you also need to be ready to look up the script the modder tells you with NI (Near Infinity).

For debugging as a modder, installing the tool will show ingame which scripts are running. The displayed messages should help you identify which script block is stuttering.

The tool functions like a normal WeiDU mod and can be installed and completely deinstalled like one. It is supposed to be installed directly onto your game. For EET, it can be installed after EET-end.
The tool is not meant to be included into a normal playthrough.

INSTALLATION

For installation, same as with every WeiDU mod, just put the content of the archive into the game folder.

Start setup-stutterdebug.exe (for Windows) or setup-stutterdebug (for OSX) for installation and uninstallation.

Chose your language and the install choice (chose [1] if you are unsure). From there on, wait for the process to end, it can take anything from three seconds to about three hours, depending on what kind of installation you have, and how many mods you have installed. On my (Jarno's) computer a past version took about 81 minutes when it was "copying and patching 11211 files", the installation type was then a Tactical BWS game, so it really took it's time. 
Uninstallation will take about a minute or two, maximum.

COMPATIBILITY

The Stutter Debug Tool should be compatible with all IE games. It is meant to be installed directly onto your finished game (also EET) for debugging purposes only. 

LINKS

Tutorial about how to gather clues when debugging stuttering from the bigg: http://www.shsforums.net/topic/33937-how-to-gather-clues-when-debugging-stuttering/

Tutorial from Jarno Mikkola (the tool version from that post was taken and modified for this Stutter Debug Tool):
http://www.shsforums.net/topic/41036-faq-for-the-megamods/?p=504055

Tutorial for stutter debugging from Ascalon (German):
https://www.baldurs-gate.de/index.php?threads/stutter-debug-wie-wann-und-warum.41439/

Near Infinity:
https://github.com/Argent77/NearInfinity/releases


CREDITS

the bigg - first tutorial for the stutter debug principle
Jarno Mikkola - tool pre-versions and debug guide
Ascalon - tool pre-versions and debug guide (German)

HISTORY

Version 4.0:
-Modernized, restructured and cleaned up code.
-Added support for BG1.
-Fixed support for IWD1, IWD2 and PST.

Version 3.1:
-typo correction.

Version 3:
-Removed "ActionOverride(Player1" from text output to make it more stable ingame.
-Added libiconv-1.9.2-1-src.zip for licence info.

Version 2:
-Added DisplayStringHead so text will show in window.

Version 1:
-first public release
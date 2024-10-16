<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Spellhold-Studios/Spellhold-Studios.github.io/main/assets/images/shs-corner-logo.png" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Spellhold-Studios/Spellhold-Studios.github.io/main/assets/images/shs-corner-logo.png" />
  <img align="right" alt="SHS logo" src="https://raw.githubusercontent.com/Spellhold-Studios/Spellhold-Studios.github.io/main/assets/images/shs-corner-logo.png" width="22%">
</picture>

[![Release](https://img.shields.io/github/v/release/Spellhold-Studios/Stutter-Debug-Tool?include_prereleases&color=%2392403a)](https://github.com/Spellhold-Studios/Stutter-Debug-Tool/releases/latest)
[![Published](https://img.shields.io/github/release-date/Spellhold-Studios/Stutter-Debug-Tool?display_date=published_at&label=published&color=%2392403a)](https://github.com/Spellhold-Studios/Stutter-Debug-Tool/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/Spellhold-Studios/Stutter-Debug-Tool/total?color=%2392403a)](https://github.com/Spellhold-Studios/Stutter-Debug-Tool/releases)
[![Views](https://badges.pufler.dev/visits/Spellhold-Studios/Stutter-Debug-Tool?label=views&color=%2392403a)](https://github.com/Spellhold-Studios/Stutter-Debug-Tool/releases)
[![Language](https://img.shields.io/badge/language-en%20%a0%20de%20%a0%20fr-%2392403a)](https://github.com/Spellhold-Studios/Stutter-Debug-Tool/releases)
<br>
[![Games](https://img.shields.io/badge/games-BG1%20%a0%20BG2%20%a0%20BGT%20%a0%20BG%3AEE%20%a0%20SoD%20%a0%20BG2%3AEE%20%a0%20EET%20%a0%20IWD1%20%a0%20IWD2%20%a0%20IWD%3AEE%20%a0%20PST%20%a0%20PST%3AEE-%2392403a)](https://github.com/Spellhold-Studios/Stutter-Debug-Tool/releases)

<!--
Badges white space separator: %20%a0%20
Badges ":" (colon) symbol: %3A
Badges "-" (hyphen) symbol: --
Games full list: BG1 BG2 BGT BG%3AEE SoD BG2%3AEE EET IWD1 IWD2 IWD%3AEE PST PST%3AEE
IETF language tags: https://spellhold-studios.github.io/readmes/template-basic/ietf-lang-tags.pdf
Why some badges update slowly: https://github.com/pujux/badge-it/issues/78
-->

# Stutter Debug Tool

*A Spellhold Studios tool for Infinity Engine games*

<br>

[<img alt="Download" src="https://raw.githubusercontent.com/Spellhold-Studios/Spellhold-Studios.github.io/main/assets/buttons/download.svg" height="28">](https://github.com/Spellhold-Studios/Stutter-Debug-Tool/releases/latest)&nbsp;
[<img alt="Readme" src="https://raw.githubusercontent.com/Spellhold-Studios/Spellhold-Studios.github.io/main/assets/buttons/readme.svg" height="28">](https://spellhold-studios.github.io/readmes/stutter-debug-tool/readme-stutterdebug.english.txt)&nbsp;
[<img alt="Webpage" src="https://raw.githubusercontent.com/Spellhold-Studios/Spellhold-Studios.github.io/main/assets/buttons/webpage.svg" height="28">](https://spellhold-studios.github.io/)&nbsp;
[<img alt="Discord" src="https://raw.githubusercontent.com/Spellhold-Studios/Spellhold-Studios.github.io/main/assets/buttons/discord-blue.svg" height="28">](https://discord.gg/pE2Njbdb2a)

## Introduction

Stutter Debug Tool helps debug script malfunctions in the game. For example, if an NPC "stutters", i.e. only walks a few steps and constantly terminates any actions, or if the NPC's PID (player initiated dialogue) pops up repeatedly. Also, if the game experiences a lag which could be caused by a looping script.

The tool will patch every script block with a text stating which script and block number is running. The text is shown in the dialogue box in-game and right above the entity executing the script.

*Please check the complete [Readme](https://spellhold-studios.github.io/readmes/stutter-debug-tool/readme-stutterdebug.english.txt) to learn more about this tool before installation.*

## How to debug a script stutter

1. If you encounter an issue that could be caused by a repeating script action, save your game.
2. Install the Stutter Debug Tool onto your game.
3. Load the save and identify which script or block keeps repeating. There might be a lot of scripts mentioned in the dialogue box, so try to identify the one that leads to the issue.
4. The output will be something like, "Running block 54 of scriptxy.bcs". Note this down.
5. Exit the game.
6. Open Near Infinity. Browse to the bcs files. Open the script file that was mentioned ("scriptxy" in our example).
7. Inside the script, search for the textline you noted down, e.g. "Running block 54 of scriptxy.bcs" (without the quotion marks). The block with this text inside is the script block you are looking for.
8. I'll stress this again: the number given in the "Running block 54 of scriptxy.bcs" is NOT the line number. It refers to the BLOCK containing this text.
9. Copy the whole script block and ask for help with the stutter if need be.
10. Deinstall the Stutter Debug Tool to continue your playthrough.

## Credits

<!-- double space after each credits **Heading** if you don't need lists -->

**WeiDU coding**

- jastey
- Argent77

**Contributors**  

- the bigg &nbsp;&ndash;&nbsp; first tutorial for the stutter debug principle
- Jarno Mikkola &nbsp;&ndash;&nbsp; tool pre-versions and debug guide
- Ascalon &nbsp;&ndash;&nbsp; tool pre-versions and debug guide (German)

**Translators**  

- Selphira &nbsp;&ndash;&nbsp; French

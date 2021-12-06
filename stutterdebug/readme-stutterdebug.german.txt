				    STUTTER DEBUG TOOL

ALLGEMEINES

Das Stutter Debug Tool hilft dabei, durch Skripte ausgelöste Probleme im Spiel zu debuggen. Diese können z.B. ein NPC sein, der immer nach wenigen Schritten stehen bleibt, alle Aktionen abbricht, und (falls vorhanden) sich immer wieder der PID (spieler-initiierter Dialog) öffnet. Es können aber auch Lags im Spielfluss sein, die auf eine durch Skripte (über)beschäftigte Engine hinweisen könnten.

Das Stutter Debug Tool stattet hierzu jeden Skriptblock mit einer Textausgabe aus, die den Namen des ausführenden Skripts und die Nummer des Skriptblocks im Spiel sowohl in der Dialogbox als auch als fliegender Text über dem Hauptcharakter anzeigt.


Das Tool hat zwei Installationsmöglichkeiten. Die erste lässt alle Skriptblöcke aus, die aktiv sind, solange das entsprechende Skript nichts anderes "zu tun" hat (NoAction()). Diese führen zu vielen sich wiederholenden Textausgaben, die aber vom eigentlichen Stutter ablenken können. Die erste Installationsoption sollte gewählt werden, wenn es für die zweite keinen Grund gibt. Die zweite patcht alle Skriptblöcke und sollte nur gewählt werden, wenn die erste zu keinem Ergebnis führt.

Als Spieler ohne Moddingerfahrung installiert Ihr die erste Option [1] und startet das Spiel mit dem Save, der die Probleme enthält. Schreibt alle Textnachrichten im Spiel auf oder macht Screenshots, bis sich der Stutter wiederholt. Mit den nun in Erfahrung gebrachten Skriptnamen kann Euch der Modautor oder ein anderer Modder nun sagen, welches davon Ihr mit Near Infinity nachschauen könnt, um den bzw. die relevanten Skriptblöcke zu identifizieren.

Zum Debuggen mit Moddingerfahrung installiert Ihr das Tool und verwendet die angezeigten Textnachrichten im Spiel, um den relevanten Skriptblock herauszufinden.

Das Tool funktioniert wie ein normales WeiDU-Mod und kann daher auch vollständig wieder deinstalliert werden. Es wird einfach auf das bestehende Spiel installiert. Dies gilt auch für EET: die EET-End.exe muss (bzw. soll auch) nicht danach ausgeführt werden.
Das Tool ist nicht dazu gedacht, in eine normale Spielinstallation von Beginn an beinhaltet zu sein.

INSTALLATION

Extrahiert den Inhalt des Modpakets (den Modordner und die Executables) in Euren Spielordner. Die Installation erfolgt wie bei einer normalen WeiDU-Mod durch Starten der setup-stutterdebug.exe (für Windows) bzw. setup-stutterdebug (für OSX). Dies gilt auch für die Deinstallation.

Wählt Eure Sprache aus und eine der Installationsoptionen. Falls es keinen besonderen Grund für die zweite gibt, sollte die erste Installationsoption [1] gewählt werden. 
Danach muss gewartet werden, bis das Patchen der Skripte erfolgt ist. Dies kann durchaus sehr lange dauern. Bei einer früheren Version des Tools in einer Tactical BWS-Installation (Jarno's) mit 11211 Skripten dauerte die Installation 81 Minuten.
Das Deinstallieren ist wie immer bei WeiDU-Mods sehr schnell.

KOMPATIBILITÄT

Das Stutter Debug Tool sollte mit allen IE-Spielen kompatibel sein. Es ist dafür gedacht, temporär für das Debuggen auf eine fertige Installation installiert zu werden, auch für EET.

LINKS

(Englisch) Tutorial about how to gather clues when debugging stuttering from the bigg: http://www.shsforums.net/topic/33937-how-to-gather-clues-when-debugging-stuttering/

(Englisch) Tutorial from Karno Mikkola (the tool version from that post was taken and modified for this Stutter Debug Tool):
http://www.shsforums.net/topic/41036-faq-for-the-megamods/?p=504055

Tutorial über Stutter Debugging von Ascalon:
https://www.baldurs-gate.de/index.php?threads/stutter-debug-wie-wann-und-warum.41439/

Near Infinity:
https://github.com/Argent77/NearInfinity/releases


CREDITS

the bigg - first tutorial for the stutter debug principle
Jarno Mikkola - tool pre-versions and debug guide
Ascalon - tool pre-versions and debug guide (German)

HISTORY

Version 3:
-Removed "ActionOverride(Player1" from text output to make it more stable ingame.
-Added libiconv-1.9.2-1-src.zip for licence info.

Version 2:
-Added DisplayStringHead so text will show in window.

Version 1:
-first public release
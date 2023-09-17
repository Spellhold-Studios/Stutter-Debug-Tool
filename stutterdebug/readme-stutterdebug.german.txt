				    STUTTER DEBUG TOOL

ALLGEMEINES

Das Stutter Debug Tool hilft dabei, durch Skripte ausgelöste Probleme im Spiel zu debuggen. Diese können z.B. ein NPC sein, der immer nach wenigen Schritten stehen bleibt, alle Aktionen abbricht, und (falls vorhanden) sich immer wieder der PID (spieler-initiierter Dialog) öffnet. Es können aber auch Lags im Spielfluss sein, die auf eine durch Skripte (über)beschäftigte Engine hinweisen könnten.

Das Stutter Debug Tool stattet hierzu jeden Skriptblock mit einer Textausgabe aus, die den Namen des ausführenden Skripts und die Nummer des Skriptblocks im Spiel sowohl in der Dialogbox als auch als fliegender Text über dem Hauptcharakter anzeigt.


Das Tool hat zwei Installationsmöglichkeiten. Die erste lässt alle Skriptblöcke aus, die aktiv sind, solange das entsprechende Skript nichts anderes "zu tun" hat (NoAction()). Diese führen zu vielen sich wiederholenden Textausgaben, die aber vom eigentlichen Stutter ablenken können. Die erste Installationsoption sollte gewählt werden, wenn es für die zweite keinen Grund gibt. Die zweite patcht alle Skriptblöcke und sollte nur gewählt werden, wenn die erste zu keinem Ergebnis führt.

Als Spieler ohne Moddingerfahrung installiert Ihr die erste Option [1] und startet das Spiel mit dem Save, der die Probleme enthält. Schreibt alle Textnachrichten im Spiel auf oder macht Screenshots, bis sich der Stutter wiederholt. Mit den nun in Erfahrung gebrachten Skriptnamen kann Euch der Modautor oder ein anderer Modder nun sagen, welches davon Ihr mit Near Infinity nachschauen könnt, um den bzw. die relevanten Skriptblöcke zu identifizieren.

Zum Debuggen mit Moddingerfahrung installiert Ihr das Tool und verwendet die angezeigten Textnachrichten im Spiel, um den relevanten Skriptblock herauszufinden.

Das Tool funktioniert wie ein normales WeiDU-Mod und kann daher auch vollständig wieder deinstalliert werden. Es wird einfach auf das bestehende Spiel installiert. Dies gilt auch für EET: die EET-End.exe muss (bzw. soll auch) nicht danach ausgeführt werden.
Das Tool ist nicht dazu gedacht, in eine normale Spielinstallation von Beginn an beinhaltet zu sein.
Bitte beachten: Das Tool kann Cutscenes "hängen" lassen. Deinstalliert es, bevor Ihr mit dem Durchspielen fortfahrt.

WIE MAN BEIm DEBUGGING VORGEHT
(übersetzt mit DeepL)

1. Wenn Sie auf ein Problem stoßen, das auf eine sich wiederholende Skriptaktion zurückzuführen sein könnte, speichern Sie Ihr Spiel.
2. Installieren Sie das Stutter Debug Tool in Ihrem Spiel.
3. Laden Sie den Spielstand und finden Sie heraus, welcher Skriptblock sich wiederholt. Möglicherweise werden in der Dialogbox viele Skripte erwähnt. Versuchen Sie herauszufinden, welches Skript zu dem Problem führt. 
4. Die Ausgabe wird in etwa lauten: "Running block 54 of scriptxy.bcs". Notieren Sie sich dies.
5. Schließen Sie das Spiel.
6. Öffnen Sie Near Infinity (Link unten) und suchen Sie die bcs-Dateien. Öffnen Sie die erwähnte Skriptdatei ("scriptxy" in unserem Beispiel).
7. Suchen Sie innerhalb des Skripts nach der Textzeile, die Sie notiert haben, z. B. "Running block 54 of scriptxy.bcs" (ohne die Anführungszeichen). Der Block, in dem dieser Text steht, ist der gesuchte Skriptblock.
8. Ich betone es noch einmal: Die Nummer in "Running block 54 of scriptxy.bcs" ist NICHT die Zeilennummer. Sie bezieht sich auf den BLOCK, der diesen Text enthält.
9. Kopieren Sie den gesamten Skriptblock und fragen Sie in den Foren nach Hilfe, wenn Sie Hilfe benötigen.
10. Deinstallieren Sie das Stutter Debug Tool, um Ihr Spiel fortzusetzen.

INSTALLATION

Extrahiert den Inhalt des Modpakets (den Modordner und die Executables) in Euren Spielordner. Die Installation erfolgt wie bei einer normalen WeiDU-Mod durch Starten der setup-stutterdebug.exe (für Windows) bzw. setup-stutterdebug (für OSX). Dies gilt auch für die Deinstallation.

Wählt Eure Sprache aus und eine der Installationsoptionen. Falls es keinen besonderen Grund für die zweite gibt, sollte die erste Installationsoption [1] gewählt werden. 
Danach muss gewartet werden, bis das Patchen der Skripte erfolgt ist. Dies kann durchaus sehr lange dauern. Bei einer früheren Version des Tools in einer Tactical BWS-Installation (Jarno's) mit 11211 Skripten dauerte die Installation 81 Minuten.
Das Deinstallieren ist wie immer bei WeiDU-Mods sehr schnell.

KOMPATIBILITÄT

Das Stutter Debug Tool sollte mit allen IE-Spielen kompatibel sein. Es ist dafür gedacht, temporär für das Debuggen auf eine fertige Installation installiert zu werden, auch für EET.

LINKS

(Englisch) Tutorial about how to gather clues when debugging stuttering from the bigg: http://www.shsforums.net/topic/33937-how-to-gather-clues-when-debugging-stuttering/

(Englisch) Tutorial from Jarno Mikkola (the tool version from that post was taken and modified for this Stutter Debug Tool):
http://www.shsforums.net/topic/41036-faq-for-the-megamods/?p=504055

Tutorial über Stutter Debugging von Ascalon:
https://www.baldurs-gate.de/index.php?threads/stutter-debug-wie-wann-und-warum.41439/

Near Infinity:
https://github.com/Argent77/NearInfinity/releases

DeepL Online Translator:
https://www.deepl.com/translator


CREDITS

the bigg - first tutorial for the stutter debug principle
Jarno Mikkola - tool pre-versions and debug guide
Ascalon - tool pre-versions and debug guide (German)

HISTORY

Version 4.1:
-French version added, by Selphira.
-Added paragraph to the readme: HOW TO DEBUG A SCRIPT STUTTER.
-Fix SoD detection for game info output.

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
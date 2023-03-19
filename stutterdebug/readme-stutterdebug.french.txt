				    STUTTER DEBUG TOOL
                                         

À PROPOS

Le Stutter Debug Tool est destiné à aider à déboguer les dysfonctionnements des scripts dans le jeu. Par exemple, si un PNJ "bégaie", c'est-à-dire qu'il ne fait que quelques pas et interrompt constamment toute action, ou si le PID (dialogue initié par le joueur) du PNJ s'affiche de manière répétée.
De même, si le jeu subit un ralentissement qui pourrait être causé par un script qui tourne en boucle.

Le Stutter Debug Tool ajoutera à chaque bloc de script un texte indiquant le nom et le numéro du bloc du script en cours d'exécution. Le texte est affiché dans la zone de texte en jeu et au-dessus de la tête du joueur 1.


L'outil a deux choix d'installation. Le premier permet de laisser de côté tous les blocs de script contenant NoAction() qui ont tendance à tourner en boucle et à encombrer la fenêtre de message. Utilisez ce choix si vous n'êtes pas sûr de vous. N'utilisez le second choix d'installation que si vous êtes sûr que c'est ce dont vous avez besoin.

Pour le débogage en tant que joueur, installez le premier choix [1] de l'outil et chargez la sauvegarde avec le problème. Notez ou faites une capture d'écran de tous les messages affichés jusqu'à ce que vous soyez sûr que le problème a été rencontré  au moins deux fois. Transmettez les noms des scripts et les numéros des blocs à l'auteur du mod ou au moddeur qui vous aide. Pour pouvoir identifier le(s) bloc(s) de script en question, vous devez également être prêt à rechercher le script que le moddeur vous indique avec NI (Near Infinity).

Pour le débogage en tant que moddeur, l'installation de l'outil montrera en jeu quels scripts sont en cours d'exécution. Les messages affichés devraient vous aider à identifier le bloc de script responsable du problème.

L'outil fonctionne comme un mod WeiDU normal et peut être installé et désinstallé comme tel. Il est censé être installé directement sur votre jeu. Pour EET, il peut être installé après EET_End.
L'outil n'est pas destiné à être inclus dans une partie normale.

INSTALLATION

Pour l'installation, comme pour tous les mods WeiDU, il suffit de mettre le contenu de l'archive dans le dossier du jeu.

Lancez setup-stutterdebug.exe (pour Windows) ou setup-stutterdebug (pour OSX) pour l'installation et la désinstallation.

Choisissez votre langue et le composant à installer (choisissez [1] si vous n'êtes pas sûr). A partir de là, attendez que le processus se termine, cela peut prendre de trois secondes à environ trois heures, selon le type d'installation que vous avez, et le nombre de mods que vous avez installés. Sur mon ordinateur (celui de Jarno), une version antérieure a pris environ 81 minutes lorsqu'il s'agissait de "copier et patcher 11211 fichiers", le type d'installation était l'option Tactical du BWS, il a donc vraiment pris son temps.
La désinstallation prendra environ une minute ou deux, au maximum.

COMPATIBILITÉ

Le Stutter Debug Tool devrait être compatible avec tous les jeux IE. Il est destiné à être installé directement sur votre jeu (également EET) à des fins de débogage uniquement.

LIENS

Tutoriel sur la façon de recueillir des indices lors du débogage des problèmes de bégaiement de the bigg :http://www.shsforums.net/topic/33937-how-to-gather-clues-when-debugging-stuttering/

Tutoriel de Jarno Mikkola (la version de cet outil a été reprise et modifiée pour ce Stutter Debug Tool) :
http://www.shsforums.net/topic/41036-faq-for-the-megamods/?p=504055

Near Infinity:
https://github.com/Argent77/NearInfinity/releases


CRÉDITS

the bigg - premier tutoriel pour le principe de débogage des problème de bégaiement
Jarno Mikkola - pré-versions de l'outil et guide de débogage
Ascalon - pré-versions de l'outil et guide de débogage (allemand)

HISTORIQUE

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
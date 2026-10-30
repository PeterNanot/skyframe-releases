# Skyframe — versions publiées

Skyframe est un logiciel de montage vidéo pour Windows, pensé pour les vidéos de drone : stabilisation, profils
D-Log et HLG, données de vol DJI, montage automatique, export pour YouTube, Instagram et TikTok.

Ce dépôt contient uniquement les **installeurs Windows**. Le code source de Skyframe est privé.

## Installer

1. Ouvrez la [dernière version](https://github.com/PeterNanot/skyframe-releases/releases/latest) et téléchargez
   `skyframe-<version>-setup.exe`.
2. Lancez-le. L'installeur n'est pas signé : Windows SmartScreen affiche un avertissement au premier lancement.
   Cliquez sur « Informations complémentaires », puis « Exécuter quand même ».

Skyframe s'installe pour votre compte Windows, sans droits administrateur.

## Mettre à jour

Dans Skyframe : **Paramètres → À propos → Rechercher une mise à jour**. C'est le seul moment où Skyframe se connecte
à internet. Vous pouvez aussi lancer le nouvel installeur : il indique la version en place et propose la mise à jour.
Vos projets et vos vidéos ne sont jamais modifiés.

## Licences des composants

Depuis la version 0.12.0, Skyframe embarque **FFmpeg 9.0.2** compilé par [BtbN/FFmpeg-Builds](https://github.com/BtbN/FFmpeg-Builds)
(variante « win64-lgpl », sans composant GPL), distribué sous licence **GNU LGPL v3**. Le texte de la licence est
installé avec Skyframe (`resources/bin/FFMPEG-LICENSE.txt`).

Code source correspondant :

- FFmpeg 9.0.2 : <https://github.com/FFmpeg/FFmpeg/tree/n9.0.2> et <https://ffmpeg.org/releases/>
- Scripts de compilation : <https://github.com/BtbN/FFmpeg-Builds>
- Archive utilisée (copie à l'identique) : <https://github.com/PeterNanot/skyframe-releases/releases/tag/ffmpeg-9.0.2-lgpl>

Les versions 0.11.0 et antérieures embarquaient FFmpeg 9.0.2 « essentials » de [gyan.dev](https://www.gyan.dev/ffmpeg/builds/),
sous licence GNU GPL v3 (sources : <https://ffmpeg.org/releases/ffmpeg-9.0.2.tar.xz>,
<https://github.com/GyanD/codexffmpeg/releases/tag/9.0.2>).

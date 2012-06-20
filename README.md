#VisualVoiceLink

Une application Android qui fait le lien entre les messages vocaux envoyés par mail et le lecteur Visual Voicemail d'Android 4.0

##Objectif

Intégrer la lecture des messages vocaux Free Mobile dans Android 4.x

##Principes

L'application doit via une connexion IMAP récupérer un message vocal envoyé par mail ainsi que les informations associées (numéro / date / type) et les transférer en tant que voicemail dans Android 4.x

La création de voicemail fonctionne déjà (voir code initial) grace aux démo du projet Android.

cf https://docs.google.com/drawings/d/1PflMU_wSkBtmh3jeSBpLIvCVWIdsSVamL7fg-9cDKq8/edit pour le fonctionnement général.

##Technique

* Utilisation de l'expedition de mails automatique pour les messages reçus de FreeMobile https://mobile.free.fr/moncompte/index.php?page=messagerie
* Connexion de l'application android en IMAP et recherche des messages contenant VMS et [Freemobile]
* Téléchargement du fichier .wav contenant le message et ajout des méta information depuis le mail
* Enregistrement de l'ID du message (pour ne pas le re-télécharger)
* Envois du message dans l'API Voicemail d'Android 4.x
* That's all folks!

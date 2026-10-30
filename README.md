# Découpe

[Télécharger l’APK](https://github.com/Zachiran42/decoupe/releases/latest/download/decoupe-0.1.0.apk) · [Versions](https://github.com/Zachiran42/decoupe/releases) · [Page du jeu](https://zachiran42.github.io/decoupe/)

Prototype Android natif hors ligne, sans publicité et sans permission. Android8+, APK universel. Licence MIT.

Trois plaques, deux traits maximum par plaque. Garde 50 %, 35 % puis65 % de la surface initiale. Trace un trait qui traverse la plaque, touche le fragment à garder, puis valide ou affine par une seconde coupe. Refaire permet un nouvel essai sans pénalité. Le score récompense la précision.

## Compiler
Configurer .toolchain.json à partir du modèle et définir MINIGAMES_KEYSTORE_PASSWORD dans l’environnement. scripts/build.ps1 prend une clé externe (-KeyStore) et son alias (-KeyAlias). Ne jamais publier les clés.

APK signé de développement ; aucun essai sur appareil physique effectué. Pause à la mise en arrière-plan. Le record est conservé localement ; la tentative en cours reste en mémoire tant que le processus vit.

## Dans Cercle

Dans « Ajouter depuis GitHub », coller `https://github.com/Zachiran42/decoupe`. La dernière Release contient un seul APK, signé, universel et sans permission Internet.

## Compilation

Copier `.toolchain.example.json` vers `.toolchain.json`, renseigner JDK21, Android SDK36 et Build Tools, puis définir `MINIGAMES_KEYSTORE_PASSWORD` dans l’environnement. Utiliser `scripts/build.ps1 -KeyStore C:/cles/jeu.keystore -KeyAlias votre-alias`. Garder les clés hors du dépôt.

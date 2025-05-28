1. Installer les prérequis
a) Installer Flutter SDK
Télécharge Flutter sur flutter.dev (selon ton OS).

Ajoute le dossier flutter/bin à ta variable PATH pour pouvoir lancer flutter depuis le terminal.

b) Installer Android Studio (pour l’émulateur)
Même si tu ne veux pas coder dans Android Studio, il te faut le SDK Android et l’émulateur.

Installe Android Studio depuis developer.android.com.

Pendant l’installation, coche les cases pour installer le Android SDK et le Android Emulator.

c) Configurer un AVD (Android Virtual Device)
Lance Android Studio une fois.

Ouvre le AVD Manager (dans la barre d’outils ou via menu Tools > AVD Manager).

Crée un nouvel émulateur (par exemple Pixel 5, Android 13).

Lance cet émulateur et laisse-le démarrer.

2. Configurer VS Code
a) Installer l’extension Flutter
Ouvre VS Code.

Va dans l’onglet Extensions (icône carré à gauche).

Recherche Flutter et installe l’extension officielle (elle installera aussi Dart automatiquement).

b) Vérifier la configuration Flutter
Ouvre un terminal intégré (Ctrl+ ou Cmd+).

Tape flutter doctor et vérifie que tout est OK.

S’il manque quelque chose (ex : licence Android SDK), suis les instructions affichées.

3. Lancer ton app Flutter dans VS Code
a) Ouvrir ton projet Flutter dans VS Code
Ouvre le dossier racine de ton projet.

b) Lancer l’émulateur Android (si pas déjà lancé)
Si l’émulateur est déjà ouvert, VS Code le détectera automatiquement.

Sinon, lance-le via Android Studio ou en ligne de commande (ex: emulator -avd Pixel_5_API_30).

c) Lancer l’app sur l’émulateur
Dans VS Code, tu peux cliquer en bas à droite sur la liste des devices et sélectionner ton émulateur Android.

Puis appuie sur F5 ou va dans le menu Run > Start Debugging.

L’app se compile en mode debug et s’installe sur l’émulateur.

4. Utiliser le Hot Reload
Une fois l’app lancée en debug, tu peux modifier ton code dans VS Code.

Sauvegarde le fichier (Ctrl+S / Cmd+S).

Le hot reload s’exécute automatiquement, tu vois les changements quasi instantanément dans l’émulateur.

Tu peux aussi utiliser la commande Flutter: Hot Reload via palette de commandes (Ctrl+Shift+P).

5. Tester sur un vrai appareil Android (optionnel)
Active le mode développeur sur ton téléphone Android (tapote 7 fois sur “Numéro de build” dans les paramètres).

Active le débogage USB.

Connecte ton téléphone en USB à ton PC.

Dans VS Code, le téléphone apparaîtra dans la liste des devices.

Lance l’app dessus comme sur l’émulateur.

Bonus : conseils pour un workflow smooth
Active l’option Auto Save dans VS Code pour ne pas oublier de sauvegarder.

Utilise le terminal intégré pour lancer des commandes Flutter (flutter clean, flutter pub get).

Garde un œil sur la console Debug pour voir logs et erreurs en temps réel.
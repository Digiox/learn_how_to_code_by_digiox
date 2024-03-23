
# Versionner son code

Dans cet exercice, nous allons apprendre à créer différentes versions de notre code en utilisant Git.

## Installation de Git

1. Commencez par télécharger et installer Git depuis [ce lien](https://github.com/git-for-windows/git/releases/download/v2.44.0.windows.1/Git-2.44.0-64-bit.exe).

2. Une fois l'installation terminée, ouvrez une invite de commande pour vérifier l'installation avec la commande suivante : `git --version`. Si Git est correctement installé, la version de Git s'affichera.

Si la version ne s'affiche pas, essayez de redémarrer votre invite de commande ou votre éditeur de code (comme Visual Studio Code). Si le problème persiste, redémarrez votre ordinateur. Ce problème peut survenir car l'invite de commande ou l'éditeur ne reconnaît pas les nouvelles variables d'environnement sans un redémarrage.

## Initialisation de Git

1. Dans le dossier racine de votre projet, initialisez Git avec la commande `git init`. Un message devrait confirmer que le dépôt Git a été initialisé avec succès.

## Création de branches

Git utilise un système de branches pour gérer différentes versions du code. Voici comment créer des branches :

- Pour créer une branche, utilisez `git branch nom_de_la_branche`, par exemple : `git branch feat/login`.
- Pour lister toutes les branches, tapez `git branch`.
- Créez les branches suivantes pour l'exercice : `feat/login`, `fix/button-size`, `chore/code-cleaning`, `deps/bootstrap`.

## Navigation entre les branches

- Pour naviguer entre les branches, utilisez `git checkout nom_de_la_branche`.
- Par défaut, vous commencez sur la branche principale nommée `main`.

## Suivi de fichiers avec Git

1. Sur la branche `feat/login`, créez un fichier `login.txt`.
2. Pour que Git suive ce fichier, utilisez `git add login.txt`.
3. Pour vérifier que le fichier est suivi, tapez `git ls-files`.
4. Enregistrez vos modifications avec `git commit -m "feat/login: Ajout du login"`.

## Rendu attendu

Vous devriez avoir 4 branches avec un fichier dans chacune, tous suivis et commités :

- `feat/login` contenant `login.txt`
- `fix/button-size` contenant `button.txt`
- `chore/code-cleaning` contenant `clean.txt`
- `deps/bootstrap` contenant `bootstrap.txt`

## Note

Toutes les modifications apportées aux fichiers seront également sauvegardées par Git.

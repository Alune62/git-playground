# git-playground
# Configuration du comportement de Push par défaut dans Git

<!-- Ce projet documente la résolution du défi LabEx consistant à configurer Git pour qu'il pousse automatiquement la branche locale actuelle vers une branche distante portant exactement le même nom, sans avoir à le spécifier explicitement à chaque fois.

--- -->

## 📝 Contexte du Défi

<!-- Par défaut, pousser des modifications vers un dépôt distant peut s'avérer fastidieux si l'on doit constamment spécifier la branche cible (`git push origin ma-branche`). Configurer le paramètre `push.default` sur `current` permet de simplifier le flux de travail et d'éviter les erreurs de saisie, en particulier lors de la gestion de multiples branches de fonctionnalités (*feature branches*). -->

## 🛠️ Étapes de Réalisation

### 1. Clonage et Configuration du Dépôt
<!-- Commencez par cloner votre fork personnel et accédez au répertoire :
```bash
git clone [https://github.com/votre-nom-utilisateur/git-playground.git](https://github.com/votre-nom-utilisateur/git-playground.git)
cd git-playground -->

<!-- Définition de la branche de poussée par défaut
Configurez Git pour qu'il utilise le nom de la branche locale actuelle comme cible par défaut lors d'un git push :

Bash
git config push.default current -->
<!-- 
Création d'une nouvelle branche et modifications
Créez une branche de test nommée my-branch, basculez dessus, puis créez le fichier demandé :

Bash
# Créer et basculer sur la branche
git checkout -b my-branch

# Créer le fichier hello.txt avec le contenu requis
echo "Hello, World" > hello.txt

# Indexer et commiter les modifications
git add hello.txt
git commit -m "Add hello.txt" -->

<!-- Poussée vers le dépôt distant
Grâce à la configuration effectuée à l'étape 2, il vous suffit désormais de taper la commande simplifiée suivante. Git créera et poussera automatiquement vers my-branch sur GitHub :

Bash
git push -->
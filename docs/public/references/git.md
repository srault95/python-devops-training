# Git Aide Mémoire

En partant du principe que vous venez de créer un repository **python-training** dans votre espace utilisateur GitLab, voici les commandes à effectuer pour commencer à l'utiliser:

```shell
$ cd exercices
$ git init
$ git remote add origin https://YOUR_GIT_USERNAME:TOKEN@git.lbn.fr/YOUR_GIT_USERNAME/python-training.git
$ git add .
$ git commit -m "initial commit"
$ git push origin master
```

> Le token d'authentification à gitlab doit être généré [ici](https://git.lbn.fr/profile/personal_access_tokens)


- Si le dépôt existait déjà sur Gitlab et qu'il contenait déjà des fichiers, nous aurions commencés par:
```shell
git clone https://YOUR_GIT_USERNAME:TOKEN@git.lbn.fr/YOUR_GIT_USERNAME/python-training.git
```

---

### Les commandes essentiels de GIT

- `git init`: Active git pour le répertoire en cours (créé un sous-répertoire .git)
- `git status` : Affiche le status des fichiers dans le dépôt local
- `git add -A` . : Active ou met à jour le suivi de version des fichiers
- `git commit -m "message"` : Publie localement les dernières modifications
- `git remote add origin http://xxx`: Définit l'adresse du dépôt distant (.git/config)
- `git push origin master`: Publie les modifications sur le dépôt distant
- `git log`: Affiche les dernières modifications


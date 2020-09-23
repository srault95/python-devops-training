# Initiation au langage Python

---

## Résumé du planning de la formation

---

## Description des objectifs pédagogiques

---

## Introduction à Python

---

### Python VS les autres languages

* Librairies disponibles pour tous les Cloud Providers
* Installé par défaut sur la plupart des distributions Linux
* Pas de compilation, l'exécution du code est immédiate
* Courbe d'apprentissage rapide
* Langage structurant
* Beaucoup de documentation et d'exemples sur internet
* C'est aussi, une question d'appétence !

---

### Les Success Stories Python

- [Django](https://www.djangoproject.com/)
- [Ansible](https://github.com/ansible/ansible)
- [OpenStack](https://github.com/openstack)
- [docker-compose](https://github.com/docker/compose)
- Python scientifique (Scipy|Matplotlib|Numpy)
- Machine Learning (scikit-learn)
- Big Data (Pandas)

---

### Python et le Cloud

- Amazon AWS
    - Lambda serverless
    - Boto3
- Microsoft Azure
    - Azure Functions
    - az-cli
- Google GCP
    - Cloud Functions
    - App Engine

---

### Python2 vs Python3

- **Python 3** est disponible depuis **fin 2008**
- **Python 2** n'est plus supporté par l'éditeur depuis le 1er Janvier 2020
- Encodage natif en UTF8
- Coroutines avec AsyncIO

*Les principales différences sont décrites [ici](https://python-future.org/compatible_idioms.html)*

---

### L'Ecosystème Python

- [Dépôt central des projets Python](https://pypi.org/)
- [Référentiel d'outils et projet Python](https://github.com/vinta/awesome-python)
- [Github](https://github.com/topics/python?l=python&o=desc&s=stars)

---

### IDE pour Python

- VSCode
- Pycharm
- Eclipse
- notepadd++ (windows)
- vim (linux)

---

### Trouver de l'aide sur Python

- Fonction help
- [stackoverflow](https://stackoverflow.com/questions/tagged/python)
- [developpez.com](https://python.developpez.com/)
- [Algorithmie](https://github.com/TheAlgorithms/Python/blob/master/DIRECTORY.md)
- [Designs Patterns](https://github.com/faif/python-patterns)

---

## Les bases du langage Python

---

### Les bases du langage (partie 1/3)

* Python en ligne de commande
* Le shell Python
* Les types de base
* Variables & Constantes
* Formatage des chaines
* Manipulation de chaines
* Calcul avec les types numériques

---

### Les bases du langage (partie 2/3)

* Le type None
* Le type Boolean
* Les tableaux indexés (list/tuple)
* Le tableau associatif (dict)
* Python et l’indentation
* La boucle for
* La boucle while
* Conditions if/elif/else

---

### Les bases du langage (partie 3/3)

* Lecture et écriture dans un fichier
* Les modules standards fournis avec Python
* Le module time
* Le module datetime
* Passage du shell au script Python

---

## Exercice 1

Un client vous demande de générer un fichier [**.htaccess**](http://httpd.apache.org/docs/current/howto/htaccess.html) pour Apache à partir d'une liste d'adresse IP qu'il vous fournit dans un ticket. 

Dans un premier temps, nous allons uniquement afficher le résultat à l'écran, plus tard nous verrons comment l'écrire dans un fichier.

[Lien vers l'exercice](EXERCICE_URL/#/ex1.html)

---

### Correction de l'exercice n°1

---

## Versionner un projet avec Git

---

## Exercice 2

La demande du client évolue, vous allez maintenant générer le fichier .htaccess à partir d’un fichier CSV qui contiendra également une colonne pour appliquer un Deny ou un Allow sur chaque adresse IP

[Lien vers l'exercice](EXERCICE_URL/#/ex2.html)

---

### Correction de l'exercice n°2

---

## Gestion des erreurs en Python

---

### Intégration de la gestion d’erreur au générateur de fichier .htaccess

---

## Les logs Python avec le module logging

---

### Intégration de logging au générateur de fichier .htaccess

---

## Exercice 3

À la suite d’erreurs dans le format d’adresse IP, vous allez ajouter une validation du format dans le générateur de fichier .htaccess à l’aide du module standard [ipaddress](https://docs.python.org/fr/3.7/library/ipaddress.html) 

[Lien vers l'exercice](EXERCICE_URL/#/ex3.html)

---

### Correction de l'exercice n°3

---

## Retour sur les acquis de la journée

- Les bases du langage
- Git
- Etat de l'application de génération de fichier .htaccess

---

## Environnement d’exécution Python (virtualenv, pip)

---

## Installation et utilisation du shell IPython

---

## Les fonctions en Python

---

### La pseudo fonction main

---

## Exercice n°4

Transformez le code du générateur de fichier .htaccess en le réécrivant sous forme de fonction et appelez les fonctions à l’intérieur d’une fonction main.

---

### Correction de l'exercice n°4

---

## Les bonnes pratiques du nommage

---

## Documenter du code Python

---

## Documenter un projet Python avec Markdown

---

## Exercice n°5

Appliquez les bonnes pratiques du nommage et documentez le code & projet pour le générateur de fichier .htaccess

---

### Correction de l'exercice n°5

---

## Le module argparse pour des options en ligne de commande

---

## Exercice n°6

Dans le générateur de fichier .htaccess, utilisez argparse pour choisir l’emplacement du fichier CSV et le niveau de logging.

---

### Correction de l'exercice n°6

---

## Configuration dynamique à l’aide des variables d’environnement

---

## Exercice n°7

Dans le générateur de fichier .htaccess, utilisez argparse pour choisir l’emplacement du fichier CSV et le niveau de logging.

---

### Correction de l'exercice n°7

Dans notre générateur, configurez l’emplacement du fichier .htaccess à l’aide d’une variable d’environnement.

---

## Utilisation de templates Jinja

---

## Exercice n°8

Créez et utilisez un template Jinja pour formater le fichier .htaccess

---

### Correction de l'exercice n°8

---

## Introduction aux tests unitaires

---

## Exercice n°9

Créez un test unitaire pour la fonction qui renvoi le résultat du template Jinja.

---

### Correction de l'exercice n°9

---

## Retour sur les acquis

- Documenter du code
- Documenter un projet
- Le module argparse
- La configuration par variable d'environnement
- Template Jinja
- Les tests unitaires

---

## Introduction au CI/CD avec Gitlab-CI

---

## Exercice n°10

Automatisez l’exécution du test unitaire développé lors de l’exercice n°9 pour qu’il s’exécute à chaque commit du code sur Gitlab.

---

### Correction de l'exercice n°10

---

## Introduction aux tests qualités

---

## Exercice n°11

Ajoutez l’automatisation du test qualité au fichier .gitlab-ci.yml

---

### Correction de l'exercice n°11

---

## Exercice n°12

Dépannez et améliorez les scripts qui vous seront fournis

---

### Correction de l'exercice n°12

---

## Lecture/Ecriture de fichier JSON

---

## Lecture/Ecriture de fichier YAML

---

## Lecture/Ecriture de fichier XML

---

## Survol des modules standards Python les plus utiles

---

## Consommation de service web avec la librairie requests

---

## Exercice n°13

Avec la librairie requests, téléchargez le contenu du service web  https://jsonplaceholder.typicode.com/todos et écrivez le dans un fichier todos.json

---

### Correction de l’exercice n°13

---

## Production de service web avec le framework flask

---

## Exercice n°14

Fournissez une route avec Flask qui exposera le service web /todos et consommez ce service avec requests.

---

### Correction de l’exercice n°14

---

## Retour sur les acquis

- Le CI/CD avec Gitlab-CI
- Test qualité
- Dépanner du code Python
- Gestion de fichier JSON/YAML/XML
- Les modules standard les plus utiles

---

## La notion de Package en Python

---

## L’outil pip et le fichier requirements.txt

---

## L’installation d’un projet Python avec setup.py

---

## Exercice n°15

Ajoutez un setup.py au générateur de fichier .htaccess et modifiez, le CI/CD pour l’utiliser lors de l’installation.

---

### Correction de l’exercice n°15

---

## Analyser et comprendre un projet Python existant

- La compatibilité avec Python3
- Les dépendances
- Les bonnes pratiques
- La conformité PEP8
- Les tests automatisés
- La documentation

---

## Exercice n°16

Chaque participant va créer une nouvelle branche de son projet et introduire des bugs qui seront corrigés par un autre participant.

---

## Exécution de commandes systèmes

- subprocess
- pyinvoke

---

## Exercice n°17

A l’aide de subprocess ou de pyinvoke, afficher la liste des fichiers du répertoire courant.

---

### Correction de l’exercice n°17

---

## Les possibilités de traitements parallèles en Python

- Le multi threading
- Le multi processing
- Les coroutines
- Les micros-services

---

## Introduction au modèle objet en Python

- Les classes
- Les instances de classe
- L'héritage
- Les méthodes (fonctions)

---

## Introduction à Microsoft Azure Functions en Python

---

## Introduction aux fonctions Lambda sur AWS en Python

---

## Introduction à Ansible

---

## Jeux surprise

---

## Questions/Réponse et conclusion de la formation

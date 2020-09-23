# Exercice n°1.1

### Scénario

Un client vous demande de générer un fichier [**.htaccess**](http://httpd.apache.org/docs/current/howto/htaccess.html) pour Apache à partir d'une liste d'adresse IP qu'il vous fournit dans un ticket. 

Dans un premier temps, nous allons uniquement afficher le résultat à l'écran, plus tard nous verrons comment l'écrire dans un fichier.

### Opérations à réaliser

1. Créez un script python generate-apache-rewrite.py
2. Placez les adresses IP dans un tableau
3. Bouclez sur le tableau pour afficher chaque adresse IP à l'écran avec le "Allow from" devant
4. Quand le script fonctionne, effectuez un commit sur le git avec le libellé "exo1 solution"

### Résultat attendu à l'écran

```
Order Allow, Deny
Allow from 192.168.1.10
Allow from 172.100.2.11
Deny from all
```

### Acquis

- Tableau python
- Template de chaîne de caractère
- Instruction print
- Boucle for in
- Commit git

# Exercice n°1

## Scénario

Un client vous demande de générer un fichier [htaccess](http://httpd.apache.org/docs/current/howto/htaccess.html) pour Apache à partir d'une liste d'adresse IP qu'il vous fournit dans un ticket. 

## Adresses fournies par le client

```
192.168.1.10
172.100.2.11
```

## Opérations à réaliser

1. Créez un script python generate-apache-rewrite.py
2. Placez les adresses IP dans un tableau
3. Bouclez sur le tableau pour afficher chaque adresse IP à l'écran avec le "Allow from" devant
4. Remplacez l'affichage écran par l'écriture dans un fichier htaccess.txt
5. Testez le fichier htaccess.txt sur http://www.htaccesscheck.com/
6. Quand le script fonctionne, effectuez un commit avec le libellé "exercice 1 done" et un push

## Résultat attendu

Dans le fichier htaccess.txt

```
Order Allow, Deny
Allow from 192.168.1.10
Allow from 172.100.2.11
Deny from all
```

## Les acquis

- Python list (tableau indexé)
- Boucle for dans un tableau
- Écriture dans un fichier texte
- Commit git

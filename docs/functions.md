# Les fonctions en Python

**Rappel:**
- Un module python est un fichier unique contenant du code python. Ce n'est pas obligatoire mais par convention, les fichiers Python on l'extension .py.
- Le code dans un module Python est interprété de la 1ère ligne à la dernière ligne
- L'importation d'un module dans un autre, suit les mêmes règles d'interprétation du code
- Les fonctions présentes dans un module ne sont exécutés que si elles sont appellés explicitement.

**Les fonctions permettent:**
- De mieux découper le code
- Une meilleure réutilisation
- Une plus grande lisibilité

Exemple de code sans fonction:

```python
first_name = "Alain"
last_name = "Durant"
print(f"{first_name} {last_name}")
```

Avec fonction:

```python
def merge_name(first_name, last_name):
    return f"{first_name} {last_name}"

full_name = merge_name("Alain", "Durant")
print(full_name)
```

> Le résultat est le même dans les 2 cas, mais celui avec fonction est lisible et réutilisable. 


## La pseudo fonction main

Placez ce code dans un module function1.py

```python
print(__file__)
print(__name__)

if __name__ == "__main__":
    print("Main function")
```

Exécutez le module:

```shell
$ python3 function1.py
archives/tmp1.py
__main__
```

La variable `__file__`, renvoi toujours un String avec le chemin relatif du module

La variable `__name__`, renvoi une valeur qui peut changer selon la méthode d'exécution et de packaging (que nous verrons plus tard). Pour l'instant gardez à l'esprit que pour un script exécutable, il faudra toujours utiliser les 2 dernières lignes pour exécuter du code.




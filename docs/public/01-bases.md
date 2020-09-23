# Les bases du langage

## Python en ligne de commande

```shell
$ python -V
Python 3.8.2

$ python -c "print('Hello LBN')"
Hello LBN

$ python -m http.server -d .
Serving HTTP on 0.0.0.0 port 8000 (http://0.0.0.0:8000/) ...
```

## Le shell Python

```shell
$ python3
```

```python
>>> "Hello LBN"
'Hello LBN'

>>> exit()
```

## Les types de base

```python
>>> my_string = "mystring"
>>> my_integer = 123
>>> my_float = 1.2
>>> my_bool = True
>>> my_list = [1, -2, "a", "b"]
>>> my_dict = {"key1": "value1", "key2": 2}
```

> Python, n'est pas un language *typé*, c'est à dire qu'il n'est pas nécessaire de déclarer le type de variable avant son utilisation.

## Variables & Constantes


```python
>>> my_var = 10
>>> my_var += 10
>>> print(my_var)
20

>>> MY_VAR = 10
# L'instruction suivante ne devrait pas fonctionné si c'était une vraie constante
>>> MY_VAR += 10
>>> print(MY_VAR)
20
```

En réalité, il n'existe pas de *constante* en Python mais par convention, elles sont déclarées en MAJUSCULE. Comme vous le voyez, le résultat est le même qu'avec une variable.

> Vous aurez remarqués que les noms de variables sont sensibles à la casse !

## Formatage des chaines

```python
>>> last_name = "DURANT"
>>> first_name = "Alain"

>>> first_name + " " + last_name
'Alain DURANT'

>>> "{} {}".format(first_name, last_name)
'Alain DURANT'

>>> "%s %s" % (first_name, last_name)
'Alain DURANT'

>>> "%(first_name)s %(last_name)s" % {"first_name": first_name, "last_name": last_name}
'Alain DURANT'
```

**f-string:**

Les f-string sont la nouvelle méthode recommandée pour obtenir un code
plus lisible. [Documentation de f-string](https://docs.python.org/fr/3/tutorial/inputoutput.html#formatted-string-literals)

```python
>>> f"{first_name} {last_name}"
'Alain DURANT'

>>> full_name = f"{first_name} {last_name}"
>>> full_name
'Alain DURANT'
```

**Simple quote et Double quote:**

```python
>>> f'{first_name} {last_name}'
'Alain DURANT'
```

**Caractère d'échapement dans les chaînes:**

```python
>>> f"\"{first_name} {last_name}\""
'"Alain DURANT"'
```

## Manipulation de chaines

```python
# Transforme une chaine en tableau (séparateur espace par défaut)
>>> "Un Deux Trois".split()
['Un', 'Deux', 'Trois']

# Même chose avec séparateur ","
>>> "Un,Deux,Trois".split(",")
['Un', 'Deux', 'Trois']

# Supprime les caractères inutiles en début et fin de chaine
>>> " Ma phrase ".strip()
'Ma phrase'
```

## Calcul avec les types numériques

```python
>>> a = 1
>>> a += 1
>>> a
2

>>> a -= 1
>>> a
1

>>> a = a + 1
>>> a
2

>>> multiplicator = 10
>>> a * multiplicator
20

>>> a
2
```

## Le type None

None est une valeur null. Vous pouvez l'utilisez par exemple, pour vérifier si un champs à bien été remplit dans un formulaire.

```python
>>> a = None
>>> a is None
True

>>> a = "abcd"
>>> a is None
False
```

## Le type Boolean

```python
>>> a = True
>>> a is True
True

>>> b = False
>>> b == a
False
```

## Le tableau indexé (list/tuple)

Les tableaux sont très utilisés en Python et les exemples suivants sont les plus fréquents.

```python
>>> a = [1, 2, 3]
>>> a.append(4)
>>> a
[1, 2, 3, 4]

# Renvoi la position de la valeur 2
>>> a.index(2)
1

# Elément à la position 1
>>> a[1]
2

# Dernier éléments
>>> a[-1]

>>> len(a)
4

>>> a.reverse()
>>> a
[4, 3, 2, 1]

>>> a.sort()
>>> a
[1, 2, 3, 4]

>>> a.pop()
4
>>> a.pop()
3
>>> a
[1, 2]

>>> a.insert(0, 10)
>>> a
[10, 1, 2, 3]

>>> a = [1, 2, 3]
>>> type(a)
<class 'list'>

# Transforme un tableau de chaines en une chaine
>>> a = ["A", "l", "a", "i", "n"]
>>> a
['A', 'l', 'a', 'i', 'n']
>>> "".join(a)
'Alain'

# Transforme un mot ou une chaine en tableau
>>> list("Alain")
['A', 'l', 'a', 'i', 'n']
```

### Les tuple

Un tuple est identique à un type **list** à la différence qu'il se déclare avec () au lieu de [] et n'est pas modifiable

```
>>> a = (1, 2, 3)

# La méthode d'ajout d'un élément au tableau n'existe pas dans un tuple
>>> a.append(4)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
AttributeError: 'tuple' object has no attribute 'append'

# Transformation d'un type list en tuple
>>> a = [1, 2, 3]
>>> tuple(a)
```

> Les tuples sont plus rapides et moins couteux en mémoire que les **list** mais ils ne répondent pas toujours à vos besoins.


## Le tableau associatif (dict)

```python

```

## Python et l’indentation

Jusqu'à maintenant, l'identation du code n'était pas nécessaire car nous n'avons pas utilisé d'instruction sur plusieurs ligne comme les boucles ou les conditions.

Python est particulièrement dépendant de l'indentation pour exécuter son code.

L'indentation se définit par lot de 4 espaces.

**Exemple:**

```python
a = 1
b = 2
if a >= 1:
    print("OK")
    if b < 10:
        print("OK2")
```

## La boucle for

La boucle **for** parcours les éléments d'une liste et continue jusqu'à la fin de la liste.

```python
>>> my_list = [3, 1, 10]

>>> for i in my_list:
...     print(i)
...
3
1
10

>>> my_list = [1, 2, "a", "b"]

# Vous pouvez aussi le faire sur une ligne
>>> for l in my_list: print(l)
```

## La boucle while

## Conditions if/elif/else

```python

```



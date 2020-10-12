# Configuration dynamique à l’aide des variables d’environnement

```python
import os

HOST=os.environ.get("HOST", "1.1.1.1")
PORT=int(os.environ.get("PORT", 8080))

print("%s:%s" % (HOST, PORT))
```

```shell
python tp_environ.py
1.1.1.1:8080

HOST=2.2.2.2 python tp_environ.py
2.2.2.2:8080
```

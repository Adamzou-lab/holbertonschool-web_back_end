# Python Async Function

## Description

Ce projet explore la programmation asynchrone en Python avec le module `asyncio`. Il couvre la création de coroutines, l'exécution concurrente de tâches et la mesure des performances.

## Fichiers

**0-basic_async_syntax.py**
Coroutine `wait_random` qui attend un délai aléatoire entre 0 et `max_delay` secondes et retourne ce délai.

**1-concurrent_coroutines.py**
Coroutine `wait_n` qui exécute `wait_random` n fois en parallèle et retourne la liste des délais en ordre croissant.

**2-measure_runtime.py**
Fonction `measure_time` qui mesure le temps d'exécution total de `wait_n` et retourne le temps moyen par appel.

**3-tasks.py**
Fonction `task_wait_random` qui crée et retourne un objet `asyncio.Task` pour `wait_random`.

**4-tasks.py**
Coroutine `task_wait_n` similaire à `wait_n` mais utilisant `task_wait_random` pour créer les tâches.

## Concepts abordés

- Syntaxe `async` / `await`
- `asyncio.gather` pour l'exécution concurrente
- `asyncio.Task` pour la gestion des tâches
- Mesure du temps d'exécution avec `time.perf_counter`

## Utilisation

```python
import asyncio
from 1-concurrent_coroutines import wait_n

print(asyncio.run(wait_n(5, 10)))
```

## Auteur

Adam Zouaoui 

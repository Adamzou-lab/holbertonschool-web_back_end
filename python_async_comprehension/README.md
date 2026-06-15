# Python Async Comprehension

## Description

Ce projet explore les générateurs asynchrones, les compréhensions asynchrones et l'exécution parallèle de coroutines en Python avec le module `asyncio`.

## Fichiers

**0-async_generator.py**
Coroutine `async_generator` qui boucle 10 fois, attend 1 seconde à chaque itération, puis génère un nombre aléatoire entre 0 et 10.

**1-async_comprehension.py**
Coroutine `async_comprehension` qui collecte 10 nombres aléatoires en utilisant une compréhension asynchrone sur `async_generator`.

**2-measure_runtime.py**
Coroutine `measure_runtime` qui exécute `async_comprehension` 4 fois en parallèle avec `asyncio.gather` et retourne le temps total d'exécution. Le résultat est environ 10 secondes car les 4 coroutines s'exécutent en parallèle sur le même event loop.

## Concepts abordés

- Générateurs asynchrones avec `async def` et `yield`
- Boucle `async for` pour itérer sur un générateur asynchrone
- Compréhensions asynchrones
- Exécution parallèle avec `asyncio.gather`
- Mesure du temps d'exécution avec `time.perf_counter`

## Auteur

Adam Zouaoui

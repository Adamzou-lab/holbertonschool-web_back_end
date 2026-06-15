# Python Async Comprehension

## Description

Ce projet explore les générateurs asynchrones et les compréhensions asynchrones en Python avec le module `asyncio`.

## Fichiers

**0-async_generator.py**
Coroutine `async_generator` qui boucle 10 fois, attend 1 seconde à chaque itération, puis génère un nombre aléatoire entre 0 et 10.

## Concepts abordés

- Générateurs asynchrones avec `async def` et `yield`
- Boucle `async for` pour itérer sur un générateur asynchrone
- Compréhensions asynchrones

## Utilisation

```python
import asyncio
from 0-async_generator import async_generator

async def main():
    result = []
    async for i in async_generator():
        result.append(i)
    print(result)

asyncio.run(main())
```

## Auteur

Adam Zouaoui

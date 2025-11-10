---
title: "Introducción a la Mecánica Cuántica: Ejemplo Práctico"
date: 2024-01-15
categories: [cuantica, calculos]
---

# La Ecuación de Schrödinger

La ecuación de Schrödinger independiente del tiempo:

$$-\frac{\hbar^2}{2m}\nabla^2\psi + V\psi = E\psi$$

## Ejemplo: Partícula en una Caja

Para una partícula en una caja unidimensional:

```python
# Cálculo de energías permitidas
import numpy as np

hbar = 1.0545718e-34  # J·s
m = 9.109e-31         # kg (electrón)
L = 1e-9              # m (1 nm)

def energia(n):
    return (n**2 * np.pi**2 * hbar**2) / (2 * m * L**2)

print(f"E1 = {energia(1):.2e} J")

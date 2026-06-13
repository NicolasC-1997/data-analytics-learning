# Notas Día 5 — Transformación de Datos y Feature Engineering

## Conceptos aprendidos
- `apply()`: ejecuta una función sobre cada elemento de una Serie
- `map()`: reemplaza valores usando un diccionario de mapeo
- `lambda`: función anónima de una línea, usada dentro de apply()
- Feature Engineering: crear nuevas variables a partir de las existentes

## Funciones clave
| Función | Uso |
|---------|-----|
| `df['col'].apply(func)` | Transformación con lógica personalizada |
| `df['col'].map({dict})` | Recodificación de categorías |
| `df['col'].idxmax()` | Índice del valor máximo (responder "¿cuál?") |
| `pd.cut()` | Segmentación en rangos |

## Errores cometidos hoy
1. Etiquetas distintas al enunciado → respetar el contrato de datos
2. Espacios/tildes en etiquetas → usar snake_case sin tildes
3. Conclusión causal sin datos → correlación ≠ causalidad
4. No usar idxmax() para responder "¿cuál tiene más?"
5. Confundir la variable analizada con la conclusión

## Regla de oro aprendida
> Una conclusión analítica debe responder exactamente la pregunta planteada,
> con el número concreto, sin afirmar causas que no están demostradas en los datos.

## Variables nuevas creadas en el dataset Titanic
- `nivel_tarifa`: segmentación por precio del ticket
- `tam_familiar`: tamaño del grupo familiar
- `tipo_viajero`: solo / grupo_pequeño / grupo_grande
- `titulo`: extraído del nombre con apply() + lambda
- `clase_nombre`: recodificación de Pclass con map()

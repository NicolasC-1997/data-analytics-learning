# Día 2 — Selección y Filtrado de Datos con Pandas

## Objetivo de la sesión

Aprender a seleccionar columnas, acceder a filas y filtrar información utilizando Pandas para responder preguntas de negocio sobre un dataset.

---

## Conceptos clave

### Selección de columnas

```python
df['Age']
```

Retorna una **Series**.

```python
df[['Name', 'Age']]
```

Retorna un **DataFrame**.

### Regla importante

* Un corchete → Series.
* Doble corchete → DataFrame.

---

## Selección de filas

### `.loc`

Basado en etiquetas.

```python
df.loc[0]
df.loc[0, 'Name']
```

### `.iloc`

Basado en posiciones.

```python
df.iloc[0]
df.iloc[0, 3]
```

### Diferencia importante

```python
df.loc[0:4]
```

Incluye la fila 4.

```python
df.iloc[0:5]
```

No incluye la posición 5.

---

## Filtrado condicional

### Una condición

```python
df[df['Age'] > 30]
df[df['Sex'] == 'female']
```

### Múltiples condiciones

AND:

```python
df[(df['Sex'] == 'female') & (df['Survived'] == 1)]
```

OR:

```python
df[(df['Pclass'] == 1) | (df['Pclass'] == 2)]
```

NOT:

```python
df[~(df['Survived'] == 1)]
```

---

## Métodos útiles

### `.isin()`

```python
df[df['Pclass'].isin([1, 2])]
```

Permite filtrar por múltiples valores.

### `.between()`

```python
df[df['Age'].between(18, 35)]
```

Permite filtrar por rangos.

---

## Mostrar resultados

### Contar registros

```python
len(resultado)
```

o

```python
resultado.shape[0]
```

### Mostrar resultados formateados

```python
print(f"Mujeres a bordo: {len(mujeres)}")
```

### Mostrar primeras filas

```python
print(resultado.head())
```

---

## Ejercicios realizados

### Pregunta 1

¿Cuántas mujeres había a bordo?

Resultado:

* 314 mujeres.

Aprendizaje:

Mi primer filtro contaba mujeres sobrevivientes y no todas las mujeres. Debo leer cuidadosamente la pregunta antes de construir el filtro.

### Pregunta 2

Edad promedio de pasajeros de primera clase.

Resultado:

* Aproximadamente 38.2 años.

Interpretación:

Los pasajeros de primera clase eran, en promedio, mayores que el resto de pasajeros.

### Pregunta 3

¿Cuántos menores de 18 años sobrevivieron?

Resultado:

* 32 pasajeros.

Aprendizaje:

Inicialmente utilicé `> 18` cuando la pregunta requería `< 18`.

### Pregunta 4

Top 5 pasajeros de primera clase que pagaron la tarifa más alta.

Conceptos utilizados:

* Filtrado.
* Selección de columnas.
* Ordenamiento con `sort_values()`.
* Limitación con `head()`.

### Pregunta 5

Porcentaje de supervivencia de mujeres en primera clase.

Resultado:

* Aproximadamente 96.8%.

Interpretación:

Las mujeres de primera clase tuvieron una probabilidad extremadamente alta de sobrevivir.

---

## Errores corregidos

### Error 1

Confundir:

```python
df[(df['Sex'] == 'female')]
```

con

```python
df[(df['Sex'] == 'female') & (df['Survived'] == 1)]
```

La segunda consulta responde una pregunta distinta.

### Error 2

Usar:

```python
Age > 18
```

cuando la pregunta solicitaba:

```python
Age < 18
```

Pequeños cambios en operadores pueden alterar completamente el resultado del análisis.

---

## Aprendizaje más importante del día

La mayoría de las preguntas de negocio siguen el mismo patrón:

```python
# 1. Filtrar
subconjunto = df[condicion]

# 2. Analizar
subconjunto['columna'].operacion()
```

Este patrón aparece constantemente en proyectos reales de análisis de datos.

---

## Próximo paso

Día 3: Agrupaciones con `groupby()`, análisis por categorías y primeras métricas comparativas de negocio.


# Día 3 — Agrupación y Agregación con .groupby()

## Conceptos aprendidos

### El patrón Split → Apply → Combine
groupby() divide el DataFrame por categoría, aplica una función a cada grupo
y combina los resultados en un nuevo objeto.

### Sintaxis básica
```python
df.groupby('columna')['columna_objetivo'].función()
```

### Funciones de agregación principales
| Función | Uso |
|---|---|
| .mean() | Promedio |
| .sum() | Suma |
| .count() | Cantidad (ignora nulos) |
| .size() | Cantidad (incluye nulos) |
| .min() / .max() | Extremos |
| .median() | Mediana |
| .agg({}) | Múltiples funciones |

### Agrupar por múltiples columnas
```python
df.groupby(['col1', 'col2'])['objetivo'].mean()
```
Produce un MultiIndex. Usar reset_index() para aplanar.

### reset_index()
Convierte el índice de agrupación en columna normal.
Imprescindible cuando queremos seguir manipulando el resultado como DataFrame.

### value_counts()
Atajo para contar valores únicos en una columna categórica.
Equivale a groupby + count pero más directo.

## Patrones profesionales

- Survived es 0/1, por eso mean() = porcentaje de supervivencia.
  Este patrón aplica a cualquier variable binaria (fraude, conversión, churn).
- Siempre anclar conclusiones en números: en vez de "la mayoría sobrevivió",
  escribir "el 62% de los pasajeros de primera clase sobrevivió".
- Después de un groupby importante, identificar el máximo/mínimo con idxmax().

## Errores a recordar
- No hay errores técnicos en esta sesión.
- Área de mejora: comunicar hallazgos con cifras concretas, no solo con
  descripciones cualitativas.

## Código de referencia
```python
# Agrupación básica
df.groupby('Pclass')['Survived'].mean()

# Múltiples métricas
df.groupby('Sex').agg(
    edad_promedio=('Age', 'mean'),
    tarifa_promedio=('Fare', 'mean'),
    cantidad=('PassengerId', 'count')
)

# Resultado como DataFrame limpio
resultado = df.groupby('Embarked')['Survived'].mean().reset_index()
resultado.columns = ['Puerto', 'Tasa']
resultado['Tasa_Pct'] = (resultado['Tasa'] * 100).round(1)

# Identificar el máximo
puerto_max = resultado.loc[resultado['Tasa'].idxmax(), 'Puerto']
```

## Progreso acumulado
- Día 1: Fundamentos de Pandas — Series, DataFrame, lectura de CSV, inspección
- Día 2: Selección, filtrado con condiciones simples y múltiples
- Día 3: groupby, agg, value_counts, reset_index
- Dominio estimado de Pandas fundamentals: ~50%

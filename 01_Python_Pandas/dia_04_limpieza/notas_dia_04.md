# Día 4 — Limpieza de Datos

## Conceptos clave

- Limpieza de datos = 60-80% del trabajo real de un analista
- Tres problemas principales: valores nulos, duplicados, tipos incorrectos
- Antes de imputar: preguntar **por qué** falta el dato

## Funciones aprendidas

| Función | Uso |
|---|---|
| `df.isnull().sum()` | Contar nulos por columna |
| `(df.isnull().sum() / len(df) * 100).round(2)` | Porcentaje de nulos |
| `df['col'].fillna(valor)` | Rellenar nulos con un valor |
| `df.drop(columns=['col'])` | Eliminar columna |
| `df.drop_duplicates()` | Eliminar filas duplicadas |
| `df.duplicated().sum()` | Contar duplicados |
| `df['col'].astype(tipo)` | Cambiar tipo de dato |
| `pd.cut(col, bins, labels)` | Segmentar en rangos |

## Estrategias de imputación

- **Numérica con outliers** → mediana (más robusta)
- **Numérica sin outliers** → media o mediana
- **Categórica** → moda (valor más frecuente)
- **Cuando falta = ausencia real** → imputar con 0 o valor de negocio

## Errores corregidos hoy

1. **Usar variable antes de crearla:** usé `df_limpio` sin haberlo definido primero.
   Corrección: siempre hacer `df_limpio = df.copy()` antes de modificar.

2. **Elegir media sin analizar distribución:** en delay_minutes de aerolínea,
   los retrasos son asimétricos → la mediana es más representativa.
   
3. **Imputar sin preguntar el origen del nulo:** si delay_minutes falta
   porque el vuelo llegó a tiempo → imputar con 0, no con el promedio.

## Concepto nuevo: distribución sesgada

Cuando una variable tiene outliers en un extremo (retrasos, salarios, tarifas),
la media sube artificialmente. La mediana representa mejor al "caso típico".

## pd.cut() — segmentación por rangos

```python
df['RangoPrecio'] = pd.cut(
    df['Fare'],
    bins=[0, 20, 100, float('inf')],
    labels=['Bajo', 'Medio', 'Alto'],
    include_lowest=True
)
```

Muy usada para: segmentar clientes, rangos de riesgo, categorías de precio.

## Próximo tema

Día 5 — Estadística descriptiva: media, mediana, moda, desviación estándar,
distribuciones, y cómo interpretar datos en contexto de negocio.

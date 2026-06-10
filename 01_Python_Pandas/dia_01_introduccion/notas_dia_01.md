# Día 1 — Introducción al Data Analytics

## Objetivo de la sesión

Comprender los fundamentos del Data Analytics, el flujo de trabajo de un analista de datos y realizar una primera exploración de un dataset utilizando Pandas.

---

## Conceptos clave

### ¿Qué es Data Analytics?

Proceso de recopilar, limpiar, transformar, analizar e interpretar datos para apoyar la toma de decisiones basada en evidencia.

### Tipos de análisis

* **Descriptivo:** ¿Qué ocurrió?
* **Diagnóstico:** ¿Por qué ocurrió?
* **Predictivo:** ¿Qué podría ocurrir?
* **Prescriptivo:** ¿Qué debería hacerse?

### Flujo de trabajo de un Data Analyst

1. Definir el problema.
2. Obtener los datos.
3. Limpiar los datos.
4. Realizar análisis exploratorio (EDA).
5. Visualizar y comunicar hallazgos.
6. Apoyar la toma de decisiones.

### Conceptos fundamentales

* **Dataset:** colección estructurada de datos.
* **Variable:** característica medida en cada observación.
* **Valor nulo:** dato faltante.
* **EDA (Exploratory Data Analysis):** exploración inicial para comprender un dataset.
* **KPI (Key Performance Indicator):** indicador clave de desempeño.
* **ETL (Extract, Transform, Load):** proceso de extracción, transformación y carga de datos.

---

## Pandas: primeros pasos

### Comandos aprendidos

```python
pd.read_csv()
df.head()
df.tail()
df.shape
df.info()
df.describe()
df.dtypes
df.isnull().sum()
```

### Utilidad de cada comando

| Comando          | Propósito                           |
| ---------------- | ----------------------------------- |
| `read_csv()`     | Cargar datos desde un archivo CSV   |
| `head()`         | Visualizar las primeras filas       |
| `tail()`         | Visualizar las últimas filas        |
| `shape`          | Obtener dimensiones del dataset     |
| `info()`         | Revisar estructura y tipos de datos |
| `describe()`     | Obtener estadísticas descriptivas   |
| `dtypes`         | Ver tipos de datos por columna      |
| `isnull().sum()` | Detectar valores faltantes          |

---

## Dataset utilizado

### Titanic Dataset

Fuente utilizada para practicar exploración básica de datos.

### Dimensiones

* Filas: 891
* Columnas: 12

### Valores nulos detectados

| Columna  | % Nulos |
| -------- | ------- |
| Age      | 19.87%  |
| Cabin    | 77.10%  |
| Embarked | 0.22%   |

### Estadísticas relevantes

**Edad (Age)**

* Media: ~29.7 años
* Mediana: 28.0 años

**Tarifa (Fare)**

* Mínimo: 0
* Máximo: 512.33
* Mediana: ~14.45

Observación:

La diferencia entre media y mediana indica una distribución asimétrica. Un grupo reducido de pasajeros pagó tarifas muy elevadas, lo que incrementa la media.

---

## Errores corregidos y aprendizajes

### Diferencia entre media, mediana y midrange

Error inicial:

Confundir la mediana con el punto medio entre el valor mínimo y máximo.

Corrección:

* **Media:** promedio de todos los valores.
* **Mediana:** valor central al ordenar los datos.
* **Midrange:** (máximo + mínimo) / 2.

El midrange casi no se utiliza en análisis profesional debido a su sensibilidad a valores extremos.

---

## Reflexión personal

Durante esta sesión comprendí que el trabajo de un Data Analyst no consiste únicamente en programar o crear gráficos, sino en transformar datos en información útil para la toma de decisiones. También aprendí la importancia de explorar un dataset antes de comenzar cualquier análisis y comprendí mejor la diferencia entre media y mediana, un concepto fundamental para futuras unidades de estadística.

---

## Próximo paso

Día 2: Selección y filtrado de datos con Pandas, primeras preguntas de negocio y profundización en el análisis exploratorio de datos.

# 📊 Data Analytics Learning — Programa de 90 días

> Repositorio de aprendizaje estructurado en Data Analytics, Business Intelligence y preparación para Machine Learning.  
> **Estudiante:** Ingeniería Informática · **Meta:** nivel Junior Data Analyst profesional.

---

## 🎯 Objetivo del programa

Desarrollar competencias técnicas y analíticas desde un nivel intermedio de programación hasta un perfil profesional junior en Data Analytics, construyendo un portafolio real con proyectos sobre datos reales.

**Duración:** 90 días · **Dedicación:** ~1 hora diaria  
**Stack tecnológico:** Python · Pandas · NumPy · SQL · Power BI · Matplotlib · Seaborn · Jupyter / Google Colab

---

## 📁 Estructura del repositorio

```
data-analytics-learning/
│
├── 📂 01_Fundamentos/                  # Python para análisis de datos
│   ├── dia_01_intro_pandas/
│   ├── dia_02_seleccion_filtrado/
│   ├── dia_03_groupby/
│   ├── dia_04_limpieza/
│   └── dia_05_transformacion/
│
├── 📂 02_Estadistica/                  # Estadística descriptiva e inferencial
│
├── 📂 03_SQL/                          # SQL para análisis de negocio
│
├── 📂 04_Visualizacion/                # Matplotlib, Seaborn, dashboards
│
├── 📂 05_Proyectos_Guiados/            # Proyectos completos con documentación
│
├── 📂 06_Portafolio/                   # Proyectos independientes para entrevistas
│
├── 📂 datasets/
│   └── titanic.csv
│
└── README.md
```

---

## 📈 Progreso del programa

### Módulo 1 — Fundamentos de Python para Análisis de Datos

| Día | Tema | Estado | Notebook |
|-----|------|--------|----------|
| 1 | Introducción a Pandas · Exploración inicial de datasets | ✅ Completado | [dia_01](./01_Python_Pandas/dia_01_intro_pandas/) |
| 2 | Selección de columnas · `.loc` · `.iloc` · Filtrado condicional | ✅ Completado | [dia_02](./Python_Pandas/dia_02_seleccion_filtrado/) |
| 3 | Agrupaciones con `.groupby()` · `.agg()` · `value_counts()` | ✅ Completado | [dia_03](./Python_Pandas/dia_03_groupby/) |
| 4 | Limpieza de datos · Nulos · Duplicados · Tipos de datos | ✅ Completado | [dia_04](./Python_Pandas/dia_04_limpieza/) |
| 5 | Transformación · `apply()` · `map()` · Feature Engineering | ✅ Completado | [dia_05](./Python_Pandas/dia_05_transformacion/) |
| 6–10 | EDA · Estadística descriptiva · Primeras visualizaciones | 🔜 Próximamente | — |

### Módulos siguientes

| Módulo | Contenido | Estado |
|--------|-----------|--------|
| 2 — Estadística | Descriptiva · Inferencial · Probabilidad | 🔜 Próximamente |
| 3 — SQL | Consultas · JOINs · Análisis de negocio | 🔜 Próximamente |
| 4 — Visualización | Matplotlib · Seaborn · Storytelling | 🔜 Próximamente |
| 5 — Business Intelligence | Power BI · Dashboards · KPIs | 🔜 Próximamente |
| 6 — Proyectos | Análisis completos end-to-end | 🔜 Próximamente |

---

## 🛠️ Habilidades desarrolladas

### Completadas
- Exploración inicial de datasets con Pandas (`shape`, `dtypes`, `describe`, `info`)
- Selección de filas y columnas con `.loc` e `.iloc`
- Filtrado condicional con operadores booleanos (`&`, `|`, `~`)
- Agrupaciones y agregaciones con `.groupby()` y `.agg()`
- Detección y tratamiento de valores nulos (`isnull`, `fillna`, `dropna`)
- Eliminación de duplicados (`drop_duplicates`)
- Corrección de tipos de datos (`astype`, `pd.cut`)
- Transformación de columnas con `apply()` y funciones personalizadas
- Recodificación de categorías con `map()`
- Creación de nuevas variables (Feature Engineering básico)
- Extracción de información desde texto con `lambda`

### En desarrollo
- Análisis Exploratorio de Datos (EDA)
- Estadística descriptiva aplicada
- Visualización con Matplotlib y Seaborn

---

## 📊 Dataset principal

**Titanic — Kaggle**  
Dataset clásico de análisis de datos con información de 891 pasajeros: edad, género, clase, tarifa, puerto de embarque y supervivencia.

Columnas trabajadas: `Survived`, `Pclass`, `Name`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`, `Cabin`  
Variables creadas: `grupo_edad`, `tam_familiar`, `tipo_viajero`, `titulo`, `clase_nombre`, `nivel_tarifa`, `categoria_tarifa`

---

## 🗂️ Estructura de cada sesión

Cada carpeta de día contiene:

```
dia_XX_tema/
├── dia_XX_tema.ipynb     # Notebook con código y análisis
└── notas_diaXX.md        # Resumen de conceptos, errores y aprendizajes
```

---

## 🚀 Proyectos (próximamente)

Los proyectos completos se publicarán en `05_Proyectos/` con:

- Definición del problema de negocio
- Exploración y limpieza del dataset
- Análisis exploratorio completo
- Visualizaciones
- Hallazgos y conclusiones
- README individual por proyecto

---

## 👤 Sobre este repositorio

Programa de mentoría personalizada estructurado en 90 días.  
Cada sesión incluye teoría, práctica, corrección de errores y construcción progresiva de portafolio.


---

*Última actualización: Día 5 de 90 completado — Módulo: Fundamentos de Python para Análisis de Datos*


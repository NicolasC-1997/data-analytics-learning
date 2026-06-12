# 📊 Data Analytics Learning — Programa de 90 días

> Repositorio de aprendizaje estructurado en Data Analytics, Business Intelligence y preparación para Machine Learning.  
> Estudiante: Ingeniería Informática · Meta: nivel **Junior Data Analyst** profesional.

---

## 🎯 Objetivo del programa

Desarrollar competencias técnicas y analíticas desde un nivel intermedio de programación hasta un perfil profesional junior en Data Analytics, construyendo un portafolio real con proyectos sobre datos reales.

**Duración estimada:** 90 días · ~1 hora diaria  
**Estado actual:** 🟢 En progreso — Día 4 de 90

---

## 🛠️ Stack tecnológico

| Categoría | Herramientas |
|---|---|
| Lenguaje | Python 3 |
| Manipulación de datos | Pandas, NumPy |
| Visualización | Matplotlib, Seaborn |
| Business Intelligence | Power BI |
| Bases de datos | SQL |
| Entorno | Google Colab, Jupyter Notebook |
| Control de versiones | Git, GitHub |

---

## 📁 Estructura del repositorio

```
data-analytics-learning/
│
├── 01_Python_Pandas/           ← Fundamentos de Python para datos y Pandas
│   ├── dia_01_introduccion/
│   ├── dia_02_seleccion_filtrado/
│   ├── dia_03_groupby/
│   └── dia_04_limpieza/
│
├── 02_SQL/                     ← SQL para análisis de negocio
│
├── 03_Visualizacion/           ← Matplotlib, Seaborn y storytelling con datos
│
├── 04_PowerBI/                 ← Dashboards y Business Intelligence
│
├── 05_Proyectos/               ← Proyectos guiados completos con datasets reales
│
├── 06_Portafolio/              ← Proyectos seleccionados para entrevistas laborales
│
├── datasets/                   ← Datasets utilizados durante el programa
│   └── titanic.csv
│
└── README.md
```

---

## 📚 Contenidos por módulo

### 01 · Python & Pandas
Fundamentos de manipulación de datos con Python y la librería Pandas, usando datasets reales.

| Día | Tema | Conceptos clave |
|-----|------|----------------|
| 01 | Introducción al Data Analytics | Tipos de análisis, flujo de 6 fases, Series, DataFrame, `read_csv`, `head/tail/info/describe` |
| 02 | Selección y filtrado | Selección de columnas/filas, `.loc`, `.iloc`, filtros booleanos, operadores `&` `\|` `~` |
| 03 | Agrupación y agregación | `.groupby()`, `.agg()`, `.value_counts()`, `reset_index()`, MultiIndex |
| 04 | Limpieza de datos | `isnull`, `fillna`, `dropna`, `drop_duplicates`, `astype`, `pd.cut` |
| 05 | *(próximamente)* Estadística descriptiva | Media, mediana, desviación estándar, distribuciones |

### 02 · SQL *(próximamente)*
Consultas para responder preguntas de negocio. SELECT, WHERE, GROUP BY, JOINs, subconsultas y funciones de ventana.

### 03 · Visualización *(próximamente)*
Matplotlib y Seaborn para crear visualizaciones efectivas. Principios de storytelling con datos.

### 04 · Power BI *(próximamente)*
Construcción de dashboards interactivos. KPIs, segmentaciones, DAX básico.

### 05 · Proyectos guiados *(próximamente)*
Análisis completos sobre datasets reales con documentación profesional.

### 06 · Portafolio *(en construcción)*
Proyectos seleccionados listos para presentar en entrevistas laborales.

---

## 🔬 Dataset principal — Titanic

El dataset `titanic.csv` es el conjunto de datos principal de la fase inicial del programa.

| Característica | Valor |
|---|---|
| Filas | 891 |
| Columnas | 12 |
| Fuente | [datasciencedojo/datasets](https://github.com/datasciencedojo/datasets) |
| Variables clave | `Survived`, `Pclass`, `Age`, `Fare`, `Sex`, `Embarked` |

Usado para practicar: exploración, filtrado, agrupaciones, limpieza de datos y estadística descriptiva.

---

## 📈 Progreso del programa

```
Módulo 1 — Python & Pandas     ████░░░░░░░░░░░░  ~25% (4/16 sesiones estimadas)
Módulo 2 — SQL                 ░░░░░░░░░░░░░░░░   0%
Módulo 3 — Visualización       ░░░░░░░░░░░░░░░░   0%
Módulo 4 — Power BI            ░░░░░░░░░░░░░░░░   0%
Proyectos guiados              ░░░░░░░░░░░░░░░░   0%
─────────────────────────────────────────────────
Progreso total del programa    █░░░░░░░░░░░░░░░  ~4% (Día 4/90)
```

---

## 🏆 Competencias en desarrollo

- [x] Exploración de datasets con Pandas
- [x] Selección y filtrado de datos
- [x] Agrupación y análisis por segmentos
- [x] Limpieza de datos (nulos, duplicados, tipos)
- [ ] Estadística descriptiva e inferencial
- [ ] Visualización con Matplotlib y Seaborn
- [ ] SQL para análisis de negocio
- [ ] Dashboards en Power BI
- [ ] Análisis Exploratorio de Datos (EDA) completo
- [ ] Storytelling con datos
- [ ] Machine Learning introductorio

---

## 🗂️ Cómo navegar este repositorio

Cada carpeta de sesión contiene:

- `dia_XX_tema.ipynb` — notebook ejecutable en Google Colab con teoría y ejercicios
- `notas_diaXX.md` — resumen de conceptos, comandos aprendidos y errores corregidos

Los proyectos en `05_Proyectos/` incluyen además un `README.md` propio con definición del problema, metodología y hallazgos principales.

---

## 🚀 Ejecutar los notebooks

Todos los notebooks son compatibles con **Google Colab** y **Jupyter Notebook**.

```bash
# Clonar el repositorio
git clone https://github.com/NicolasC-1997/data-analytics-learning.git

# Abrir en Jupyter
jupyter notebook
```

O abrir directamente en Google Colab haciendo clic en el badge de cada notebook.

---

## 📄 Licencia

MIT License — ver archivo `LICENSE` para más detalles.

---

*Repositorio en construcción activa · Actualizado diariamente durante el programa de 90 días.*

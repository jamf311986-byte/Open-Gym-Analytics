# Open Gym Analytics

## Objetivo

Analizar patrones de uso de espacios deportivos comunitarios para identificar actividades, horarios y centros con mayor utilización.

## Dataset

El dataset contiene **28.038 registros y 16 variables** relacionadas con horarios, asistencia, actividades y centros comunitarios.

La variable `total_asistentes` acumula **171.413 asistentes registrados**.

## Proceso

1. Exploración inicial de los datos.
2. Estandarización de nombres de columnas.
3. Conversión de tipos de datos.
4. Revisión de valores faltantes.
5. Creación de variables derivadas de fecha y hora.
6. Análisis exploratorio con Python.
7. Desarrollo de dashboard interactivo en Power BI.

## Métricas

El proyecto diferencia dos conceptos:

- **Registros:** cantidad de filas del dataset.
- **Asistentes:** suma de `total_asistentes`.

Esta distinción es importante porque algunas visualizaciones del dashboard de Power BI utilizan el **recuento de registros**, mientras que el análisis en Python también calcula la suma de asistentes.

## Hallazgos principales

- Basketball es la actividad con más registros (8.971), seguida por Open Gym (7.643).
- Por suma de `total_asistentes`, Pickleball y Badminton presentan los mayores volúmenes acumulados.
- Las horas con mayor volumen acumulado de asistentes son 22:00, 13:00 y 14:00.
- BPCC presenta el mayor volumen acumulado de asistentes entre los centros comunitarios.
- La distribución registrada por género muestra una mayor participación acumulada de hombres que de mujeres.

## Herramientas

- Python
- Pandas
- Matplotlib
- Jupyter Notebook
- Power BI
- Power Query
- Excel

## Estructura

```text
Open-Gym-Analytics/
├── data/
│   ├── raw/
│   │   └── open-gym.xlsx
│   └── processed/
│       └── open-gym-clean.csv
├── notebooks/
│   └── open_gym_analysis.ipynb
├── powerbi/
│   └── OPEN GYM.pbix
├── images/
│   ├── dashboard.png
│   ├── dashboard1.png
│   └── dashboard2.png
├── README.md
└── .gitignore
```

# ⚡ Análisis de Energía Eléctrica en España

## Descripción general
Este proyecto realiza un **análisis exploratorio de los datos de la CNMC** sobre la evolución anual de la energía eléctrica generada a partir de **fuentes renovables, cogeneración y residuos**, así como la **energía vendida y la potencia instalada por comunidad autónoma**.

El propósito de este análisis es **identificar tendencias, comparar regiones y generar insights accionables** que puedan **respaldar la planificación de infraestructuras y la toma de decisiones estratégicas en energías renovables**.

--------

## Objetivos del análisis

A lo largo del análisis se abordarán los siguientes objetivos:

- 📈 **Evolución temporal de la energía generada y potencia instalada**:  
  Estudiar cómo han cambiado año a año los valores de energía vendida y potencia instalada a nivel nacional y regional, identificando **tendencias y picos significativos**.

- 🌍 **Comparación del desempeño de las comunidades autónomas**:  
  Evaluar la contribución de cada comunidad autónoma a la generación total y detectar **líderes y rezagados** en distintas tecnologías.

- ⚡ **Desglose de la generación por tecnología**:  
  Analizar la participación de cada fuente de energía (**eólica, solar, biomasa, residuos, cogeneración, hidráulica**) en el mix energético, así como su evolución a lo largo del tiempo.

- 📊 **Evaluación de eficiencia y rendimiento**:  
  Relacionar la energía generada con la potencia instalada para identificar regiones o tecnologías más **eficientes y con mayor rendimiento**.

- 🔍 **Detección de patrones y correlaciones**:  
  Explorar posibles relaciones entre tecnologías, regiones y años, así como la influencia de factores externos sobre la evolución de la generación.

- 🔮 **Proyecciones futuras**:  
  Estimar tendencias futuras en **energía vendida y potencia instalada** por comunidad y tecnología, destacando regiones con mayor potencial de crecimiento.

--------

## 📂 Estructura del proyecto
```
Spain_Electricity_Analysis
├── README.md
├── 📁 data
│   ├── cnmc_energy.csv           # Dataset original CNMC
│   └── cnmc_energy_cleaned.csv   # Dataset limpio y procesado
├── 📁 notebooks
│   ├── data_cleaning.ipynb            # Limpieza y preprocesamiento
│   ├── national_trends.ipynb          # Evolución nacional por año
│   ├── regional_analysis.ipynb        # Comparación por comunidad autónoma
│   └── technology_breakdown.ipynb     # Análisis por tipo de energía
├── 📁 query
│   ├── cnmc_energy.db                  # Base de datos SQLite
│   └── community_technology.sql       # Consultas SQL por comunidad y tecnología
├── 📁 reports
│   └── 📊 spain_electricity_dashboard.pbix  # Dashboard interactivo Power BI
└── 📁 images
    ├── kpis.png
    ├── national_trends.png
    ├── regional_comparison.png
    └── technology_breakdown.png
```
## 🗂 Dataset

El dataset proviene de **CNMC Data** e incluye registros anuales de **energía vendida (GWh)** y **potencia instalada (MW)** por **comunidad autónoma** y **tipo de tecnología**.

### Columnas principales

- **Año**: Año del registro.  
- **CCAA**: Comunidad autónoma en España.  
- **Tecnología**: Tipo de energía (**eólica, solar fotovoltaica, biomasa, residuos, cogeneración, hidráulica**, etc.).  
- **Energía vendida (GWh)**: Energía eléctrica vendida.  
- **Potencia instalada (MW)**: Potencia instalada.

## 🛠 Herramientas utilizadas

- **Jupyter Notebook + Python (pandas, matplotlib, seaborn,scikit-learn)**: Análisis y visualizaciones interactivas.  
- **SQL (SQLite)**: Consultas para segmentar por comunidad, tecnología y año.  
- **Power BI**: Creación de dashboards interactivos para KPIs, tendencias y comparaciones por región y tecnología.


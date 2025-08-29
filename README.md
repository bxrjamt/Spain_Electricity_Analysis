# ⚡ Análisis de Energía Eléctrica en España

## Descripción general
Este proyecto realiza un **análisis exploratorio de los datos de la CNMC** sobre la evolución anual de la energía eléctrica generada a partir de **fuentes renovables, cogeneración y residuos**, así como la **energía vendida y la potencia instalada por comunidad autónoma**.  
El propósito de este análisis es **identificar tendencias, comparar regiones y realizar predicciones** que puedan **respaldar la planificación de infraestructuras y la toma de decisiones estratégicas en energías renovables**.

--------
## Objetivos del análisis

### Evolución temporal de la energía generada y potencia instalada
- ¿Cuál ha sido la evolución anual de energía vendida a nivel nacional?  
- ¿Cómo ha cambiado la potencia instalada en cada año y por tecnología?  
- ¿Qué años presentan incrementos o caídas abruptas en la generación?  
- ¿Existen patrones de crecimiento sostenido para alguna tecnología específica?  

### Comparación del desempeño de las comunidades autónomas
- ¿Qué comunidades contribuyen más a la energía total vendida?  
- ¿Qué comunidades muestran menor crecimiento relativo en generación?  
- ¿Cómo se distribuye la potencia instalada entre las distintas regiones?  
- ¿Qué comunidades destacan por su capacidad instalada frente a energía realmente vendida?  

### Desglose de la generación por tecnología
- ¿Qué porcentaje del mix energético representa cada fuente (eólica, solar, biomasa, residuos, cogeneración, hidráulica)?  
- ¿Qué tecnologías han experimentado mayor crecimiento en la última década?  
- ¿Qué fuentes han perdido participación en el mix energético?  
- ¿Existen diferencias en la adopción de tecnologías entre comunidades autónomas?  

### Evaluación de eficiencia y rendimiento
- ¿Qué regiones convierten mejor la potencia instalada en energía vendida?  
- ¿Qué tecnologías muestran mayor rendimiento promedio?  
- ¿Existen comunidades o tecnologías con infrautilización significativa?  
- ¿Se observa un incremento de eficiencia con el tiempo en alguna fuente específica?  

### Detección de patrones y correlaciones
- ¿Se observan relaciones entre la adopción de distintas tecnologías en la misma comunidad?  
- ¿Qué combinaciones de tecnologías se repiten en regiones eficientes?  
- ¿Existen tendencias comunes entre comunidades con comportamientos similares en energía generada?  
- ¿Qué variables podrían estar correlacionadas con incrementos o caídas de generación?  

### Proyecciones futuras (modelos predictivos)
- ¿Qué comunidades tienen mayor potencial de crecimiento de energía renovable?  
- ¿Qué tecnologías muestran tendencia de expansión sostenida para los próximos años?  
- ¿Qué variables resultan más relevantes para predecir energía futura (potencia instalada, año, tipo de fuente)?  
- ¿Qué precisión alcanzan los modelos predictivos al estimar energía futura por comunidad y tecnología?  

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


## 📊 Objetivos del análisis y preguntas clave

### 1. Evolución temporal de la energía  
**Objetivo:** Analizar cómo ha variado la energía vendida y la potencia instalada a lo largo de los años.  

**Preguntas clave:**  
- 📈 ¿Cuál ha sido la tendencia general de la energía renovable vendida en España en la última década?  
- 📉 ¿Existen años con picos o caídas significativas? ¿A qué se deben?  
- ⚡ ¿Cómo ha evolucionado la potencia instalada en comparación con la energía vendida?  
- 🌱 ¿Se observa un crecimiento sostenido en la penetración de energías renovables?  

---

### 2. Comparación entre comunidades autónomas  
**Objetivo:** Evaluar las diferencias regionales en cuanto a capacidad instalada y energía vendida.  

**Preguntas clave:**  
- 🏙️ ¿Qué comunidades destacan por mayor potencia instalada de renovables?  
- ⚖️ ¿Qué regiones generan más energía en relación con su capacidad instalada?  
- 🔄 ¿Existen comunidades que dependen más de cogeneración o residuos en lugar de renovables?  
- 🚀 ¿Cuáles son las regiones con mayor crecimiento relativo en los últimos años?  

---

### 3. Distribución por fuentes de energía  
**Objetivo:** Identificar qué tipos de fuentes (renovables, cogeneración, residuos) dominan la producción energética.  

**Preguntas clave:**  
- 🌍 ¿Qué porcentaje de la energía vendida proviene de renovables frente a cogeneración y residuos?  
- ⏳ ¿Cómo ha cambiado esta distribución a lo largo del tiempo?  
- 📊 ¿Qué fuentes muestran mayor crecimiento y cuáles están estancadas o en retroceso?  
- 🗺️ ¿Existen diferencias en la diversificación de fuentes entre comunidades autónomas?  

---

### 4. Modelos de predicción con *scikit-learn*  
**Objetivo:** Construir modelos predictivos para estimar la energía futura a partir de los datos históricos.  

**Preguntas clave:**  
- 🔮 ¿Podemos predecir la energía vendida de cada comunidad autónoma para los próximos años?  
- 🧩 ¿Qué variables (potencia instalada, año, tipo de fuente) resultan más relevantes en la predicción?  
- 📐 ¿Qué precisión alcanzan modelos como *Linear Regression* o *Random Forest* al predecir la evolución energética?  
- 🌟 ¿Qué escenarios de crecimiento podemos anticipar para las renovables en España?  

---

### 5. Optimización y consultas SQL  
**Objetivo:** Aplicar consultas SQL para responder preguntas concretas sobre el dataset.  

**Preguntas clave:**  
- 🔝 ¿Qué comunidad tuvo el mayor incremento de potencia instalada en un año determinado?  
- 📅 ¿Cuál fue la media anual de energía renovable vendida en España en la última década?  
- 🥇 ¿Qué regiones superaron consistentemente la media nacional en producción de energía renovable?  
- 📊 ¿Qué tipo de fuente energética presenta mayor variabilidad entre comunidades?  




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
## Dataset

El dataset proviene de **CNMC Data** e incluye registros anuales de **energía vendida (GWh)** y **potencia instalada (MW)** por **comunidad autónoma** y **tipo de tecnología**.

### Columnas principales:

- **Año**: Año del registro.  
- **CCAA**: Comunidad autónoma en España.  
- **Tecnología**: Tipo de energía (**eólica, solar fotovoltaica, biomasa, residuos, cogeneración, hidráulica**, etc.).  
- **Energía vendida (GWh)**: Energía eléctrica vendida.  
- **Potencia instalada (MW)**: Potencia instalada.

## 🛠 Herramientas utilizadas

- **Jupyter Notebook + Python (pandas, matplotlib, seaborn,scikit-learn)**: Análisis y visualizaciones interactivas.  
- **SQL (SQLite)**: Consultas para segmentar por comunidad, tecnología y año.  
- **Power BI**: Creación de dashboards interactivos para KPIs, tendencias y comparaciones por región y tecnología.




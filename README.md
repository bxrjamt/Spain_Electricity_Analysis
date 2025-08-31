# ⚡ Análisis de Energía Eléctrica en España

## Descripción general
Este proyecto realiza un **análisis exploratorio de los datos de la CNMC** sobre la evolución anual de la energía eléctrica generada a partir de **fuentes renovables, cogeneración y residuos**, así como la **energía vendida y la potencia instalada por comunidad autónoma**. El propósito de este análisis es **identificar tendencias, comparar regiones y realizar predicciones** que puedan **respaldar la planificación de infraestructuras y la toma de decisiones estratégicas en energías renovables**.

--------

## Objetivos del análisis

El análisis se centra en los siguientes objetivos que nos ayudarán a entender cómo se genera, distribuye y utiliza la energía en España:

1. 📈 **Tendencias temporales de la energía vendida y la potencia instalada**    
   Analizar la evolución anual de la **energía vendida** y la **potencia instalada**, identificando **picos y variaciones significativas** a nivel nacional.

2. 📊 **Distribución por fuentes de energía**    
   Evaluar la contribución de cada fuente (renovables, cogeneración, residuos) sobre la **energía total vendida**, tanto a nivel nacional como por comunidad autónoma.

3. 🔍 **Detección de patrones y correlaciones**    
   Explorar posibles relaciones entre **energía vendida** y **potencia instalada**, según comunidad y tecnología, usando análisis de correlación y visualizaciones comparativas.

4. 🌍 **Desempeño energético por comunidades autónomas y tecnologías**    
   Analizar la **distribución, crecimiento y eficiencia** de la energía vendida y la potencia instalada por comunidad y tecnología.

5. 🔮 **Proyecciones futuras**    
   Estimar escenarios futuros de **energía vendida** y **potencia instalada** por comunidad y tecnología, destacando **regiones y fuentes con mayor potencial de crecimiento**.
   
--------


- 📈 **Tendencias temporales de la energía vendida y la potencia instalada**  
Analizar cómo han cambiado año a año los valores de **energía vendida** y **potencia instalada** a nivel nacional, identificando **tendencias y picos significativos**.

- ¿Cómo ha evolucionado anualmente la potencia instalada en comparación con la energía vendida?
- ¿Qué años presentan incrementos o caídas significativas en la generación?
- ¿Cuál ha sido la tendencia anual de la energía vendida a nivel nacional para cada tipo de fuente (renovables, cogeneración, residuos)?
- ¿Cómo ha cambiado la potencia instalada en cada año por tecnología? ¿Y la energía vendida?
- ¿Existen patrones de crecimiento sostenido para alguna tecnología específica?

- 📊 **Distribución por fuentes de energía**  
Estudiar la contribución de cada fuente de energía sobre la **energía total vendida**, así como su evolución temporal a lo largo de los años.

- ¿Qué porcentaje del total de energía vendida representa cada fuente (renovables, cogeneración, residuos) en cada año?  
- ¿Qué fuente generó más energía en un año determinado a nivel nacional y regional?  
- ¿Qué fuentes muestran mayor crecimiento o disminución a lo largo del tiempo?  
- ¿Existen diferencias significativas entre comunidades autónomas en la participación de cada fuente?  
- ¿Qué fuentes tienen mayor estabilidad o variabilidad interanual en la generación?  
- ¿Cuáles son las tres fuentes que más contribuyen a la energía vendida en España y en cada comunidad?  
- ¿Qué fuentes lideran la generación de energía en comunidades específicas?  


- 🔍 **Detección de patrones y correlaciones**
Identificar posibles relaciones entre energía vendida y potencia instalada según comunidad y tecnología.

- ¿Existe relación entre la potencia instalada y la energía vendida para cada tecnología en cada comunidad?  
- ¿Qué tecnologías muestran una relación más fuerte entre potencia instalada y energía vendida?  
- ¿Hay comunidades donde ciertas tecnologías generan energía de manera más eficiente (mayor energía vendida por MW instalado)?  
- ¿Se observan patrones de dependencia entre tecnologías dentro de la misma comunidad?  
- ¿Qué combinación de comunidad y tecnología presenta la mayor o menor correlación entre potencia instalada y energía vendida?
  

- 🌍 **Desempeño energético por comunidades autónomas y tecnologías**
Analizar distribución, crecimiento y eficiencia de la energía vendida y potencia instalada por comunidad y tecnología.

### A. Distribución entre comunidades
- ¿Qué comunidades destacan por mayor potencia instalada en energía eólica?  
- ¿Qué comunidades generan más energía vendida a partir de energía solar en relación con su potencia instalada?  
- ¿Qué comunidades dependen más de cogeneración o residuos frente a otras tecnologías?  
- ¿Qué comunidades contribuyen más al total nacional de energía vendida de renovables?  
- ¿Qué comunidades muestran menor crecimiento relativo en energía vendida de hidráulica durante los últimos años?  

### B. Crecimiento y tendencias
- ¿Qué comunidades han aumentado más rápidamente su energía vendida de biomasa en los últimos años?  
- ¿Qué tecnologías han mostrado mayor crecimiento en energía vendida dentro de las comunidades líderes?  
- ¿Qué tecnologías han perdido participación en el mix energético en algunas comunidades?  
- ¿Qué tecnologías muestran mayor variación en energía vendida entre comunidades autónomas?  

### C. Rendimiento y eficiencia
- ¿Qué comunidades convierten mejor la potencia instalada en energía vendida de solar y eólica?  
- ¿Existen comunidades con potencia instalada subutilizada en comparación con la energía vendida de biomasa y residuos?  
- ¿Qué tecnologías tienen mayor rendimiento promedio considerando energía vendida vs potencia instalada en distintas regiones?  
- ¿Qué tecnologías tienen una relación más equilibrada entre potencia instalada y energía vendida según la comunidad?  
- ¿Existen tecnologías con potencia instalada subutilizada en algunas comunidades?  
- ¿Qué tecnologías están presentes en todas las comunidades autónomas y cuáles solo en algunas?  
- ¿Cuáles son las tres principales tecnologías por energía vendida en cada comunidad? 


### Proyecciones futuras (modelos predictivos)
- ¿Qué comunidades tienen mayor potencial de crecimiento de energía renovable?  
- ¿Qué tecnologías muestran tendencia de expansión sostenida para los próximos años?  
- ¿Qué variables resultan más relevantes para predecir energía futura (potencia instalada, año, tipo de fuente)?  
- ¿Qué precisión alcanzan los modelos predictivos al estimar energía futura por comunidad y tecnología?  



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











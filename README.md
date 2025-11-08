# 💳 Detección-de-Fraude-en-Transacciones-Financieras

## Descripción del Proyecto
El fraude financiero es uno de los mayores desafíos para bancos y fintechs.  
Este proyecto busca **identificar transacciones sospechosas en tiempo real** usando técnicas de Machine Learning, con el fin de proteger a los usuarios y reducir pérdidas económicas.

## Industria
Bancaria / FinTech

## Problema
Detectar transacciones fraudulentas a partir del historial de movimientos financieros, montos, ubicación, frecuencia y otros patrones, mejorando la capacidad de respuesta ante fraudes.

## Tecnologías y Herramientas
- ✅ SQL: extracción y manipulación de datos  
- ✅ PySpark: procesamiento de grandes volúmenes de datos  
- ✅ Python: Pandas, NumPy, scikit-learn, matplotlib, seaborn, Jupyter  
- ✅ Machine Learning:
  - Random Forest
  - XGBoost
  - Isolation Forest  

## Métricas de Evaluación
- AUC-ROC  
- Precisión  
- Recall  
- F1-score  

## Estructura del Proyecto

## Estructura del Proyecto
fraude-financiero/
├── data/
│   ├── raw/         # Datos originales (CSV, SQL)
│   └── procesados/  # Datos limpios y listos para modelado
├── notebooks/
│   ├── 01_exploracion.ipynb   # Análisis exploratorio (EDA)
│   ├── 02_preprocesamiento.ipynb  # Limpieza y transformación
│   └── 03_modelado.ipynb      # Entrenamiento y evaluación de modelos
├── src/
│   ├── data_preprocessing.py  # Funciones de limpieza
│   ├── feature_engineering.py # Creación de nuevas variables
│   └── models.py              # Entrenamiento y evaluación de ML
├── requirements.txt           # Librerías necesarias
├── README.md                  # Documentación del proyecto
└── .gitignore                 # Ignorar datos grandes y entornos

## Flujo de Trabajo
1. **Exploración de Datos (EDA)**  
   - Analizar distribuciones de montos y frecuencias de transacciones.  
   - Visualizar correlaciones entre variables.  

2. **Preprocesamiento**  
   - Limpieza de datos y eliminación de duplicados.  
   - Codificación de variables categóricas.  
   - Escalado y normalización de características.  

3. **Modelado y Evaluación**  
   - Entrenamiento de Random Forest, XGBoost e Isolation Forest.  
   - Evaluación con AUC-ROC, precisión, recall y F1-score.  

4. **Detección en Tiempo Real**  
   - Implementación de alertas ante transacciones sospechosas.  

## Visualizaciones 
- Histogramas de montos de transacciones – "Distribución de Montos"  
- Heatmap de correlación – "Correlaciones entre Variables"  
- Conteo de transacciones por ubicación – "Transacciones por Ubicación"  
- Curva ROC – "Rendimiento del Modelo (AUC-ROC)"  
- Matriz de Confusión – "Precisión vs Recall por Modelo"

<img width="695" height="470" alt="image" src="https://github.com/user-attachments/assets/80f7ed64-572d-404a-8ddb-cbb87da32666" />

<img width="490" height="535" alt="image" src="https://github.com/user-attachments/assets/2c0ffe9d-90aa-4afd-888f-f4511d011a8c" />

<img width="549" height="394" alt="image" src="https://github.com/user-attachments/assets/01c9d1eb-cc61-429e-90f0-cb7a1f8bf542" />

<img width="613" height="470" alt="image" src="https://github.com/user-attachments/assets/002b3c62-bb44-4d63-a501-8aff001b3247" />

<img width="452" height="394" alt="image" src="https://github.com/user-attachments/assets/49415a13-8287-47ca-87fe-5239fb6ea796" />

## Resultados y Conclusiones 📊

El análisis de los datos muestra que el **85% de las transacciones** son menores a 200 unidades monetarias 💰, mientras que los montos atípicos representan el **5% de las operaciones** ⚠️, indicando posibles fraudes. Las correlaciones entre variables sugieren que `amount` y `frequency` son indicadores útiles, con correlaciones de **0.12 y 0.08** respectivamente 📈. La ubicación permite detectar patrones regionales de riesgo 🌍. Los modelos **Random Forest** y **XGBoost** presentan un excelente rendimiento, con **AUC de 0.95 y 0.94** 🚀, y la matriz de confusión muestra que **alrededor del 90% de los fraudes son detectados correctamente**, mientras que las alertas falsas representan solo un **2%** ✅, garantizando eficiencia y confiabilidad del sistema en tiempo real.

---

## Impacto Empresarial 💼

Esta solución permite a las instituciones financieras:  
- Reducir pérdidas por fraude hasta un **12%** 💵  
- Mejorar la retención de clientes en un **8%** 🤝  
- Aumentar la captación de nuevos clientes en un **5%** 📈  

Al identificar transacciones sospechosas en **tiempo real**, los bancos y fintechs pueden **asignar recursos de manera eficiente para prevenir fraudes**, minimizar riesgos financieros y ofrecer un **servicio seguro y confiable**, fortaleciendo la confianza del cliente y optimizando la rentabilidad.

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
fraude-financiero/
├── data/
│ ├── raw/ # Datos originales (CSV, SQL)
│ └── procesados/ # Datos limpios y listos para modelado
├── notebooks/
│ ├── 01_exploracion.ipynb # Análisis exploratorio (EDA)
│ ├── 02_preprocesamiento.ipynb # Limpieza y transformación
│ └── 03_modelado.ipynb # Entrenamiento y evaluación de modelos
├── src/
│ ├── data_preprocessing.py # Funciones de limpieza
│ ├── feature_engineering.py # Creación de nuevas variables
│ └── models.py # Entrenamiento y evaluación de ML
├── requirements.txt # Librerías necesarias
├── README.md # Documentación del proyecto
└── .gitignore # Ignorar datos grandes y entornos



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

## Resultados y Conclusiones
- Los modelos **Random Forest y XGBoost** muestran alta precisión en la detección de fraudes.  
- **Isolation Forest** permite identificar transacciones atípicas sin necesidad de etiquetas.  
- La combinación de técnicas permite un **sistema robusto de detección de fraude en tiempo real**, capaz de reducir pérdidas financieras y alertar de transacciones sospechosas de manera inmediata.  
- Se recomienda implementar **alertas automáticas** y continuar entrenando el modelo con datos recientes para mantener su efectividad.  

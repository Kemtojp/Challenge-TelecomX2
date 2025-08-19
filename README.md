# 📊 Challenge Telecom X – Parte 2  
**Predicción de Cancelación de Clientes (Churn) – Telecom LATAM**  

Este proyecto desarrolla modelos de *Machine Learning* para predecir qué clientes tienen mayor probabilidad de cancelar sus servicios en una empresa de telecomunicaciones.  
El objetivo principal es **identificar patrones de cancelación** para diseñar estrategias de retención más efectivas.  

---

## 🎯 Objetivos del Proyecto
- Preparar y preprocesar los datos de clientes para modelado predictivo.  
- Analizar la distribución de clientes que cancelan (*Churn*) vs. los que permanecen activos.  
- Entrenar y evaluar modelos de clasificación para predecir *churn*.  
- Interpretar la importancia de variables y su influencia en la cancelación.  
- Proponer **estrategias de retención basadas en datos**.  

---

## 📂 Estructura del Proyecto

Challenge_TelecomX2/

│── datos_tratados.csv # Datos tratados en formato CSV

│── Challenge_TelecomX2.ipynb # Cuaderno principal de análisis

│── README.md # Este archivo

---

## ⚙️ Preparación de los Datos
1. **Clasificación de variables**:  
   - *Numéricas*: tenure, MonthlyCharges, TotalCharges.  
   - *Categóricas*: Contract, PaymentMethod, InternetService, etc.  

2. **Preprocesamiento aplicado**:  
   - Expansión de columnas anidadas (customer, phone, internet, account).  
   - Eliminación de columnas irrelevantes (customerID).  
   - Tratamiento de valores faltantes.  
   - Codificación de variables categóricas con **One-Hot Encoding**.  
   - Normalización de variables numéricas con **StandardScaler** (para regresión logística).  
   - Balanceo de clases con **RandomUnderSampler**.  

3. **División en conjuntos**:  
   - Entrenamiento: 80%  
   - Prueba: 20%  

---

## 🔎 Análisis Exploratorio de Datos (EDA)
Durante el EDA se identificaron los siguientes patrones:  
- Clientes con **contratos cortos (Month-to-month)** presentan mayor cancelación.  
- **Tenure bajo** es el predictor más fuerte de churn.  
- Clientes con **facturación electrónica (PaperlessBilling)** tienden a cancelar más.  
- **Cargos mensuales bajos** se relacionan con mayor probabilidad de cancelación.  

📊 **Ejemplos de gráficos incluidos en el notebook**:  
- Boxplots de gastos mensuales y totales vs. churn.  
- Scatter plots de tenure × churn.  
- Matrices de correlación entre variables.  
- Matrices de confusión de los modelos.  

---

## 🤖 Modelado Predictivo
Se entrenaron y evaluaron dos modelos principales:  

- **Regresión Logística**  
  - Accuracy: ~0.74  
  - F1-score: ~0.74  
  - Limitación: más falsos negativos al predecir clientes que cancelan.  

- **Random Forest**  
  - Accuracy: ~0.77  
  - F1-score: ~0.78  
  - Mejor desempeño en detección de churners.  

📌 **Importancia de variables clave**:  
- Contract (duración de contrato).  
- Tenure (tiempo de permanencia).  
- MonthlyCharges y TotalCharges.  
- PaperlessBilling.  

---

## 📈 Conclusiones e Insights
- **Random Forest** superó a la regresión logística en métricas de rendimiento.  
- Los factores más críticos para la cancelación son:  
  1. Contratos cortos.  
  2. Bajo tiempo de permanencia.  
  3. Facturación electrónica.  
  4. Gastos mensuales bajos.  

📢 **Recomendaciones para la empresa**:  
- Incentivar renovación de contratos cortos.  
- Programas de fidelización para clientes nuevos.  
- Mejorar la experiencia de PaperlessBilling.  
- Monitoreo de clientes con bajo gasto mensual y tenure bajo.  

---

## 🛠️ Tecnologías Usadas
- **Manejo de datos**: pandas, numpy, json, ast.
- **Visualización**: matplotlib, seaborn.
- **Preprocesamiento y Modelado**:
  - OneHotEncoder, StandardScaler, ColumnTransformer, Pipeline (scikit-learn).
  - **Modelos**: LogisticRegression, RandomForestClassifier.
  - **División de datos**: train_test_split.
  - **Balanceo de clases**: RandomUnderSampler (imblearn).
- **Métricas y evaluación**: classification_report, confusion_matrix, ConfusionMatrixDisplay. 

---

## 🚀 Ejecución del Proyecto
1. Clonar el repositorio o descargar el archivo `.ipynb`.  
2. Abrir el cuaderno en Google Colab o Jupyter Notebook.  
3. Instalar dependencias:  

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
Cargar los datos (ubicados en datos_tratados.csv).

Ejecutar las celdas en orden para reproducir el análisis completo.
```

---

## 👤 Autor

- **Juan Velasquez**
- [Perfil de GitHub] (https://github.com/Kemtojp)
- [Perfil de LinkedIn] (https://www.linkedin.com/in/juan-velasquez-becerra/)

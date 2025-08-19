# Challenge-TelecomX2

## 📊 Predicción de Cancelación de Clientes (Churn) – Telecom LATAM

Este proyecto tiene como objetivo desarrollar modelos de Machine Learning para predecir qué clientes tienen mayor probabilidad de cancelar sus servicios en una empresa de telecomunicaciones, permitiendo diseñar estrategias de retención más efectivas.

## 🎯 Objetivos del Proyecto

- Preparar y preprocesar los datos de clientes para modelado predictivo.

- Analizar la distribución de clientes que cancelan vs. los que permanecen activos.

- Entrenar y evaluar modelos de clasificación para predecir churn.

- Interpretar la importancia de variables y su influencia en la cancelación.

- Proponer estrategias de retención basadas en datos.

## 🛠️ Tecnologías Usadas

- Python 3.10+

- Google Colab / Jupyter Notebook

- Pandas, NumPy

- Scikit-learn (Regresión Logística, Random Forest, métricas)

- Imbalanced-learn (balanceo de clases)

- Matplotlib / Seaborn (visualización de datos)

## ⚙️ Instalación y Requisitos

- Para ejecutar este proyecto:

- Clona este repositorio o descarga el archivo .ipynb.

- Abre el notebook en Google Colab o Jupyter Notebook.

- Ejecuta las celdas en orden, asegurándote de tener instaladas las librerías necesarias (pip install pandas scikit-learn imbalanced-learn matplotlib seaborn).

## 📂 Estructura del Análisis

- Carga y limpieza de datos

- Expansión de columnas anidadas (customer, phone, internet, account).

- Eliminación de columnas irrelevantes (customerID).

- Tratamiento de valores faltantes y balanceo de clases (RandomUnderSampler).

- Preprocesamiento

- Codificación de variables categóricas (One-Hot Encoding).

- Normalización de variables numéricas para modelos sensibles a la escala.

- Análisis Exploratorio (EDA)

- Distribución de churn y proporción de clases.

- Visualización de patrones en variables categóricas (contrato, método de pago, servicios) y numéricas (gastos, tiempo de permanencia).

- Identificación de relaciones significativas con churn.

- Modelado Predictivo

- Entrenamiento de Regresión Logística y Random Forest.

- Evaluación con accuracy, precision, recall, F1-score y matriz de confusión.

- Comparación de desempeño y análisis crítico de overfitting/underfitting.

- Interpretación de Variables

- Regresión Logística: análisis de coeficientes para evaluar impacto individual.

- Random Forest: importancia de variables basada en reducción de impureza.

- Identificación de variables más relevantes para predecir churn.

- Conclusiones y Recomendaciones

- Principales factores que influyen en la cancelación: contratos cortos, bajo tiempo de permanencia, métodos de pago electrónicos, gastos mensuales/total.

- Estrategias de retención: incentivos a contratos largos, programas de fidelización, revisión de servicios electrónicos y comunicación personalizada.

---

## 👤 Autor

- **Juan Velasquez**
- [Perfil de GitHub] (https://github.com/Kemtojp)
- [Perfil de LinkedIn] (https://www.linkedin.com/in/juan-velasquez-becerra/)

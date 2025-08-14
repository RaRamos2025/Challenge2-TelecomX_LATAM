# Proyecto Challenge2-TelecomX_LATAM: Análisis de la Tasa de Cancelación de Clientes (Churn)

## 1. Introducción 📌

Este proyecto se centra en el **análisis y la predicción de la tasa de cancelación de clientes (Churn)** para una empresa de telecomunicaciones. El objetivo principal es identificar a los clientes con mayor probabilidad de cancelar sus servicios y comprender los factores clave que influyen en esta decisión. La información generada permitirá a la empresa desarrollar estrategias de retención más efectivas, mejorando así la lealtad y el valor del cliente. El análisis se realiza sobre una base de datos de clientes, que ha sido previamente normalizada.

---

## 2. Objetivos 📄

Los objetivos del proyecto son los siguientes:
* **Análisis Exploratorio de Datos (EDA):** Entender la distribución de los datos y la relación entre las variables, prestando especial atención a la variable `Churn`.
* **Preparación de Datos:** Realizar un preprocesamiento exhaustivo, incluyendo la gestión de valores nulos, la codificación de variables categóricas y el balanceo de clases para preparar los datos para el modelado.
* **Construcción de Modelos Predictivos:** Desarrollar y entrenar al menos dos modelos de clasificación, como Regresión Logística y Random Forest, para predecir la probabilidad de churn.
* **Evaluación de Modelos:** Comparar el rendimiento de los modelos utilizando métricas clave como **Accuracy, Precision, Recall, F1-score y la Matriz de Confusión**.
* **Interpretación y Conclusiones:** Analizar la importancia de las variables en los modelos para identificar los factores más influyentes en la cancelación de clientes y generar conclusiones estratégicas para la empresa.

---

## 3. Herramientas utilizadas 🛠️

* **Google Colab:** Entorno de desarrollo para la ejecución del código Python.
* **Python:** Lenguaje de programación principal.
* **Pandas:** Para la manipulación y análisis de datos.
* **NumPy:** Para operaciones numéricas y matriciales.
* **Scikit-learn:** Para el preprocesamiento de datos y la construcción de modelos de machine learning.
* **Matplotlib y Seaborn:** Para la visualización de datos y la creación de gráficos (mapas de calor, boxplots, etc.).
* **Imbalanced-learn:** Para el manejo de desbalance de clases (SMOTE).

---

## 4. Estructura del proyecto 📊

El proyecto se encuentra organizado en un único notebook de Google Colab (`TelecomX2_LATAM.ipynb`), que contiene todo el flujo de trabajo, desde la carga de los datos hasta la interpretación de los resultados. Además, se utiliza el archivo `TelecomX_normalizado.csv` como la fuente de datos principal para el análisis.

* `README.MD`: Archivo MD que da cuenta de la información del presente repositorio.
* `TelecomX2_LATAM.ipynb`: Notebook de Google Colab con el código completo del proyecto.
* `TelecomX_normalizado.csv`: Archivo CSV con los datos de clientes, previamente preparados.
* `Informe final Challenge 2 TelecomX.pdf`: Archivo PDF con informe final que da cuenta de soluciones a la empresa. 

---

## 5. Ejecución del proyecto 🔧

El proyecto se realizó en las siguientes etapas generales:

1.  **Carga de Datos:** Se cargó el archivo `TelecomX_normalizado.csv` y se realizó una inspección inicial para entender la estructura de los datos. Se gestionaron los valores nulos y se eliminaron columnas irrelevantes como `customerID`.

2.  **Preparación de Datos:** Se transformaron las variables categóricas a formato numérico mediante One-Hot Encoding y Label Encoding. Se verificó la proporción de la variable objetivo (`Churn`) y se aplicó la técnica de sobremuestreo **SMOTE** para balancear las clases, ya que se detectó un desbalance significativo.

3.  **Análisis Exploratorio:** Se visualizaron las correlaciones entre las variables a través de un mapa de calor, enfocándose en las variables con una correlación significativa con `Churn`. Se investigó la relación de variables clave como la antigüedad (`tenure`) y el tipo de contrato con la tasa de cancelación.

4.  **Modelado:** Se dividieron los datos en conjuntos de entrenamiento y prueba. Se entrenaron dos modelos de clasificación: **Regresión Logística** (aplicando normalización) y **Random Forest** (sin normalización).

5.  **Evaluación de Modelos:** Se evaluó el rendimiento de ambos modelos utilizando un conjunto de métricas (Accuracy, Precision, Recall, F1-score) y la matriz de confusión. Los resultados permitieron identificar qué modelo tiene el mejor desempeño para este problema.

6.  **Interpretación y Conclusiones:** Se analizó la importancia de las variables en cada modelo, identificando los factores más críticos que influyen en el churn, como el tipo de contrato mensual, la antigüedad del cliente y los servicios adicionales. Finalmente, se plantearon conclusiones estratégicas para la empresa basadas en los hallazgos.

## 6. Repositorio 📁
El proyecto se puede encontrar íntegramente en: https://github.com/RaRamos2025/Challenge2-TelecomX_LATAM

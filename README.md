# 📊 Telecom X Challenge - Predicción de Churn

Este repositorio contiene el desarrollo del desafío **Telecom X** para la especialización en Data Science del programa **Oracle Next Education (ONE)**. 

El objetivo principal de este proyecto es analizar los datos de clientes de una empresa de telecomunicaciones y construir un modelo de Machine Learning capaz de predecir la cancelación del servicio (*Churn*), identificando qué factores retienen a los clientes y cuáles los impulsan a abandonar la empresa.

## 🚀 Descripción del Proyecto

El análisis se centra en un enfoque integral de ciencia de datos, abarcando desde la ingesta y tratamiento de los datos hasta el entrenamiento de modelos predictivos y la interpretación de negocio. 

A través de modelos de clasificación, buscamos responder: **¿Qué características hacen que un cliente sea propenso a cancelar su suscripción?**

## 🛠️ Tecnologías y Herramientas Utilizadas

El proyecto fue desarrollado en **Python** (vía Google Colab) utilizando las siguientes librerías:
* **Pandas:** Para la manipulación, limpieza y análisis de datos (`datos_tratados.csv`).
* **Matplotlib & Seaborn:** Para la visualización de datos y el Análisis Exploratorio (EDA).
* **Scikit-Learn:** Para el preprocesamiento, métricas de evaluación y entrenamiento de los modelos predictivos.

## 📂 Archivos Principales

* `telecom-x-parte2.ipynb`: Notebook principal que contiene todo el pipeline de Data Science. Incluye la extracción de datos, análisis bivariado, entrenamiento de los modelos y evaluación.
* `datos_tratados.csv`: Dataset limpio y preprocesado utilizado para alimentar el modelo. *(Nota: Asegúrate de tener este archivo en la ruta correcta al ejecutar el notebook).*

## 🧠 Modelado y Análisis

Para la predicción de Churn se implementó un modelo de **Regresión Logística**, entrenando tanto una versión estándar como una versión con pesos balanceados (`class_weight="balanced"`) para manejar el desequilibrio en la variable objetivo.

### Importancia de Variables (Feature Importance)
A partir del análisis de los coeficientes del modelo, se extrajeron las siguientes conclusiones estratégicas:

* **Factores de Riesgo (Aumentan el Churn):** Los contratos de mes a mes, el uso de pago con cheque electrónico y la suscripción a internet por fibra óptica son los principales impulsores de la cancelación.
* **Factores de Retención (Disminuyen el Churn):** La antigüedad del cliente (*Tenure*), los contratos a largo plazo (1 o 2 años) y la contratación de servicios adicionales (Soporte Técnico, Seguridad Online) son vitales para la fidelización.

## 💡 Conclusión Estratégica

El modelo demuestra que la retención de clientes está fuertemente ligada al compromiso contractual y a la percepción de valor de los servicios adicionales. Se recomienda incentivar la migración hacia planes anuales y revisar la relación calidad-precio del servicio de fibra óptica para reducir la tasa de abandono.

## ⚙️ Cómo ejecutar el proyecto

1. Clona este repositorio.
2. Asegúrate de tener instalado Python 3 y las librerías mencionadas.
3. Abre el archivo `telecom-x-parte2.ipynb` en Jupyter Notebook, Jupyter Lab o Google Colab.
4. Verifica que la ruta de lectura del archivo `.csv` coincida con la ubicación local del dataset.
5. Ejecuta las celdas de forma secuencial.

---
*Proyecto desarrollado como parte del track de Data Science de Oracle ONE.*

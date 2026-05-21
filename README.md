# Sistema Inteligente de Recomendación de Cultivos mediante Machine Learning

Proyecto desarrollado para la materia **Data Science 2**, enfocado en la aplicación de técnicas de Machine Learning para la recomendación de cultivos a partir de variables climáticas y del suelo.

---

# Objetivo del Proyecto

Desarrollar un modelo de clasificación capaz de recomendar el cultivo más adecuado según características ambientales y edáficas, utilizando algoritmos de Machine Learning.

---

# Dataset

Dataset público obtenido desde Kaggle.

## Variables utilizadas

- Nitrógeno
- Fósforo
- Potasio
- Temperatura
- Humedad
- pH
- Precipitaciones

## Variable objetivo

- Cultivo recomendado

El dataset contiene 22 tipos de cultivos diferentes.

---

# Tecnologías Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# Proceso Realizado

## 1. Exploratory Data Analysis (EDA)

Se realizó un análisis exploratorio de datos para:

- Analizar distribuciones
- Identificar relaciones entre variables
- Detectar correlaciones
- Comprender el comportamiento del dataset

---

## 2. Integración de API Climática

Se utilizó la API pública Open-Meteo para obtener datos climáticos correspondientes a una región agrícola de Punjab, India.

Los datos obtenidos fueron almacenados localmente en formato JSON.

---

## 3. Preprocesamiento e Ingeniería de Atributos

- Traducción y estandarización de variables
- Codificación de la variable objetivo mediante `LabelEncoder`
- Escalado de variables numéricas utilizando `StandardScaler`
- Separación entre variables predictoras y variable objetivo
- División Train/Test (80% / 20%)

---

## 4. Modelado

Se entrenaron los siguientes modelos:

- Regresión Logística
- Random Forest

---

## 5. Validación y Optimización

Se aplicaron:

- Validación cruzada (`Cross Validation`)
- Optimización de hiperparámetros mediante `GridSearchCV`

---

# Resultados

## Accuracy obtenida

| Modelo | Accuracy |
|---|---|
| Regresión Logística | 0.9795 |
| Random Forest | 0.9977 |

El modelo **Random Forest** presentó el mejor desempeño general.

---

# Importancia de Variables

El análisis de importancia de variables mostró que:

- Precipitaciones
- Humedad
- Potasio

fueron algunas de las variables más influyentes dentro del modelo predictivo.

---

# Conclusiones

Los resultados obtenidos demuestran que las variables climáticas y nutricionales poseen una elevada capacidad predictiva para la recomendación de cultivos.

El modelo Random Forest alcanzó un desempeño cercano al 100% de precisión, evidenciando el potencial del Machine Learning aplicado a la agricultura de precisión y a la toma de decisiones basada en datos.

---

# Autor

**Gastón Damiani**

Proyecto académico — Data Science 2 — Mayo 2026

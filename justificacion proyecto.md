# 📊 EduTech Analytics: Predicción de Completitud y Satisfacción Estudiantil

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?style=for-the-badge&logo=pandas)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn)
![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apachespark)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge)

## 📖 Descripción del Proyecto

Este proyecto forma parte de mi portafolio como **Científico de Datos**. Consiste en un análisis integral de datos de **500 estudiantes** de la plataforma de educación en línea *EduTech Analytics* durante el último año académico.

El objetivo principal es construir un sistema predictivo que permita a la plataforma identificar qué estudiantes están en riesgo de no completar sus cursos y predecir su nivel de satisfacción final, con el fin de generar recomendaciones basadas en datos para mejorar la retención estudiantil.

## 🎯 Objetivos Específicos

1. **Predecir la probabilidad** de que un estudiante complete exitosamente un curso (Clasificación).
2. **Estimar el puntaje de satisfacción** final que otorgará cada estudiante (Regresión).
3. **Identificar patrones de comportamiento** que influyen en el éxito académico (EDA).
4. **Generar recomendaciones estratégicas** para mejorar la retención basadas en los hallazgos.

## 🛠️ Tecnologías y Habilidades Aplicadas

Este proyecto demuestra mi capacidad para estructurar un flujo de trabajo completo de ciencia de datos, abarcando:

*   **Manipulación de Datos:** `pandas`, `numpy`
*   **Visualización de Datos:** `matplotlib`, `seaborn`
*   **Machine Learning:** `scikit-learn` (Random Forest, Logistic Regression, Ridge, SMOTE para balanceo de clases)
*   **Procesamiento a Escala:** `pyspark`
*   **Inferencia Estadística:** `scipy.stats`
*   **Buenas Prácticas:** Uso de semilla global (`RANDOM_STATE = 42`) para reproducibilidad, y prevención de *data leakage* aplicando el escalado (`StandardScaler`) después de la división train/test.

## 🧠 Justificación de Habilidades (Metodología)

El notebook está estructurado en 6 bloques que demuestran un flujo de trabajo profesional:

1.  **Análisis Exploratorio (EDA):** Limpieza de datos, identificación de valores nulos, duplicados, análisis de correlaciones (uso de `np.corrcoef`) y detección de outliers mediante el método IQR.
2.  **Feature Engineering:** Creación de variables predictivas clave como `tasa_completitud` y `estudiante_activo`, además de la codificación correcta de variables categóricas (Ordinales con *LabelEncoder* y Nominales con *OneHotEncoder*).
3.  **Modelado Predictivo:** Entrenamiento de modelos de clasificación (Random Forest, Logistic Regression) y regresión (Ridge, Random Forest Regressor) para predecir las variables objetivo.
4.  **Procesamiento con Spark:** Demostración de habilidades para manejar datos a mayor escala utilizando Apache Spark.
5.  **Inferencia Estadística:** Aplicación de pruebas estadísticas para validar hipótesis sobre el comportamiento de los estudiantes.
6.  **Reflexión Final:** Conclusiones de negocio y recomendaciones para EduTech Analytics.

## 📈 Principales Hallazgos

*   **Variables clave:** La `tasa_completitud` y el `promedio_evaluaciones` son los predictores más fuertes para determinar si un estudiante completará el curso.
*   **Satisfacción:** El `promedio_evaluaciones` y la `participacion_foros` tienen una correlación positiva significativa con el `puntaje_satisfaccion`.
*   **Retención:** Aproximadamente el 73% de los estudiantes son considerados "activos" (más de 50 sesiones), pero aún hay un margen de mejora para los estudiantes inactivos.

## 🚀 Cómo visualizar este proyecto

Puedes abrir y ejecutar este notebook directamente en Google Colab haciendo clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/orfalipadillaalexisosvaldo-hue/Ciencia_de_Datos/blob/main/Desafio_final_fundamentos_de_la_ciencia_de_datos/Desafio_final_fundamentos_de_la_ciencia_de_datos.ipynb)

## 📂 Estructura del Repositorio

*   `Desafio_final_fundamentos_de_la_ciencia_de_datos.ipynb`: Notebook principal con todo el análisis, código y visualizaciones.
*   `satisfaccion_horario.png`: Gráfico exportado en alta calidad (dpi=300) como resultado del análisis exploratorio.
*   `Estudiantes_edutech.csv`: Dataset original utilizado para el análisis.

## 👤 Autor

**Alexis Orfali**
*   Ingeniero Comercial & Programador | Trading Cuantitativo & Ciencia de Datos
*   [GitHub](https://github.com/orfalipadillaalexisosvaldo-hue)
*   [LinkedIn](https://www.linkedin.com/in/alexis-orfali-padilla-16295596/)

---
*Este proyecto fue desarrollado como parte de mi formación en Ciencia de Datos.*
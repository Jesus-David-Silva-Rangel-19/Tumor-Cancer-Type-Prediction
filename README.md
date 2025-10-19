### Análisis de Factores Clave para la Detección Temprana del Cáncer de Mama

**Descripción del Proyecto:**

Este proyecto tiene como propósito identificar los principales factores asociados al diagnóstico de cáncer de mama a partir del análisis exploratorio del conjunto de datos *Cancer_Data.csv*. El estudio se centra en comprender la estructura del dataset y en detectar patrones relevantes que sirvan de base para futuros modelos predictivos orientados a la detección temprana.

El análisis reveló que el conjunto de datos contiene **569 registros y 33 columnas**, de las cuales una se encuentra completamente vacía y debe eliminarse. La variable objetivo *diagnosis* diferencia entre tumores **benignos (B)** y **malignos (M)**, siendo esta última categoría la de mayor interés clínico. Se observó que las variables numéricas presentan **amplias diferencias de escala** —por ejemplo, *area_mean* alcanza valores superiores a 600, mientras que *smoothness_mean* ronda 0.1—, lo que indica la necesidad de **escalado previo al modelado**.

Los resultados del análisis estadístico mostraron una **alta dispersión en características como área y perímetro**, y la existencia de **valores atípicos en variables como *area_worst***, con máximos cercanos a 4254.0. Además, no se identificaron valores nulos en las columnas principales, lo que facilita el preprocesamiento. Estos hallazgos sugieren que el dataset es adecuado para modelado supervisado tras una limpieza estructural.

En conjunto, el análisis proporciona una **base sólida para el desarrollo de modelos predictivos** capaces de identificar patrones tempranos de malignidad. Se recomienda eliminar columnas irrelevantes (*id*, *Unnamed: 32*), codificar la variable objetivo, aplicar estandarización y entrenar modelos como Regresión Logística, Bosque Aleatorio o XGBoost. Estas acciones permitirán mejorar la precisión diagnóstica y apoyar decisiones clínicas basadas en datos.

---

### Key Factor Analysis for Early Breast Cancer Detection

**Project Description:**

This project aims to identify the main factors associated with breast cancer diagnosis through an exploratory analysis of the *Cancer_Data.csv* dataset. The study focuses on understanding the dataset’s structure and uncovering patterns that can support future predictive models for early detection.

The dataset contains **569 records and 33 columns**, with one entirely empty column that should be removed. The target variable *diagnosis* distinguishes between **benign (B)** and **malignant (M)** tumors, with the latter being of higher clinical importance. Numerical variables exhibit **significant scale differences** —for example, *area_mean* exceeds 600, while *smoothness_mean* remains near 0.1— indicating the need for **feature scaling before modeling**.

Statistical analysis revealed **high variability in features such as area and perimeter**, as well as **outliers in variables like *area_worst***, with values reaching up to 4254.0. No missing values were found in the main features, simplifying data preparation. These findings confirm that the dataset is suitable for supervised learning once basic cleaning is applied.

Overall, this analysis establishes a **robust foundation for predictive modeling** aimed at identifying early indicators of malignancy. It is recommended to remove irrelevant columns (*id*, *Unnamed: 32*), encode the target variable, standardize numerical data, and train models such as Logistic Regression, Random Forest, or XGBoost. These steps can enhance diagnostic accuracy and strengthen data-driven clinical decision-making.

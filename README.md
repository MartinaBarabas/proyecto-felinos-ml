# Modelado de Hábitats de Felinos Salvajes en Sudamérica mediante Machine Learning
Este repositorio contiene un proyecto personal avanzado de Ciencia de Datos enfocado en la conservación biológica y la ecología cuantitativa. El objetivo es analizar, preprocesar y clasificar los patrones geoespaciales y estacionales de las 6 especies de felinos salvajes nativos más representativas de América del Sur (*Panthera onca, Puma concolor, Leopardus pardalis, Leopardus guigna, Herpailurus yagouaroundi y Leopardus geoffroyi*).

El proyecto está diseñado como un laboratorio de experimentación científica, implementando y comparando de forma rigurosa los supuestos matemáticos de un amplio abanico de algoritmos clásicos y modernos de Machine Learning.

## Estructura del Pipeline del Proyecto
El desarrollo está organizado de forma modular en cuadernos independientes de Jupyter para facilitar su auditoría técnica:

*   **`01_eda_felinos.ipynb`:** Análisis Exploratorio de Datos avanzado. Diagnóstico de la calidad de 174,051 registros, detección de anomalías taxonómicas (depuración de fauna exótica y fósiles de *Smilodon*) e interpretación ecológica de sesgos espaciales y temporales.
*   **`02_preprocesamiento_supervisado.ipynb`:** Ingeniería de características críticas. Aplicación de submuestreo aleatorio (*undersampling*) para balancear clases, codificación cíclica sinusoidal/cosenoidal para variables temporales (meses), One-Hot Encoding controlado para mitigar multicolinealidad y escalado estándar aislado.
*   **`03_modelos_lineales_y_vecinos.ipynb`:** Primeros clasificadores supervisados. Implementación y evaluación comparativa de K-Vecinos más Cercanos (KNN) y Regresión Logística Multinomial (*Softmax*) mediante curvas ROC (AUC) y matrices de confusión.
*   **`04_analisis_discriminante.ipynb`:** Exploración de fronteras discriminantes clásicas (LDA y QDA) y análisis empírico del trade-off entre Sesgo (Bias) y Varianza.
*   **`05_reduccion_dimensionalidad.ipynb`:** Reducción del espacio de características a un plano 2D abstracto aplicando álgebra lineal mediante PCA (Componentes Principales) y SVD (Descomposición en Valores Singulares).
*   **`06_modelos_no_parametricos.ipynb`:** Modelado probabilístico y particionado ortogonal. Análisis de Ganancia de Información mediante Árboles de Decisión (Entropía de Shannon) frente al clasificador probabilístico Gaussian Naive Bayes.
*   **`07_ensembles_bosques.ipynb`:** Aprendizaje por ensamble en paralelo. Reducción drástica del error de varianza mediante arquitecturas de Bagging y Random Forest, incluyendo la auditoría del criterio de la IA a través de la importancia de variables (*Feature Importance*).

## 🚀 Tecnologías Utilizadas
*   **Lenguaje:** Python 3
*   **Entorno:** Visual Studio Code & Jupyter Notebooks
*   **Manipulación de datos:** Pandas, NumPy
*   **Visualización estadística:** Seaborn, Matplotlib
*   **Machine Learning:** Scikit-Learn

## Fuentes de Datos y Créditos
Los datos biológicos utilizados en este proyecto fueron obtenidos de la plataforma internacional **GBIF (Global Biodiversity Information Facility)**. 

* **Dataset:** Registros de ocurrencia para la familia *Felidae* en Sudamérica.
* **Cita:** GBIF.org (13 July 2026) GBIF Occurrence Download https://doi.org/10.15468/dl.3c6s46. Accedido el 13 de julio de 2026.

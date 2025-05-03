# UNIVERSIDAD TÉCNICA PARTICULAR DE LOJA

<img src="https://drive.google.com/uc?id=1X5UmWVlUX9XmckJgFLmv6mTTX81GEr0c" width="300">

## FACULTAD DE INGENIERÍAS Y ARQUITECTURA  
### MAESTRÍA EN INTELIGENCIA ARTIFICIAL APLICADA

---

## Práctica 1: Uso de aplicaciones colaborativas para herramientas de inteligencia artificial

**Autor:** Freddy Hernán Villota González  
**Docente:** M.Sc. Alexandra Cristina González Eras  
**Fecha:** 03 de mayo de 2025  

---

# UNIVERSIDAD TÉCNICA PARTICULAR DE LOJA

<img src="https://drive.google.com/uc?id=1X5UmWVlUX9XmckJgFLmv6mTTX81GEr0c" width="300">

## FACULTAD DE INGENIERÍAS Y ARQUITECTURA  
### MAESTRÍA EN INTELIGENCIA ARTIFICIAL APLICADA

---

## Práctica 1: Uso de aplicaciones colaborativas para herramientas de inteligencia artificial

**Autor:** Freddy Hernán Villota González  
**Docente:** M.Sc. Alexandra Cristina González Eras  
**Fecha:** 03 de mayo de 2025  

---

### 🎯 Objetivo del Proyecto

Desarrollar una herramienta preliminar de apoyo para clasificar la potabilidad del agua utilizando variables fisicoquímicas. Se emplea un enfoque colaborativo en Google Colab y GitHub, integrando bibliotecas de análisis y visualización como pandas, seaborn y matplotlib, y modelos de machine learning como Random Forest.

---

### 🧪 Problemática Ambiental

En zonas rurales y periurbanas, no siempre existen sistemas automatizados para evaluar la potabilidad del agua, lo cual implica un riesgo para la salud pública. Este proyecto propone un sistema de análisis automático a partir de datos abiertos para apoyar decisiones sanitarias.

---

### ⚙️ Herramientas Utilizadas

- Google Colab  
- GitHub + Google Drive  
- Python + pandas, seaborn, matplotlib, scikit-learn  
- Modelo de Random Forest con datos escalados  

---

### 📁 Estructura del Repositorio

MIAA_practica1/
│
├── data/
│ └── water_potability.csv
│
├── Practica01.ipynb # Notebook principal con análisis completo
├── git_push.ipynb # Notebook seguro para hacer git push
├── README.md # Este archivo
└── .gitignore # Ignora git_push.ipynb y otros archivos sensibles


---

### 📊 Análisis Exploratorio

Se agregaron 4 nuevas columnas al DataFrame para enriquecer el análisis:

1. `ph_categoria`: clasificación cualitativa del pH (ácido, neutro, alcalino)  
2. `indice_sales`: índice calculado a partir de sólidos disueltos y conductividad  
3. `riesgo_thm`: riesgo bajo, moderado o alto por trihalometanos  
4. `calidad_simplificada`: indicador binario de calidad general del agua

Además, se exploraron estadísticas descriptivas y visualizaciones clave, incluyendo:

- Distribución de potabilidad por categoría de pH  
- Matriz de correlación entre variables  

---

### 🤖 Modelo de Clasificación

Se entrenó un modelo de **Random Forest** para predecir la potabilidad del agua.  
**Resultados clave**:

- Accuracy: ~67%  
- Precision y Recall moderados  
- pH, Sulfatos y Cloraminas fueron las variables más importantes

También se analizó la distribución de residuos para validar que no haya overfitting y se visualizó la importancia relativa de cada parámetro.

---

### 🔐 Integración con GitHub

Este proyecto está conectado con GitHub de forma segura:

- `git_push.ipynb` permite hacer `git add`, `commit` y `push` desde Colab
- Se evita exposición de tokens usando widgets y `.gitignore`
- Se puede trabajar local o en la nube, manteniendo sincronización

---

### ✅ Resultado de aprendizaje

Este trabajo demuestra cómo aplicar herramientas colaborativas (Colab + GitHub) para resolver un problema ambiental real con inteligencia artificial, integrando análisis de datos, visualización y modelos de clasificación.

---

### 📬 Contacto

Freddy Hernán Villota González  
[freddyvillota@gmail.com](mailto:freddyvillota@gmail.com)


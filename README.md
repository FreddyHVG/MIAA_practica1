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


```plaintext
MIAA_practica1/
│
├── .git/                      # Carpeta de configuración de Git
├── data/                      # Dataset original (water_potability.csv)
├── modelo/                    # Modelos entrenados (.pkl) y scaler
├── static/                    # Archivos estáticos (imágenes, CSS)
│   └── images/
│       ├── utpl2.png
│       └── potable.jpg
├── templates/                 # Archivos HTML para Flask (formulario, resultado)
│   ├── formulario.html
│   └── resultado.html
├── .gitignore                 # Ignora archivos sensibles o innecesarios
├── app_flask.ipynb           # Aplicación web con Flask y despliegue con Ngrok
├── git_push.ipynb            # Script para autenticación y push a GitHub desde Colab
├── notebook.ipynb            # Notebook principal: análisis, visualización, entrenamiento
└── README.md                 # Descripción general del proyecto (este archivo)


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
### 🌐 Despliegue con Flask y Ngrok
Como parte del desarrollo, se integró un microservidor web utilizando Flask, permitiendo el despliegue de un formulario interactivo para la predicción de potabilidad del agua. Esta interfaz fue embellecida con HTML y CSS, mostrando una página informativa con formulario, descripciones de parámetros fisicoquímicos y un resultado visual con imágenes dinámicas según la predicción.

El modelo entrenado con Random Forest fue cargado en el backend de Flask y expuesto mediante una ruta /predict, la cual recibe los parámetros ingresados, calcula automáticamente el índice de sales y devuelve un diagnóstico sobre la potabilidad.
Además, se utilizó Ngrok para crear un túnel seguro que expone localmente la aplicación Flask y permite acceder al formulario desde cualquier dispositivo con conexión a internet, facilitando demostraciones remotas.

**Tecnologías utilizadas:**
- Flask
- Ngrok + Pyngrok
- HTML + CSS personalizados
- Imágenes y recursos cargados desde Google Drive

Este despliegue práctico refuerza la comprensión de cómo un modelo de IA puede integrarse en aplicaciones web accesibles, fortaleciendo habilidades en desarrollo backend y comunicación de resultados.

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


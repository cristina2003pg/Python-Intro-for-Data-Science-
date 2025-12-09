# Python-Intro-for-Data-Science-
This repository holds all the files seen during the CodeSpace Bootcamp for Data Science 

# Installation 

To install the required packages, run the following comand:

´´´ bash 

pip install -r requirements.txt
´´´

# Python Intro for Data Science

Este repositorio recopila las prácticas desarrolladas durante el Bootcamp de Data Science.  
La parte final del trabajo se centra en **MLflow, experiment tracking, Kaggle, y despliegue con Docker**.

---

## 🚀 MLflow – Gestión del ciclo de vida del modelo

### 📌 Setup

- Python ≥ 3.9.x  
- Clonar el repositorio  
- Crear y activar entorno virtual si se trabaja en local  

```bash
pip install -r requirements.txt


## levantar servidor de MLFLOW 
mlflow ui --port 5000

Luego abre en el navegador:

👉 http://127.0.0.1:5000

## Desplegar modelo con Docker

Ejecutar sección Docker Model del Notebook MLFLOW IV - Kaggle II para generar loan_predictions.pkl.
Este archivo no se sube a GitHub (está en .gitignore).

docker build -t loan-model-api .

docker run -p 5002:5002 loan-model-api

# estructura del proyecto 

📁 Python-Intro-for-Data-Science
 ├── 📁 data
 ├── 📁 notebooks
 ├── 📁 mlruns
 ├── Dockerfile
 ├── app.py
 ├── README.md
 ├── requirements.txt

# Motivacion 

El objetivo de este proyecto es aprender a gestionar de forma profesional el ciclo de vida de un modelo de Machine Learning mediante MLflow, visualizar métricas, versionar modelos y compararlos.
Además, se integra Kaggle para utilizar datos reales y evaluar resultados con un ranking online.


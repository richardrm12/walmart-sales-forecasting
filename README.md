# Store Sales Time Series Forecasting

Este proyecto pertenece a la competencia de Kaggle "Walmart Recruiting - Store Sales Forecasting". 
El objetivo es predecir las ventas semanales (`Weekly_Sales`) para diferentes combinaciones de tienda y departamento (Store, Dept) utilizando datos históricos.

## Estructura del Proyecto

* **`.github/`**: Archivos de configuración y prompts para GitHub Copilot.
* **`notebooks/`**: Notebooks de Jupyter con el análisis y modelado:
  * `01_EDA.ipynb`: Análisis Exploratorio de Datos.
  * `02_Feature_Engineering.ipynb`: Creación y preprocesamiento de variables.
  * `03_Modelado_LightGBM_y_XGBoost.ipynb`: Entrenamiento de modelos.
  * `04_Test_Submission.ipynb`: Predicciones sobre el conjunto de test.
  * `05_Interpretabilidad_y_Explicabilidad.ipynb`: Análisis de los modelos (ej. SHAP values).
* **`requirements.txt`**: Dependencias para reproducir el entorno.

*(Nota: Los directorios `data/`, `models/` y `outputs/` se encuentran en el repositorio, pero su contenido es excluido para no subir información pesada ni afectar los límites de GitHub).

## Instalación

Para reproducir el entorno, puedes crear un entorno virtual e instalar las dependencias:

```bash
python -m venv .venv
# Activar entorno (Windows)
.venv\Scripts\activate
# Instalar dependencias
pip install -r requirements.txt
```

## Datos

Los datos originales deben colocarse en el directorio `data/raw/` y pueden ser descargados desde [Kaggle](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting/data).

* `train.csv` / `test.csv` / `features.csv` / `stores.csv` / `sampleSubmission.csv`

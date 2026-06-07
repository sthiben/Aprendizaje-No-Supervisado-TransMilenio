# Aprendizaje no supervisado con TransMilenio

Proyecto desarrollado en Jupyter Notebook para agrupar estaciones troncales de TransMilenio según características como área, accesos, capacidad, vagones y ubicación.

## Metodología

1. Carga y limpieza del archivo `Estación_troncal.csv`.
2. Escalamiento de variables con `StandardScaler`.
3. Entrenamiento de un Autoencoder con arquitectura:

```text
8 → 2 → 8
```

4. Uso de activación ReLU.
5. Aplicación de K-Means sobre las dos neuronas comprimidas.
6. Evaluación de los clusters con Silhouette Score.

## Resultado

El mejor resultado se obtuvo con:

```text
K = 3
Silhouette Score ≈ 0.6422
```

El modelo permitió formar tres grupos de estaciones con características similares.

## Archivos principales

```text
Estación_troncal.csv
aprendizaje_no_supervisado_transmilenio.ipynb
resultado_autoencoder_transmilenio.csv
imagenes/
```

## Tecnologías

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Scikit-learn

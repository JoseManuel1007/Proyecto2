# Proyecto2

## Descripción
Script para analizar datos experimentales de baterías de ion-litio. Calcula el Estado de Carga (SOC) y el Estado de Salud (SOH), genera gráficos (voltaje, corriente, temperatura, SOC), permite dimensionar bancos de baterías y comparar químicas según energía y masa.

## Librerías usadas
```python
import os
import glob
import shutil
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from google.colab import drive

Contenido del repositorio

main.py o celdas para ejecutar en Google Colab (código principal).

README.md (este archivo).

Datos externos (no incluidos): carpeta Proyecto2 en Google Drive con metadata.csv y la carpeta data/ con los CSV de los ciclos.

Enlace de descarga de archivos necesarios

Carpeta de Drive con los datos requeridos:
https://drive.google.com/drive/folders/1UOdV_4DI9zW6ew3mz8O9dPpX2v98Py8l?usp=drive_link

Estructura esperada de la carpeta de datos
Proyecto2/
├── metadata.csv
└── data/
    ├── 00001.csv
    ├── 00002.csv
    └── ...


Importante: los archivos deben estar en una carpeta llamada Proyecto2 dentro de tu Google Drive antes de ejecutar el script.

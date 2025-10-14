# Proyecto: Análisis y Dimensionamiento de Baterías de Ion-Litio

## Descripción
Script para analizar datos experimentales de baterías de ion-litio. Calcula el Estado de Carga (SOC) y el Estado de Salud (SOH), genera gráficos (voltaje, corriente, temperatura, SOC), permite dimensionar bancos de baterías y comparar químicas según energía y masa.

## Contenido del repositorio
- `main.py` (o las celdas para ejecutar en Google Colab): código principal que monta Drive, carga metadata y datos, calcula SOC/SOH y presenta resultados.  
- `README.md`: este archivo.  
- **Datos externos (no incluidos en el repositorio):** carpeta `Proyecto2` en Google Drive con los archivos necesarios para generar las gráficas.

## Librerías usadas
```python
import os
import glob
import shutil
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from google.colab import drive
Enlace de descarga de archivos necesarios
Los archivos de datos requeridos para generar las gráficas están disponibles en la siguiente carpeta de Google Drive:

👉 Descargar carpeta Proyecto2

Esta carpeta contiene:

metadata.csv: necesario para calcular y graficar el SOH.

data/: todos los archivos CSV con la información de los ciclos experimentales.

Nota: Los archivos deben estar dentro de una carpeta llamada Proyecto2 en tu Google Drive antes de ejecutar el código.

Estructura esperada de la carpeta de datos
kotlin
Copiar código
Proyecto2/
├── metadata.csv
└── data/
    ├── 00001.csv
    ├── 00002.csv
    └── ...
Uso (Google Colab)
Abrir Google Colab y subir el script o copiar las celdas.

Montar Google Drive:

python
Copiar código
from google.colab import drive
drive.mount('/content/drive')
Verificar la ruta donde está la carpeta Proyecto2:

python
Copiar código
GOOGLE_DRIVE_DATA_PATH = "/content/drive/MyDrive/Proyecto2"
Ejecutar el script.

Seguir el flujo interactivo:

Elegir el ID de la batería y el ciclo a analizar.

Generar gráficos de voltaje, corriente, temperatura y SOC.

Visualizar la evolución del SOH.

Calcular el número de celdas necesarias según la energía deseada.

(Opcional) Comparar con otra batería.

Notas técnicas
metadata.csv debe incluir las columnas: type, start_time, ambient_temperature, battery_id, test_id, uid, filename, Capacity, Re, Rct.

Los archivos CSV deben contener al menos Time y Current_measured, y preferiblemente Voltage_measured y Temperature_measured.

Para proyectos con gran cantidad de archivos, se recomienda acceder directamente desde Google Drive para evitar límites de descarga.

Resultados esperados
Cálculo del SOC y del SOH.

Gráficas de comportamiento eléctrico.

Evolución del SOH por ciclo.

Dimensionamiento de bancos de baterías.

Comparación entre diferentes químicas.

Autor
José Manuel Criollo Chapal
Proyecto académico — 2025

yaml
Copiar código

---

El enlace de descarga es este:  
🔗 **https://drive.google.com/drive/folders/1UOdV_4DI9zW6ew3mz8O9dPpX2v98Py8l?usp=drive_link**  

¿Quieres que lo formatee también con títulos en mayúsculas (como los repos de GitHub más técnicos) y 

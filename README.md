# Proyecto2

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

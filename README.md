# Proyecto2

## Descripción
Este proyecto permite analizar el comportamiento y degradación de baterías de ion-litio mediante el cálculo del Estado de Carga (SOC) y el Estado de Salud (SOH). También incluye una función para dimensionar bancos de baterías y comparar diferentes químicas según su energía y peso.

## Librerías utilizadas
```python
import os
import glob
import shutil
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from google.colab import drive

Proyecto2/
├── metadata.csv
└── data/
    ├── B0005_cycle1.csv
    ├── B0005_cycle2.csv
    └── ...


  

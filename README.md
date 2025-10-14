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

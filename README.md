[README.md](https://github.com/user-attachments/files/23178999/README.md)
# 🧠 Parcial 2 – Análisis de Fallas Tecnológicas y Riesgo Operacional

## 📘 Descripción General
Este proyecto realiza un **análisis de fallas tecnológicas** mediante el uso de **clustering no supervisado (K-Medoids)** y métricas de riesgo, con el objetivo de identificar patrones de frecuencia y severidad en los eventos tecnológicos que afectan a una organización.

A partir de un conjunto de datos en Excel (`FallasTecnológicas.xlsx`), el código clasifica los eventos según su **frecuencia** y **severidad**, generando un **mapa de pérdidas** que permite visualizar los clústeres de riesgo más críticos.

---

## 🧩 Funcionalidades Principales
- Implementación personalizada del algoritmo **K-Medoids** para agrupar datos de frecuencia y severidad.
- Cálculo de parámetros estadísticos (media, varianza, asimetría).
- Generación de un **heatmap** (mapa de calor) para representar visualmente los niveles de pérdida combinando frecuencia y severidad.
- Identificación de clústeres representativos de eventos tecnológicos según su impacto.

---

## 📊 Estructura del Proyecto
```
Parcial2.ipynb
│
├── Carga de datos
│   └── Importa el archivo Excel con las fallas tecnológicas.
│
├── Implementación del algoritmo K-Medoids
│   └── Agrupa los datos de frecuencia y severidad.
│
├── Modelado de variables
│   └── Define niveles (Muy Pocos, Pocos, Algunos, Muchos, Bastantes).
│   └── Define severidad (Muy Bajo, Bajo, Medio, Alto, Crítico).
│
├── Mapa de Pérdidas
│   └── Calcula el producto cruzado de frecuencia y severidad.
│   └── Visualiza con un heatmap de Seaborn.
│
└── Interpretación de resultados
    └── Identifica clústeres de riesgo y patrones relevantes.
```

---

## 🧮 Requisitos Técnicos
El notebook está diseñado para ejecutarse en **Google Colab** (aunque también puede correr localmente).

**Dependencias principales:**
```bash
numpy
pandas
matplotlib
seaborn
scipy
```

Para instalarlas localmente:
```bash
pip install numpy pandas matplotlib seaborn scipy
```

---

## 📂 Datos de Entrada
El archivo de entrada debe estar ubicado en tu Google Drive en la ruta:

```
/content/drive/MyDrive/Integración de datos y prospectiva/Parcial_2/5. FallasTecnológicas.xlsx
```

Debe contener columnas con al menos:
- Identificador del evento
- Descripción del evento
- Frecuencia
- Severidad

---

## 📈 Resultados
- **Mapa de pérdidas (Heatmap):** muestra la interacción entre la frecuencia y la severidad de los eventos tecnológicos.
- **Clústeres de riesgo:** resumen los grupos de eventos con características similares.
- **Análisis interpretativo:** permite enfocar estrategias de mitigación y priorización de riesgos tecnológicos.

---

## 💡 Interpretación Clave
El análisis permite identificar:
- **Eventos frecuentes pero de baja severidad**, que representan pérdidas menores pero continuas.
- **Eventos de severidad media y frecuencia media**, que suelen revelar **problemas estructurales** en los sistemas.
- **Eventos críticos**, poco frecuentes pero con gran impacto, que requieren **planes de contingencia** específicos.

---

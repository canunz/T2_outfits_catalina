# 🧠 BI_T2_NuñezCatalina — Análisis temporal de publicaciones de prendas

---

## 📘 Descripción general

Este proyecto analiza la evolución temporal de publicaciones de prendas en línea utilizando el dataset **`outfits.csv`**, en el contexto de la asignatura **Inteligencia de Negocios**.

Se aplican tres técnicas de Machine Learning orientadas al análisis temporal dentro del marco de Business Intelligence:

- **Regresión lineal:** estima la tendencia de crecimiento en el tiempo.  
- **Clasificación (Random Forest):** distingue publicaciones recientes y periodos de alta o baja actividad.  
- **Clustering (K-Means, DBSCAN y Jerárquico):** identifica grupos de meses con comportamientos similares.

Los resultados revelan patrones de comportamiento, fluctuaciones y estacionalidades que pueden utilizarse para la toma de decisiones estratégicas.

---

## ⚙️ Entorno de desarrollo

El proyecto fue desarrollado y ejecutado en **Visual Studio Code (VS Code)** sobre un entorno local de **Python 3.11.x**.  
No se utilizó Google Colab.  
Se empleó un entorno virtual con las dependencias definidas en `requirements.txt`.

---

## 📁 Estructura del proyecto

BI_T2_NuñezCatalina/
│
├── figuras/ → Gráficos generados por los modelos
│ ├── 01_publicaciones_por_anio.png
│ ├── 02_regresion_temporal.png
│ ├── 03_validacion_cruzada.png
│ ├── 04_matriz_confusion_alta_baja.png
│ ├── 07_roc_curve_reciente.png
│ └── ...
│
├── BI_T2_NuñezCatalina.ipynb → Notebook principal con el desarrollo
├── outfits (1).csv → Dataset base
├── diccionario_variables.txt → Descripción de variables del dataset
├── referencias.txt → Bibliografía y fuentes
├── requirements.txt → Dependencias del entorno
└── README.md → Documento informativo (este archivo)


---

## 💻 Requisitos y ejecución

**Versión de Python probada:** `3.11.7`

### 1️⃣ Crear entorno virtual
```bash
python -m venv .venv
.\.venv\Scripts\Activate.ps1

2️⃣ Instalar dependencias
pip install -r requirements.txt

3️⃣ Ejecutar el proyecto

Abrir el notebook BI_T2_NuñezCatalina.ipynb en Visual Studio Code.
Seleccionar el kernel correspondiente al entorno virtual (.venv o bi_t2).
Ejecutar todas las celdas en orden.


📊 Dataset y licencia

Nombre: Vibrent Clothes Rental Dataset
Autor: K. A. K. Borgersen (2024)
Fuente: Kaggle
Licencia: Uso académico y de investigación
Contenido: 15.600 registros (2016–2024) con variables de precios, categorías, marcas y fecha de publicación (timeCreated).

🧩 Técnicas aplicadas y métricas
| Tipo de análisis  | Modelo aplicado               | Principales resultados                                |
| ----------------- | ----------------------------- | ----------------------------------------------------- |
| **Regresión**     | Lineal simple                 | R² = 0.121 · MAE = 109.45 · RMSE = 149.35             |
| **Clasificación** | Random Forest                 | Accuracy = 1.00 (reciente/antigua) · 0.63 (alta/baja) |
| **Clustering**    | K-Means / Jerárquico / DBSCAN | Silhouette = 0.677 (K-Means)                          |


🧾 Referencias

Borgersen, K. A. K. (2024). Vibrent Clothes Rental Dataset. Kaggle.
Librerías utilizadas: pandas, numpy, matplotlib, seaborn, scikit-learn.


✨ Autoría

Estudiante: Catalina Soledad Núñez Yañez
Carrera: Ingeniería en Informática y Telecomunicaciones – Duoc UC, Sede Puerto Montt
Asignatura: Inteligencia de Negocios
Año: 2025

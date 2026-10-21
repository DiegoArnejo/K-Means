# 📊 Aprendizaje No Supervisado: Agrupamiento con K-Means

Este repositorio contiene dos proyectos prácticos desarrollados en Python que aplican el algoritmo **K-Means Clustering** para la segmentación de datos. Ambos scripts implementan una metodología estandarizada: preparación de datos, escalamiento mediante $Z$-score, agrupamiento no supervisado y visualización de resultados.

---

## 🛠️ Tecnologías Utilizadas

* **Pandas:** Estructuración y manipulación de datos tabular.
* **Scikit-Learn:** 
  * `StandardScaler`: Normalización de variables para garantizar que la escala no distorsione la distancia euclidiana del algoritmo.
  * `KMeans`: Algoritmo de agrupamiento basado en centroides.
* **Matplotlib:** Creación de gráficos explicativos de dispersión.

---

## 📂 Descripción de los Proyectos

### 1. Segmentación Geográfica (`K-Means_INDEC.py`)
Analiza datos reales del Censo 2022 (INDEC) sobre viviendas particulares habitadas en las provincias argentinas.

* **Objetivo:** Clasificar las 24 jurisdicciones según la densidad de viviendas habitadas.
* **Configuración del Modelo:** $K = 3$ clústeres.
* **Metodología Destacada:** 
  * Asignación dinámica de etiquetas (*Pocas viviendas*, *Cantidad normal de viviendas*, *Muchas viviendas*) ordenando los promedios de cada grupo para dar un significado de negocio/análisis a los números.
  * Visualización formateada con etiquetas inclinadas a 90° para facilitar su lectura.

### 2. Segmentación de Perfiles Estudiantiles (`K-Means_Estudiantes.py`)
Utiliza un conjunto de datos simulados con múltiples variables sobre comportamiento académico.

* **Objetivo:** Descubrir patrones ocultos de estudiantes según su `edad`, `horas_estudio` y `promedio_academico`.
* **Configuración del Modelo:** $K = 4$ clústeres.
* **Metodología Destacada:** 
  * El modelo entrena usando 3 dimensiones cuantitativas, pero permite visualizar patrones en gráficos 2D (Edad vs. Promedio Académico) identificando cada grupo mediante un código de colores.

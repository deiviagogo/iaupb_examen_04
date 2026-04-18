# IAUPB - Examen 04: Aprendizaje No Supervisado  
## Comparación de Algoritmos de Clustering

---

## Información General

- Curso: Inteligencia Artificial  
- Programa: Ingeniería en Sistemas e Informática / Ciencia de Datos  
- Periodo: 202610  
- Tipo de evaluación: Individual  
- Estudiante: [TU NOMBRE COMPLETO]  
- Docente: Juan Darío Rodas  

---

## Estructura del Repositorio
iaupb_examen_04/
│
├── iaupb_examen_04_clustering.ipynb # Notebook principal con toda la solución
├── README.md # Documentación del proyecto
└── data/ # (Opcional) Dataset si se incluye localmente

---

## Objetivo del Proyecto

El objetivo de este proyecto es comparar el desempeño de tres algoritmos de clustering aplicados al dataset de pingüinos del archipiélago Palmer, con el fin de identificar cuál ofrece mejores resultados según distintas métricas de evaluación.

---

## Dataset

- Nombre: Palmer Penguins Dataset  
- Fuente: https://archive.ics.uci.edu/dataset/690/palmer+penguins-3  
- Registros: 344  

### Variables

- Longitud del pico  
- Profundidad del pico  
- Longitud de la aleta  
- Masa corporal  
- Isla  
- Sexo  

Variable objetivo (no utilizada en el entrenamiento):  
- Especie (3 clases)

---

## Metodología

El desarrollo del proyecto sigue una pipeline estructurada de análisis de datos:

### 1. Carga y Exploración Inicial
- Inspección de estructura y tipos de datos  
- Identificación de valores nulos  
- Estadísticas descriptivas  

### 2. Análisis Exploratorio de Datos (EDA)
- Distribución de variables  
- Detección de outliers  
- Relaciones entre variables  

### 3. Preprocesamiento
- Manejo de valores faltantes  
- Codificación de variables categóricas  
- Normalización de variables numéricas  

---

## Algoritmos Implementados

### K-Means
- Basado en centroides  
- Requiere definir el número de clusters  

### DBSCAN
- Basado en densidad  
- Permite detectar ruido  
- Parámetros clave: eps, min_samples  

### Clustering Jerárquico
- Basado en distancias  
- Métodos evaluados: ward, single  

---

## Métricas de Evaluación

Se utilizaron las siguientes métricas para comparar los modelos:

- Silhouette Score (mayor es mejor)  
- Davies-Bouldin Index (menor es mejor)  
- Calinski-Harabasz Index (mayor es mejor)  
- Número de clusters detectados  

---

## Visualizaciones

El notebook incluye:

- Comparación entre clusters reales (ground truth) y los obtenidos por cada algoritmo  
- Gráfico de barras agrupadas con las métricas evaluadas  

Cada visualización cumple con:

- Título descriptivo  
- Ejes correctamente etiquetados  
- Leyendas claras  
- Escalas adecuadas  

---

## Selección del Mejor Modelo

La selección del mejor algoritmo se realizó considerando todas las métricas de forma integral.  

No se tomó como criterio único el número de clusters, sino la calidad de separación, cohesión y consistencia de los resultados.  

La justificación detallada se encuentra en el notebook.

---

## Análisis e Interpretación

El notebook incluye respuestas a:

1. Separabilidad de las especies  
2. Naturaleza del ruido en DBSCAN  
3. Diferencias entre métodos jerárquicos  
4. Impacto de la variable island  

Cada respuesta está argumentada con base en los resultados obtenidos.

---

## Tecnologías Utilizadas

- Python 3  
- Google Colab  

Librerías principales:

- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  

---

## Requisitos de Ejecución

1. Abrir el archivo .ipynb en Google Colab  
2. Ejecutar todas las celdas en orden  
3. Verificar que no haya errores  
4. Confirmar que todas las gráficas se visualizan correctamente  

---

## Consideraciones Finales

- El notebook se entrega completamente ejecutado  
- No contiene errores en celdas  
- Incluye todas las visualizaciones requeridas  
- Cumple con las métricas y análisis solicitados  
- La solución fue desarrollada de manera individual  

---

## Entrega

- Repositorio en GitHub: iaupb_examen_04  
- Rama utilizada: main  
- Docente agregado como colaborador  
- Notificación enviada por correo  

---

## Nota de Integridad Académica

Este trabajo fue realizado respetando los principios de honestidad académica.  
El uso de herramientas de inteligencia artificial fue aplicado como apoyo para mejorar la calidad de la solución.

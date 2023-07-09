# Libreria pandas_profiling (https://pypi.org/project/pandas-profiling/)

Herramienta para crear informes en formato HTML interactivo, utilizado para hacer **EDA (Exploratory Data Analysis)**

## Analisis del informe report.html 

### Primer vistazo a estado de los datos que pueden requerir transformacion para un analisis mas acertado.

### 1. Overview

- Tipo de variables
- Filas Duplicadas
- Valores Faltantes


### 2. Alertas

#### 2.1 Correlacion Alta
#### 2.2 Desbalances
#### 2.3 Valores faltantes
#### 2.4 Sesgo (Skewness)
#### 2.5 Ceros
#### 2.6 Duplicados


### 3. Reproduction

En esta seccion del informe se observa variables del analisis como duracion, software utilizado y configuracion

 
Nota: Estas interacciones se ven afectadas por las alertas presentadas referentes a Ceros y Valores Faltantes por lo cual es necesario corregir primero esas Alertas para luego pasar a interpretar o no estas Interactions entre variables numericas

Luego de revisar esas 3 pestañas pasamos a revisar los siguientes items del informe:

### A. Variables

Cada una de las variables con sus caracteristicas y metricas estadisticas mas comunes.

### B. Correlations

Correlaciones entre variables presentadas en formato de Heatmap y Table

### C. Missing Values

Valores faltantes presentadas en formato Count, Matrix y Heatmap.

### D. Sample

Una muestra de los datos en formato tabular con dos opciones de visualizacion: Primeras Filas y Ultimas Filas.

### E. Duplicate Rows

Valores duplicados organizados de mayor a menor



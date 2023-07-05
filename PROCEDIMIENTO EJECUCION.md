## PROCEDIMIENTO EJECUCION PARA LOGRAR LOS OBJETIVOS PROPUESTOS

#### - CASO: EMPRESA TELECOMUNICACIONES ARGENTINA

#### - FUENTE DE DATOS:  ENACOM (Entidad Nacional de Telecomunicaciones) https://datosabiertos.enacom.gob.ar/dashboards/20000

#### - METODOLOGIA : KIMBALL

#### OBJETIVO PRINCIPAL EMPRESA

- Acceso a servicios

#### OBJETIVOS SECUNDARIOS EMPRESA

- Calidad de servicio
- Identificar oportunidades de crecimiento
- Plantear soluciones personalizadas a sus posibles clientes

#### REQUERIMIENTO PRINCIPAL DEL CLIENTE. (ROL A EJECUTAR)

- Analisis del sector telecomunicaciones a nivel nacional para lograr **Objetivo Principal** y **Secundarios**

#### PROCEDIMIENTO

#### I.    Extraccion de Datos

Ejecutamos 
#### II.   EDA (Exploratory Data Analysis)

Realizamos EDA con libreria de python **y_dataprofiling**
- Cargamos archivos csv de datasets principal y los convertimos a df para proceder a hacer reporte de analisis con la libreria
- A partir del reporte ejecutamos transformaciones en power query de POWER BI
- Armamos modelo de datos, tablas y sus relaciones

  1) report700.html (AccesosaInternetfijoportecnologiaylocalidad_2791751688443409700.csv)
     Transformaciones ejecutadas
     a) Eliminacion columna 13
     b) Cambio valores -0 a 0
     c) Cambio de tipo numerico de texto a numero en casi todas las columnas

  2) report653.html (AccesosaInternetfijoporvelocidaddebajadaylocalidad_2776171688443389653.csv)
     Transformaciones ejecutadas
     a) Eliminacion columna 13
     b) Cambio valores -0 a 0
     c) Cambio de tipo numerico de texto a numero en casi todas las columnas
- 
#### III.  Visualizaciones

- POWER BI
- ANALISIS DE DASHBOARDS

#### IV.   Definicion de KPI's

- 




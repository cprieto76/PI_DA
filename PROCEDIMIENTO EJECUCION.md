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
     - a) Eliminacion columna 13
     - b) Cambio valores -0 a 0
     - c) Cambio tipo de texto a numero entero en casi todas las columnas quedando las columnas de la tecnologia especifica todas con ese tipo

  3) report653.html (AccesosaInternetfijoporvelocidaddebajadaylocalidad_2776171688443389653.csv)

     Transformaciones ejecutadas
     - a) Abrir en excel y colocar texto en columnas separados por comas
     - b) Reemplazo coma con vacios o dejando la casilla vacia
     - c) Cargo el archivo csv modificado en Power Query de Power Bi
     - d) Reemplazo null por 0 por si acaso hay que hacer alguna operacion sobre estas filas
     - e) Reemplazo vacios por 0
     - f) Cambio tipo de texto a numero entero en varias columnas de tal manera que todas las que corresponden a velocidades quedan en tipo entero

  4) report771.html (AccesosaInternetfijoporvelocidadbajadayprovincia_2791741688443333771.csv)

     Transformaciones ejecutadas
     - a) Abrir en excel y colocar texto en columnas separados por comas
     - b) Reemplazo coma con vacios o dejando la casilla vacia
     - c) Cargo el archivo csv modificado en Power Query de Power Bi
     - d) Elimino ultima fila o registro [481] que esta vacio

  5) report771.html (AccesosaInternetfijoporvelocidadbajadayprovincia_2791741688443333771.csv)

     Transformaciones ejecutadas
     - a) Abrir en excel y colocar texto en columnas separados por comas
     - b) Reemplazo coma con vacios o dejando la casilla vacia
     - c) Cargo el archivo csv modificado en Power Query de Power Bi
     - d) Elimino ultima fila o registro [481] que esta vacio
    
#### III.  Visualizaciones

- POWER BI
- ANALISIS DE DASHBOARDS

#### IV.   Definicion de KPI's

- 




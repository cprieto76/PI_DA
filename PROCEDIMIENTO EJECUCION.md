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

#### II.   Primera Revision General EDA 1 (Exploratory Data Analysis)

Realizamos EDA con libreria de python **y_dataprofiling** centrandonos en Overview (Filas Duplicadas, Tipos de Datos, , Celdas Vacias, Ceros) y Alertas (Variables sin Nombre, Valores Unicos, Zeros, Valores faltantes, Valores Unicos).
El analisis detallado variable por variable se realiza en una segunda fase, luego de haber cargado los datasets en POWER BI para poderlos visualizar y confirmar que han cargado.

- Cargamos archivos csv de datasets principal y los convertimos a df para proceder a hacer reporte de analisis con la libreria
- A partir del reporte ejecutamos transformaciones en power query de POWER BI
- Armamos modelo de datos, tablas y sus relaciones

  ##### 1) report700.html .    (700AccesosaInternetfijoportecnologiaylocalidad700.csv)

     Transformaciones ejecutadas
     - a) Eliminacion columna 13
     - b) Cambio valores -0 a 0
     - c) Cambio tipo de texto a numero entero en casi todas las columnas quedando las columnas de la tecnologia especifica todas con ese tipo

  ##### 2) report653.html     (653AccesosaInternetfijoporvelocidaddebajadaylocalidad653.csv)

     Transformaciones ejecutadas
     - a) Abrir en excel y colocar texto en columnas separados por comas
     - b) Reemplazo coma con vacios o dejando la casilla vacia
     - c) Cargo el archivo csv modificado en Power Query de Power Bi
     - d) Reemplazo null por 0 por si acaso hay que hacer alguna operacion sobre estas filas
     - e) Reemplazo vacios por 0
     - f) Cambio tipo de texto a numero entero en varias columnas de tal manera que todas las que corresponden a velocidades quedan en tipo entero

  ##### 3) report771.html     (771AccesosaInternetfijoporvelocidadbajadayprovincia771.csv)

     Transformaciones ejecutadas
     - a) Abrir en excel y colocar texto en columnas separados por comas
     - b) Reemplazo coma con vacios o dejando la casilla vacia
     - c) Cargo el archivo csv modificado en Power Query de Power Bi
     - d) Elimino ultima fila o registro [481] que esta vacio

  ##### 4) report977.html       (977mapa_conectividad.xlsx)

     Transformaciones ejecutadas
     
     - a) Coloco nombres de campos que no aparecen. Los nombres de esos campos se encuentran en archivo *mapa_conectividad.xls*  
         dentro de la URL:https://datosabiertos.enacom.gob.ar/visualizations/29951/conectividad-al-servicio-de-internet/
     - b) Corregir valores mal digitados en campos Latitud y Longitud
     - c) Tipo de dato y signo menos de Latitud y Longitud convertir a numero
     - d) Datos tipo texto y numero los cambio
     - e) Cargo el archivo csv modificado en Power Query de Power Bi

  ##### 5) report300.html       (300Internet_Penetracion (1).csv)

      Transformaciones ejecutadas
  
     - a) Abrir en excel y cambio tipo de dato de texto a numero 
     - b) Cargo el archivo csv modificado en Power Query de Power Bi
          
  ##### 6) report301.html       (301Internet_Penetracion.csv)

     Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero 
     - b) Cargo el archivo csv modificado en Power Query de Power Bi

  ##### 7) report400.html       (400Internet_Ingresos.csv)

     Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Cargo el archivo csv modificado en Power Query de Power Bi

  ##### 8) report500.html       (500Internet_BAF(provincia).csv)

     Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Cargo el archivo csv modificado en Power Query de Power Bi

 ##### 9) report501.html         (501Internet_BAF.csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Cargo el archivo csv modificado en Power Query de Power Bi

 ##### 10) report600.html         (600Internet_Accesos-por-velocidad(provincia).csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Cargo el archivo csv modificado en Power Query de Power Bi   

  ##### 11) report601.html         (601Internet_Accesos-por-velocidad.csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Cargo el archivo csv modificado en Power Query de Power Bi   

  ##### 12) report800.html         (800historico_velocidad_internet(provincia).csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Cargo el archivo csv modificado en Power Query de Power Bi  

  ##### 13) report801.html         (801historico_velocidad_internet.csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Cargo el archivo csv modificado en Power Query de Power Bi 

  ##### 14) report900.html         (900Internet_Accesos-por-tecnologia(provincia).csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Se borra ultima fila
     - b) Cargo el archivo csv modificado en Power Query de Power Bi 

  ##### 15) report901.html         (901Internet_Accesos-por-tecnologia.csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Se corrigen datos numericos que tienen un asterisco (*). Se borra
     - b) Cargo el archivo csv modificado en Power Query de Power Bi 

  *	Los datos provinciales no coinciden a nivel nacional, ya que se reincorpora informacionn que no contiene apertura a nivel geografico.

  ##### 16) report185.html (5) (185Listadodelocalidadesconconectividadainternet185.csv)

  La información ya se encuentra en reporte 977 correspondiente a acceso de tecnologias por localidad, por lo cual no se carga a POWER BI

#### III.  Segunda Revision General EDA 2 (Exploratory Data Analysis

Con esta libreria volvemos a generar los reportes html y revisamos variable por variable. (Outliers y Correlaciones)

##### 1) report700.html .    (700AccesosaInternetfijoportecnologiaylocalidad700.csv)

    Revision  
    - a) Se revisa variable por variable  
    Tipo de dato  
    - b) Tipo de dato se cambia para todas las tecnologias de texto a numero en Excel  
    

  ##### 2) report653.html     (653AccesosaInternetfijoporvelocidaddebajadaylocalidad653.csv)

     Este archivo se va a descartar para el analisis y cargue en POWER BI ya que tenemos el report600 (Provincias y rangos de velocidad) y  
     el report771 (Provincia y velocidades individuales) que pueden suplir la informacion para nuestro analisis

  ##### 3) report771.html     (AccesosaInternetfijoporvelocidadbajadayprovincia_2791741688443333771.csv)

     Transformaciones ejecutadas
     - a) Abrir en excel y colocar texto en columnas separados por comas
     - b) Reemplazo coma con vacios o dejando la casilla vacia
     - c) Cargo el archivo csv modificado en Power Query de Power Bi
     - d) Elimino ultima fila o registro [481] que esta vacio

  ##### 4) report977.html       (977mapa_conectividad.xlsx)  

     -  Pendiente revisarcambiamos los SI por 1 y los vacios por 0 
     - e) Cargo el archivo csv modificado en Power Query de Power Bi

  ##### 5) report300.html       (300Internet_Penetracion (1).csv)

     Revision
  - a) Se revisa variable por variable
    Tipo de dato
  - b) Tipo de dato de "Accesos por cada 100 hogares" se cambia de Date a Numerico en Excel
  - **OUTLIERS**
  - c) Se revisan Outliers en "Accesos por cada 100 hogares"
    Q1-1.5IQR    =33.38
  - Q3+1.5IQR    =85.65
  **No se encuentran outliers**
  - d) Tampoco hay **outliers** para "Accesos por cada 100 hab"
  - e) Cargo el archivo csv modificado en Power Query de Power Bi

    ##### 6) report301.html       (301Internet_Penetracion.csv)

    - Se realizan la revision variable por variable luego de cambiar datos de tipo texto a numerico
    - Se encuentran porcentajes de penetracion superiores al 100% que segun fuente consultada  
      (https://chequeado.com/ultimas-noticias/gladys-gonzalez-en-argentina-1-de-cada-3-hogares-no-tiene-acceso-a-internet/) se debe a que los prestadores   
      de servicios reportan la cantidad de accesos de Enacom de los cuales muchos son comercios o empresas.  

      Que hace falta para tener datos mas fidedignos:  
      
      - Saber cuantos comercios o empresas acceden a banda ancha (Se disminuirian accesos a hogares)
      - Saber cuales de esos comercio o empresas no estan integrados a propiedades que tambien funcionan como hogares (Aumentarian accesos a hogares)
      - Poder acceder al 100% de las empresas prestadoras de servicios telcom (Aumentarian accesos a hogares)
      - Subdeclaración de clientes por muchas empresas (Aumentarian accesos a hogares)    

  ##### 7) report400.html       (400Internet_Ingresos.csv)

     Transformaciones ejecutadas
     - a) Abrir en excel y adiciono dos columnas, "Incremento Neto" e "Incremento Porcentual"
     - b) Genero reporte html  y reviso Alertas variable por variable
     - c) Cargo el archivo csv modificado en Power Query de Power Bi

  ##### 8) report500.html       (500Internet_BAF(provincia).csv)

  El porcentaje de Banda ancha respecto a Dial Up es del 97 al 100%

  ##### 9) report501.html         (501Internet_BAF.csv)
   
    - Agregamos dos columnas: "Incremento Porcentual Banda Ancha", "Incremento Porcentual Dial Up"

 ##### 10) report600.html         (600Internet_Accesos-por-velocidad(provincia).csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Cargo el archivo csv modificado en Power Query de Power Bi   

  ##### 11) report601.html         (601Internet_Accesos-por-velocidad.csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Cargo el archivo csv modificado en Power Query de Power Bi   

  ##### 12) report800.html         (800historico_velocidad_internet(provincia).csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Cargo el archivo csv modificado en Power Query de Power Bi  

  ##### 13) report801.html         (801historico_velocidad_internet.csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Cargo el archivo csv modificado en Power Query de Power Bi 

  ##### 14) report900.html         (900Internet_Accesos-por-tecnologia(provincia).csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Se borra ultima fila
     - b) Cargo el archivo csv modificado en Power Query de Power Bi 

  ##### 15) report901.html         (901Internet_Accesos-por-tecnologia.csv)
   
    Transformaciones ejecutadas
     - a) Abrir en excel y cambio tipo de dato de texto a numero y al contrario
     - b) Se corrigen datos numericos que tienen un asterisco (*). Se borra
     - b) Cargo el archivo csv modificado en Power Query de Power Bi 

#### IV.  Visualizaciones

- POWER BI
- ANALISIS DE DASHBOARDS

#### V.   Definicion de KPI's

1) ARPU (Average Revenue Per User, por sus siglas en inglés): El ARPU mide los ingresos promedio generados por cada abonado. Puedes calcularlo dividiendo los ingresos totales de los servicios de telecomunicaciones entre el número total de abonados durante un período determinado.

2) Tasa de crecimiento de abonados: Este KPI muestra la velocidad a la que la operadora está adquiriendo nuevos abonados a lo largo del tiempo. Puedes calcularlo dividiendo el cambio neto en el número de abonados entre el número total de abonados al comienzo del período y multiplicarlo por 100 para obtener un porcentaje. Un crecimiento constante o creciente indica una demanda sostenida de los servicios de la operadora.

3) KPI basado en cobertura de los otros servicios




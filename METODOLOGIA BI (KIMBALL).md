## METODOLOGIA KIMBALL

Metodología de diseño y construcción de Datawarehouse (DW). 

Se llama "bottom-up" (de abajo hacia arriba) porque se centra en la construcción gradual y progresiva de un almacén de datos a partir de componentes individuales.

La metodología se basa en el **Ciclo de Vida Dimensional del Negocio**.

Este ciclo de vida del proyecto de DW, está basado en cuatro principios básicos:

- **Centrado en el negocio**: Conocimiento profundo acerca del negocio
- **Infraestructura de información**: Análisis a fondo de la información a analizar para generar los modelos adecuados para los datamarts.
- **Entregas con incrementos significativos**:Se deben hacer entregas en plazos acordados que no sean tan extensos ni tan cortos.
- **Solución completa**: Se debe hacer una entrega de un diseño funcional, con las 
herramientas de consulta, aplicaciones gráficas para informes, capacitación y soporte

![image](https://github.com/cprieto76/PI_DA/assets/115907710/2d32aef4-5b47-40d9-8224-492bfc81a0d8)

### CAPAS DE METODOLOGIA

### a) **Capa de Planificación**

*Actividades*:

- Definir el alcance.
- Identificar y programar las tareas.
- Planificación del uso de los recursos.
- Asignación de trabajo a los recursos.
- Elaboración del documento de plan de proyecto.

b) **Capa de definición de requerimientos**

Los requerimientos especifican qué es lo que el sistema debe hacer (sus funciones) y sus propiedades esenciales y deseables.

La captura de los requerimientos tiene como objetivo principal la comprensión de lo que los clientes y los usuarios esperan que haga el sistema.

c) **Capa de modelado Dimensional**

Es un proceso iterativo que consta de 4 pasos:

1) **Elegir el proceso de negocio**

2) **Establecer el nivel de granularidad o nivel de detalle**

3) **Elegir las dimensiones**

4) **Identificar las tablas de hechos y medidas**

d) **Capa de Diseño Físico**

Dimensionamiento a nivel de servidores, procesadores, memoria a utilizar, almacenamiento,
sistemas de respaldo, e instalación de software en los diferentes servidores

e) **Capa de diseño e Implementación del Subsistema de ETL**
 
Identificar y recopilar la información inicial de los datos fuente, clasificar la información realizando la respectiva depuración, extrayendo los registros que no contengan cierto grado requerido de calidad y realizando las adecuaciones pensando en su visualización final, para posteriormente cargar la información procesada en el modelo diseñado

f) **Capa de implementación**

Implementación de todo el modelo, lo cual implica la convergencia del diseño lógico, diseño físico y la visualización de la solución hacia los usuarios de negocio. Es importante tener en cuenta aspectos como la capacitación, el soporte y las estrategias para el crecimiento y mantenimiento de la solución.

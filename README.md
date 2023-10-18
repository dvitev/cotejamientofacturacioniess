# **Cotejamiento de Afiliados contra Archivos Planos de Facturación**

Este proyecto realiza el cotejamiento de las cédulas de afiliados contra los archivos planos de facturación del Hospital General Milagro, con el fin de facilitar el control y seguimiento de las atenciones médicas de los afiliados.

### **Importancia de los Archivos Planos de Facturación**
-----------------------------------------------------

Los archivos planos de facturación son la fuente de información primaria para el monitoreo y control de las atenciones médicas brindadas en las unidades del IESS.

Su análisis exhaustivo permite detectar inconsistencias, mejorar procesos internos y generar indicadores para la toma de decisiones.

La digitalización de estos archivos abre las puertas al uso de técnicas de Big Data y ciencia de datos para extraer su valor.


### **Procesamiento de Grandes Volúmenes de Datos con Python**
----------------------------------------------------------

Lenguajes como Python y herramientas como Pandas permiten manipular y analizar eficientemente los millones de registros contenidos en los archivos planos de facturación.

La aplicación de buenas prácticas como las empleadas en este notebook hacen viable el procesamiento en tiempo récord de años completos de información.

Estas capacidades amplían el horizonte analítico y permiten generar nuevos insights para la mejora continua de procesos y servicios.

**Introducción**
----------------

Los archivos planos de facturación generados mensualmente por las unidades médicas del IESS contienen información valiosa sobre las atenciones realizadas a los afiliados. El análisis de estos archivos permite monitorear indicadores, detectar anomalías y optimizar procesos.

Este notebook ejemplifica cómo utilizar Python y Pandas para procesar y analizar eficientemente los grandes volúmenes de datos contenidos en los archivos planos de facturación. Las técnicas aplicadas facilitan la manipulación de millones de registros en pocos minutos.

**Descripción** 
---------------

El notebook `alamos-201702-201812.ipynb` realiza los siguientes pasos:

* Importación de librerías esenciales como Pandas.

* Carga masiva de archivos CSV mensuales de facturación del Hospital General Milagro 2017-2021.

* Limpieza y formateo de columnas críticas como cédulas e identificaciones.

* Cotejamiento de cada cédula del listado de afiliados contra la columna 'IDENTIFICACION_AFILIADO' de los archivos planos.

* Filtrado y almacenamiento incrementales de los resultados positivos en archivos CSV mensuales.

* Posterior agregación y consolidación de registros mensuales relacionados a cada afiliado.

* Inserción de totales y sumatorias a nivel de afiliado en el listado principal. 

* Generación de reporte final con los resultados del cruce y enriquecimiento de datos.


**Requisitos**
--------------

* Python 3.6 o superior

* Pandas

* OpenPyXL


**Uso**
-------

Para ejecutar el notebook:

`jupyter notebook alamos-201702-201812.ipynb`

Los archivos CSV de entrada deben estar en la carpeta `/HG Milagro` con nombres como `HG_MI_201701.csv`.

El archivo Excel de entrada debe estar en el mismo directorio con el nombre `IESS-CPPCG-2023-2144-A.xls`.

Los resultados se guardarán en `/periodos` y `alamos-201702-201812-procesado.xlsx`.


**Licencia**
------------

LGPL 2.1

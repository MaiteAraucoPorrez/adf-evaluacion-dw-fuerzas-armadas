# adf-evaluacion-dw-fuerzas-armadas

# Descripción:

Las Fuerzas Armadas de Bolivia cuentan con un sistema operacional (OLTP) que registra el día a día de la institución: el ingreso de nuevos efectivos, los traslados entre unidades, los ascensos de rango, y cada operación militar desplegada en el territorio nacional, desde el patrullaje fronterizo en el Desaguadero hasta las operaciones de defensa civil ante los incendios forestales en la Chiquitanía.

Este sistema fue desarrollado hace años por diferentes equipos técnicos y, como ocurre en muchas organizaciones reales, los datos no están en las mejores condiciones.

El Comando General necesita responder preguntas como: ¿cuántos efectivos se trasladaron por departamento en los últimos tres años? ¿Cuál es el costo promedio de las operaciones antinarcóticos comparado con las de defensa civil? ¿En qué meses del año se concentran más operaciones y cómo se relaciona eso con el presupuesto ejecutado? ¿Qué unidades tienen mayor rotación de personal? Para responder estas preguntas, necesitan un Data Warehouse.

# Stack Azure 
- Grupo de Recurso
- Sql Database
- Azure Datafactory
Todos los servicios estan automatizados con terraform
 
# Arquitectura

- Bronze -> datos crudos
- Silver -> limpieza e integración de los datos
- Gold -> creacion del datawarehouse etl & pipelines

# Método 2
 
	- raw -> datalake - datos en brutos
	- bronze -> schema bronze - dw_ventas
	- silver -> schema silver
	- gold -> schema gold y datawarehouse

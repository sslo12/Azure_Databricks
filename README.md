# Azure_Databricks
Con base en la arquitectura lakehouse desplegada previamente en Databricks, se migro el pipeline de datos desarrollado en el segundo proyecto basado en arquitectura open source. En este caso, no se uso dlt para ingestar de datos sino que debe ser mediante cualquier otra librería de python, puede ser request o leer el archivo con pyarrow. Adicionalmente, solo se debe usar un año para los datos ya que no queremos procesar tantas cantidades de datos y procurar ahorrar en los créditos. Usar al menos dos meses por tabla. El proyecto debe implementar la arquitectura Medallion (Bronze → Silver → Gold) con lógica de ingesta, transformación, calidad de datos y agregación.

# Infraestructura Requerida:
● Azure data lake Gen 2 (object storage)
● Unity Catalog (catálogo de metadatos)
● Delta table (table format)
● Apache Spark con PySpark (procesamiento)
● Databricks Jobs (orquestación)
● Databricks Notebook (ejecución manual alterna)
● Uso de DuckDB para consultar las tablas delta de silver y gold.

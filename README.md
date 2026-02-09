# Proyecto de Automatización de Datos en Odoo con Python

## Descripción del Proyecto

Este proyecto tiene como objetivo automatizar la importación de datos de un archivo CSV que contiene información sobre centros educativos en una base de datos PostgreSQL de Odoo. Utilizando un script Python, el proceso ETL (Extracción, Transformación y Carga) lee el archivo CSV, lo procesa y carga en la base de datos, creando la tabla necesaria si no existe.

## Tecnologías Utilizadas

- **Python 3.10+** para el desarrollo del script.
- **pandas** para la manipulación y procesamiento de los datos del archivo CSV.
- **psycopg2-binary** para la conexión con la base de datos PostgreSQL.
- **Docker** para ejecutar los contenedores de Odoo y PostgreSQL.
- **pgAdmin** (opcional) para verificar los datos cargados en la base de datos.

## Procedimiento

1. **Configurar el Entorno**:
   - Asegúrate de tener **Docker Desktop** corriendo con los contenedores de **Odoo** y **PostgreSQL** activos.
   - Instala las dependencias necesarias, como `pandas` y `psycopg2-binary`, utilizando un entorno virtual en Python.

2. **Ejecutar el Script**:
   - Coloca el archivo `listado.csv` en el directorio donde está el script `importar.py`.
   - Ejecuta el script para procesar y cargar los datos a la base de datos PostgreSQL de Odoo.

3. **Verificación de los Datos**:
   - Una vez ejecutado el script, usa **pgAdmin** para verificar que los datos se han cargado correctamente en la tabla `import_centros` mediante una consulta `SELECT`.



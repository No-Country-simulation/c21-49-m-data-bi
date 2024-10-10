# Documentación de los datos

En esta carpeta se encuentran los datos utilizados en el proyecto de análisis de datos sobre la violencia en América Latina.

## Estructura de carpetas

- **/raw/**: Contiene los datos de las bases de datos utilizadas en el proyecto.
  - `base_de_datos.txt`: En este archivo se encuentra el enlace a la base de datos original. Es necesario tener cuenta en Armed Conflict Location and Event Data (ACLED) para su uso.
- **/processed/**: Contiene los datos limpios de la base de datos original.
  - `_dbLimpia04Oct.csv`: En este archivo se encuentran los datos procesados y limpios, listos para analizar. Los datos corresponden al 4 de octubre del 2024.

## Descripción de los archivos

### Datos originales

- `base_de_datos.txt`: Muestra un enlace para acceder a la base de datos externa. Para acceder a la base de datos es necesario hacer lo siguiente:

#### Para usuarios registrados
1. Abrir el archivo `\raw\base_de_datos.txt`.
2. Copiar la URL que se encuentra dentro del archivo.
3. Presionar el botón `Download File`.
4. Colocar la API Key y el correo electrónico con el cual están registrados.
5. Presionar `Submit`, para descargar la base de datos original.

#### Para usuarios no registrados
1. Ingresar a https://developer.acleddata.com/
2. Registrarse con tus datos y validar el mail que llega a la dirección de correo indicada.
3. En el menú `Dashboard`, seleccionamos la opción `Add New Key` para obtener una API.
4. Guardar la API mostrada porque no puede ser regenerada. Se deberá solicitar otra.
5. Abrir el archivo `\raw\base_de_datos.txt`.
6. Copiar la URL que se encuentra dentro del archivo.
7. Presionar el botón `Download File`.
8. Colocar la API Key y el correo electrónico con el cual están registrados.
9. Presionar `Submit`, para descargar la base de datos original.

### Datos procesados

- **`_dbLimpia04Oct.csv`**: Incluye los datos finales a utilizar en este proyecto.

## Notas sobre el procesamiento

### Limpieza de datos
Se eliminaron columnas con valores innecesarios para el análisis, como `timestamp`, `tags`, `source`, `iso`, `admin2`, `admin3`, `time_precision`, `geo_precision`, `notes` y `event_id_cnty`.

## Diccionario de datos
Para los datos en crudo, el diccionario de datos (codebook) para este proyecto se encuentra en la [página de ACLED](https://acleddata.com/knowledge-base/codebook/).

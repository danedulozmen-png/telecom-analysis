# Proyecto Final Sprint 7 - Análisis de Clientes ConnectaTel

## Descripción del Proyecto

El objetivo de este proyecto es analizar el comportamiento de los clientes de ConnectaTel a partir de información demográfica y registros de uso del servicio. Se realizó un proceso de limpieza, exploración, segmentación y análisis de datos para identificar patrones de comportamiento y oportunidades de negocio.

## Datasets Utilizados

### users

Contiene información de los clientes:

* user_id
* first_name
* last_name
* age
* city
* reg_date
* plan
* churn_date

### usage

Contiene información de uso de los servicios:

* id
* user_id
* type
* date
* duration
* length

## Etapas del Análisis

### 1. Exploración Inicial

* Identificación de valores nulos.
* Identificación de sentinels.
* Revisión de tipos de datos.
* Análisis de variables numéricas y categóricas.

### 2. Limpieza de Datos

* Reemplazo de edades inválidas (-999).
* Conversión de sentinels en valores nulos.
* Corrección de fechas fuera de rango.
* Verificación de nulos tipo MAR (Missing At Random).

### 3. Ingeniería de Características

* Agregación de métricas de uso por usuario.
* Creación de:

  * cant_mensajes
  * cant_llamadas
  * cant_minutos_llamada

### 4. Análisis Exploratorio

* Estadísticas descriptivas.
* Histogramas.
* Boxplots.
* Detección de outliers mediante IQR.

### 5. Segmentación de Clientes

* Segmentación por edad:

  * Joven
  * Adulto
  * Adulto Mayor

* Segmentación por nivel de uso:

  * Bajo uso
  * Uso medio
  * Alto uso

### 6. Insights de Negocio

* Identificación de segmentos relevantes.
* Detección de usuarios de alto consumo.
* Recomendaciones para optimizar la oferta de planes.

## Principales Hallazgos

* La mayoría de los clientes pertenece al segmento Adulto.
* La mayoría de los usuarios presenta un nivel de Uso medio.
* Se identificaron usuarios con consumos significativamente superiores al promedio.
* Los outliers detectados representan comportamientos reales y fueron conservados para el análisis.

## Cómo Ejecutar el Proyecto

### Opción 1: Google Colab

1. Descargar el archivo `.ipynb`.
2. Abrir Google Colab.
3. Seleccionar "Subir Notebook".
4. Ejecutar las celdas en orden.

### Opción 2: Jupyter Notebook

1. Clonar el repositorio.
2. Instalar las librerías necesarias:

   * pandas
   * numpy
   * matplotlib
   * seaborn
3. Abrir el notebook.
4. Ejecutar las celdas secuencialmente.

## Autor

Daniel Lozano
Bootcamp de Análisis de Datos

git add .
git commit -m "feat: final ConnectaTel customer analysis"
git push

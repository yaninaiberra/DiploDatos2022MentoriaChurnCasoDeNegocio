# DiploDatos 2022 - Mentoría "Churn Prediction: ¿Cómo retengo a mis clientes? Machine Learning aplicado a un caso de negocio"

La pérdida de clientes puede ser complicada para las empresas. En este proyecto, desarrollaremos un modelo de aprendizaje automático para ayudar a predecir aquellos clientes que cancelarán la suscripción a una plataforma de streaming de música, y poder con ello implementar alguna estrategia de marketing para retenerlos con anticipación a su posible abandono del servicio.


## Datos

**Conjunto de datos de actividad de los usuarios de [Udacity](https://www.udacity.com/) <br>**

El conjunto de datos registra la información demográfica de los usuarios (por ejemplo, nombre del usuario, sexo, estado) y la actividad con la plataforma (por ejemplo, canción escuchada, tipo de evento, dispositivo utilizado) en marcas de tiempo individuales.

Estos datos se utilizarán para el análisis y el entrenamiento del modelo:

mini_sparkify_event_data.zip
+ [(```mini_sparkify_event_data.zip```)](data/raw/mini_sparkify_event_data.zip): El cual contiene zipeados 543705 registros de actividad de usuarios de una plataforma de streaming de música, ésta información es ficticia y proviene de un curso de Udacity.

### Estructura

root
 |-- artist: string (nullable = true)
 |-- auth: string (nullable = true)
 |-- firstName: string (nullable = true)
 |-- gender: string (nullable = true)
 |-- itemInSession: long (nullable = true)
 |-- lastName: string (nullable = true)
 |-- length: double (nullable = true)
 |-- level: string (nullable = true)
 |-- location: string (nullable = true)
 |-- method: string (nullable = true)
 |-- page: string (nullable = true)
 |-- registration: long (nullable = true)
 |-- sessionId: long (nullable = true)
 |-- song: string (nullable = true)
 |-- status: long (nullable = true)
 |-- ts: long (nullable = true)
 |-- userAgent: string (nullable = true)
 |-- userId: string (nullable = true)

# DiploDatos 2022 - Mentoría "Churn Prediction: ¿Cómo retengo a mis clientes? Machine Learning aplicado a un caso de negocio"

La pérdida de clientes puede ser complicada para las empresas. En este proyecto, desarrollaremos un modelo de aprendizaje automático para ayudar a predecir aquellos clientes que cancelarán la suscripción a una plataforma de streaming de música, y poder con ello implementar alguna estrategia de marketing para retenerlos con anticipación a su posible abandono del servicio.


## Datos

**Conjunto de datos de actividad de los usuarios de [Udacity](https://www.udacity.com/) <br>**

Sparkify es un falso servicio de streaming de música inventado por Udacity. En él, los usuarios pueden escuchar música de forma gratuita (con anuncios entre canciones) o por una tarifa plana. Los usuarios pueden subir, bajar de categoría o cancelar. EL objetivo será predecir el usuario que se va a ir para ofrecerle un gran descuento antes de cancelar la suscripción.

El conjunto de datos registra la información demográfica de los usuarios (por ejemplo, nombre del usuario, sexo, estado) y la actividad con la plataforma (por ejemplo, canción escuchada, tipo de evento, dispositivo utilizado) en marcas de tiempo individuales.

Estos datos se utilizarán para el análisis y el entrenamiento del modelo:

mini_sparkify_event_data.zip
+ [(```mini_sparkify_event_data.zip```)](data/raw/mini_sparkify_event_data.zip): El cual contiene zipeados 543705 registros de actividad de usuarios de con la plataforma de streaming de música.


### Estructura

```
  artist: string - artist name
  auth: string  - authentification method
  firstName: string - user first name
  gender: string - user gender
  itemInSession: long
  lastName: string - user last name
  length: double - length of the song listened
  level: string - sparkifiy user service level (paid or free)
  location: string - location of the user
  method: string - http service method
  page: - user service interaction event 
  registration: long - timestamp of user service registration 
  sessionId: service session id
  song: song name played by the user
  status: - http status
  ts: long - timestamp of user service event 
  userAgent: - web browser used
  userId: string - unique userid 
```

<ins>Los features del conjunto de datos pueden dividirse en cuatro categorías </ins>:
  * **User information** : userid, first name, last name, gender, location
  * **Sparkify service information** : level, registration
  * **User service event/interactions information** : method, iteminsession, page, status, ts, useragent, sessionid
  * **Songs & artist informations** : artist, song, length
  

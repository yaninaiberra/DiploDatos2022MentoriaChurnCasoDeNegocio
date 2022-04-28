# DiploDatos 2022 - Mentoría "Churn Prediction: ¿Cómo retengo a mis clientes? Machine Learning aplicado a un caso de negocio"

La pérdida de clientes puede ser complicada para las empresas. En este proyecto, desarrollaremos un modelo de aprendizaje automático para ayudar a predecir aquellos clientes que cancelarán la suscripción a una plataforma de streaming de música, y poder con ello implementar alguna estrategia de marketing para retenerlos con anticipación a su posible abandono del servicio.


## Datos

**Conjunto de datos de actividad de los usuarios de [Udacity](https://www.udacity.com/) <br>**

Sparkify es un falso servicio de streaming de música inventado por Udacity. En él, los usuarios pueden escuchar música de forma gratuita (con anuncios entre canciones) o por una tarifa plana. Los usuarios pueden subir, bajar de categoría o cancelar. El objetivo será predecir el usuario que se va a ir para ofrecerle un gran descuento antes de cancelar la suscripción.

El conjunto de datos registra la información demográfica de los usuarios (por ejemplo, nombre del usuario, sexo, estado) y la actividad con la plataforma (por ejemplo, canción escuchada, tipo de evento, dispositivo utilizado) en marcas de tiempo individuales.

Estos datos se utilizarán para el análisis y el entrenamiento del modelo:

mini_sparkify_event_data.zip
+ [(```mini_sparkify_event_data.zip```)](data/raw/mini_sparkify_event_data.zip): El cual contiene zipeados 543705 registros de actividad de usuarios de con la plataforma de streaming de música.


### Estructura

**Información a nivel de usuario**

Estas columnas contienen datos sobre los usuarios: sus nombres, sexo, ubicación, fecha de registro, navegador y nivel de cuenta (paga o gratuita).

- userId (string): user’s id
- firstName (string): user’s first name
- lastName (string): user’s last name
- gender (string): user’s gender, 2 categories (M and F)
- location (string): user’s location
- userAgent (string): agent (browser) used by the user
- registration (int): user’s registration timestamp
- level (string): subscription level, 2 categories (free and paid)serId: string - unique userid 


**Información específica del uso de la plataforma**

Muestra cómo interactúa un usuario concreto con el servicio.

- ts (int): timestamp of the log
- page (string): type of interaction associated with the page (NextSong, Home, Login, Cancellation Confirmation, etc.)
- auth (string): authentication level, 4 categories (Logged In, Logged Out, Cancelled, Guest)
- sessionId (int): a session id
- itemInSession (int): log count in the session
- method (string): HTTP request method, 2 categories (GET and PUT)
- status (int): HTTP status code, 3 categories (200, 307 and 404)

**Información a nivel de canción**

- song (string): song name
- artist (string): artist name
- length (double): song’s length in seconds


  

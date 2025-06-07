# Timestamp Microservice

Este proyecto es parte del curso **Back End Development and APIs** de [freeCodeCamp](https://www.freecodecamp.org/), reto **"Microservicio de marca de tiempo"**.

## 📚 Descripción del reto

El objetivo de este reto es construir un **microservicio** funcionalmente similar al que se encuentra en:

👉 [https://timestamp-microservice.freecodecamp.rocks](https://timestamp-microservice.freecodecamp.rocks)

Este microservicio debe aceptar una fecha como parámetro (en formato UNIX o ISO) y devolver una respuesta en formato JSON con la fecha en formato UNIX y UTC.

## 🚀 ¿Qué hace este microservicio?

El servicio expone una API que responde a las siguientes rutas:

- `/api/:date`  
  → Acepta una fecha como parámetro. El parámetro puede ser:
  
  - Una fecha en formato `YYYY-MM-DD`, como `2015-12-25`
  - Un timestamp UNIX en milisegundos, como `1451001600000`

  La respuesta será un objeto JSON con este formato:

  ```json
  {
    "unix": 1451001600000,
    "utc": "Fri, 25 Dec 2015 00:00:00 GMT"
  }
  ```

  Si la fecha es inválida, responde con

  ```json
  {
   "error": "Invalid Date"
  }
  ```

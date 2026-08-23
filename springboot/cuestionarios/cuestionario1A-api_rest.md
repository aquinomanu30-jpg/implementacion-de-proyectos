# Cuestionario sobre API REST

## Conceptos Básicos
1. ¿Qué es una API y cuál es su función principal?
API significa Interfaz de Programación de Aplicaciones (Application Programming Interface). Permite la comunicación entre diferentes sistemas de software.
2. Define brevemente el estilo arquitectónico REST.
REST (Representational State Transfer) es un estilo de arquitectura que establece restricciones y recomendaciones para construir APIs. Fue definido por Roy Fielding en el año 2000.
3. ¿Qué significa que una API sea RESTful?
Significa que la API cumple con las restricciones y principios de REST.
## Recursos y URIs
4. ¿Qué es un recurso en el contexto de una API REST?
Un recurso es la información que maneja la API, por ejemplo, usuarios, productos o tareas.
5. Explica la importancia de las URIs en una API REST.
Las URIs permiten identificar de manera única a cada recurso.
Ejemplo:https://api.ejemplo.com/usuarios/123
Esta URI identifica al usuario con ID 123.
6. Menciona tres características importantes de las URIs.
Identifican de manera única un recurso.
Deben ser claras y fáciles de entender.
Permiten acceder a los recursos mediante una dirección única.
7. ¿Por qué es recomendable usar nombres en plural para las URIs que representan colecciones de recursos?
Porque permite identificar que la URI representa una colección de recursos.
## Métodos HTTP
8. ¿Cuáles son los métodos HTTP principales utilizados en una API REST y cuál es la función de cada uno?
GET: consulta o obtiene información.
POST: crea un nuevo recurso.
PUT: actualiza un recurso.
DELETE: elimina un recurso.
9. Describe la diferencia entre los métodos POST y PUT.
POST se utiliza principalmente para crear recursos, mientras que PUT se utiliza para actualizar un recurso específico.
10. ¿Qué significa que un método HTTP sea idempotente? Da un ejemplo de un método idempotente.
Significa que realizar varias veces la misma operación produce el mismo resultado final que realizarla una sola vez.Un ejemplo es PUT.
## Códigos de Estado HTTP
11. ¿Qué indican los códigos de estado en las respuestas HTTP de una API REST?
Indican el resultado de una solicitud HTTP, informando si fue exitosa o si ocurrió algún error.
12. Da un ejemplo de un código de estado para cada una de las siguientes categorías y explica su significado: 
    - 2xx (Éxito)
    - 4xx (Errores del cliente)
    - 5xx (Errores del servidor)

2xx (Éxito): 200 OK  la solicitud se realizó correctamente.
4xx (Errores del cliente): 404 Not Found  el recurso solicitado no fue encontrado.
5xx (Errores del servidor): 500 Internal Server Error  ocurrió un error en el servidor.
## JSON
13. ¿Por qué es JSON el formato de datos más comúnmente utilizado en las APIs REST?
Porque es simple, liviano y fácil de leer y procesar por diferentes lenguajes de programación.
14. Explica brevemente la estructura de un objeto JSON.
Un objeto JSON está formado por pares clave-valor y se encuentra entre llaves { }.
15. ¿Qué tipos de datos pueden representarse en JSON?
JSON puede representar:Texto (String), Números, Booleanos, Null, Objetos y Arrays.
## Postman
16. ¿Qué es Postman y para qué se utiliza en el desarrollo de APIs?
Postman es una herramienta utilizada para probar y realizar solicitudes a APIs.
17. Menciona dos funcionalidades importantes de Postman que facilitan el trabajo con APIs.
Permite enviar solicitudes GET, POST, PUT y DELETE.
Permite ver y analizar las respuestas de la API.
## Ejercicios Prácticos
18. Describe cómo implementarías una operación CRUD (Crear, Leer, Actualizar, Eliminar) en una API REST.
Utilizaría los métodos HTTP:
Crear: POST
Leer: GET
Actualizar: PUT
Eliminar: DELETE
19. ¿Cómo usarías Postman para probar una nueva API que acabas de desarrollar?
Seleccionaría el método HTTP, escribiría la URL del endpoint, enviaría la solicitud y comprobaría la respuesta y el código de estado.
20. Propone un ejemplo de una API REST para gestionar un catálogo de productos y describe brevemente los endpoints necesarios.
GET /productos  consultar todos los productos.
GET /productos/1 : consultar un producto.
POST /productos : crear un producto.
PUT /productos/1 : actualizar un producto.
DELETE /productos/1 : eliminar un producto.

# Cuestionario sobre Spring Framework

## Definición y Origen:
1. ¿Qué es Spring Boot y para qué se utiliza?
Spring Boot es un framework que se utiliza para desarrollar aplicaciones basadas en Java. Es ideal para construir aplicaciones web y servicios de backend.
2. ¿Cuál es la relación entre Spring Boot y el Spring Framework?
Spring Boot funciona como una extensión del Spring Framework, pero simplifica el proceso de configuración y despliegue de las aplicaciones.
3. ¿Para qué tipos de aplicaciones es ideal Spring Boot?
Es ideal para desarrollar aplicaciones web, servicios de backend y aplicaciones independientes.
## Características Principales:
1. ¿Cuál es una de las principales ventajas de usar Spring Boot en términos de configuración?
Una de sus principales ventajas es que reduce la cantidad de configuración necesaria para iniciar una aplicación Spring.
2. ¿Qué significa el principio de "convenio sobre configuración" en el contexto de Spring Boot?
Significa que Spring Boot intenta determinar automáticamente la configuración necesaria basándose en las bibliotecas y dependencias que tiene el proyecto.
3. ¿Cómo ayuda Spring Boot a reducir el tiempo de arranque y desarrollo?
Ofrece configuraciones predeterminadas y automáticas, reduciendo la cantidad de configuración manual y facilitando el desarrollo.
## Ecosistema:
1. ¿Qué otros proyectos forman parte del ecosistema de Spring junto con Spring Boot?
El ecosistema incluye proyectos como Spring Framework, Spring Data, Spring Security y Spring MVC.
2. ¿Cómo facilita Spring Boot la creación de aplicaciones independientes y arquitecturas de microservicios?
Facilita la creación de aplicaciones independientes y simplifica su configuración y despliegue, siendo muy útil para construir arquitecturas de microservicios.
## MVC (Modelo-Vista-Controlador):
1. Describe el rol del Modelo en una aplicación Spring Boot.
El Modelo representa la capa de datos y la lógica de negocio. Está formado por objetos que contienen datos y la lógica relacionada con ellos.
2. ¿Cómo se maneja la capa de datos en el modelo utilizando Spring Boot?
Se utiliza JPA para relacionar los objetos Java con los registros de una base de datos. Spring Data JPA facilita las operaciones comunes sobre los datos, como el CRUD.
3. Explica cómo se genera la Vista en una aplicación Spring Boot.
La Vista se encarga de presentar los datos al usuario. Spring Boot utiliza plantillas para generar el HTML que se muestra en el navegador.
4. ¿Qué tecnologías de plantillas son compatibles con Spring Boot para generar la Vista?
Puede utilizar tecnologías como Thymeleaf, Mustache y JSP.
5. ¿Cuál es la función del Controlador en el patrón MVC y cómo se implementa en Spring Boot?
El Controlador actúa como intermediario entre la Vista y el Modelo. Recibe las solicitudes del usuario, procesa los datos y devuelve una respuesta. En Spring Boot se implementa utilizando @Controller o @RestController.
6. ¿Qué diferencia hay entre un @Controller y un @RestController en Spring Boot?
@Controller se utiliza principalmente para devolver vistas HTML, mientras que @RestController se utiliza principalmente para servicios API y devuelve datos, generalmente en formato JSON o XML.
7. Describe el flujo de trabajo de solicitud/respuesta en una aplicación Spring Boot.
El usuario realiza una solicitud, generalmente HTTP. El Controlador recibe y procesa la solicitud, interactúa con el Modelo si es necesario y luego devuelve una respuesta. Esta puede ser una Vista renderizada o datos.
## Maven:
1. ¿Qué es Maven y para qué se utiliza en proyectos Spring Boot?
Maven es una herramienta de gestión de proyectos utilizada para manejar dependencias, compilar el proyecto y gestionar el ciclo de vida del software.
2. ¿Qué tipo de información se define en el archivo `pom.xml` de un proyecto Spring Boot?
En el pom.xml se definen las dependencias del proyecto, la versión de Spring Boot, los plugins y otras configuraciones necesarias para Maven.
## Configuración de un Proyecto Básico:
1. ¿Qué es Spring Initializr y cómo facilita la generación de un proyecto Spring Boot?
Spring Initializr es una herramienta disponible en start.spring.io que permite generar fácilmente un proyecto Spring Boot. Permite seleccionar la versión de Spring Boot, dependencias, nombre, descripción y tipo de empaquetado, como JAR o WAR.
2. ¿Qué directorios y archivos son importantes en la estructura de un proyecto Spring Boot?
src/main/java contiene el código fuente Java. src/main/resources contiene archivos de configuración, plantillas y archivos estáticos. src/test/java contiene las pruebas. También son importantes application.properties y pom.xml.
3. ¿Cuál es el propósito del archivo `application.properties` en un proyecto Spring Boot?
Sirve para configurar diferentes aspectos de la aplicación, como la base de datos, los parámetros del servidor y otras propiedades personalizadas.
4. ¿Qué anotación se utiliza para marcar la clase principal de una aplicación Spring Boot y qué funciones realiza?
Se utiliza la anotación @SpringBootApplication. Esta incluye las funciones de @Configuration, @EnableAutoConfiguration y @ComponentScan, y actúa como punto de entrada para ejecutar la aplicación.
## Ejemplo Práctico:
1. Describe la estructura de un proyecto Spring Boot utilizando Mustache para las vistas.
El proyecto contiene src/main/java para el código fuente, donde se encuentra MiAplicacion.java y el controlador SaludoControlador.java. En src/main/resources se encuentra la carpeta templates, que contiene saludo.mustache, y el archivo application.properties. También contiene src/test/java para las pruebas y pom.xml para la configuración de Maven.
2. Explica el propósito del controlador `SaludoControlador.java` en el ejemplo proporcionado.
El controlador maneja las solicitudes web y utiliza una vista Mustache para mostrar un saludo. Agrega el mensaje "Hola, Mundo!" al modelo y devuelve la vista llamada "saludo".
3. ¿Cómo se define una plantilla Mustache y cómo se enlaza con el controlador en Spring Boot?
La plantilla Mustache se encuentra en saludo.mustache y utiliza una variable como {{mensaje}}. El controlador agrega el contenido de esa variable mediante model.addAttribute("mensaje", "Hola, Mundo!") y devuelve "saludo", que corresponde al nombre del archivo saludo.mustache.

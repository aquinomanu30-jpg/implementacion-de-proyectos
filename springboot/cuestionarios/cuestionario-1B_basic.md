# Cuestionario sobre Spring Framework

## Definición y Origen:
1. ¿Qué es Spring Boot y para qué se utiliza?
  Es un framework que se utiliza para desarrollar aplicaciones basadas en java. 

3. ¿Cuál es la relación entre Spring Boot y el Spring Framework?
Funciona como una extensión del ya conocido Spring Framework, pero con un enfoque en simplificar el proceso de configuración y despliegue de aplicaciones.

5. ¿Para qué tipos de aplicaciones es ideal Spring Boot?
Es ideal para construir tanto aplicaciones web como servicios backend.

## Características Principales:
1. ¿Cuál es una de las principales ventajas de usar Spring Boot en términos de configuración?
Es su capacidad para minimizar la configuración requerida para arrancar una aplicación Spring.

3. ¿Qué significa el principio de "convenio sobre configuración" en el contexto de Spring Boot?
Significa que intenta adivinar la configuración que necesitas en función de las bibliotecas que tienes en tu classpath.

5. ¿Cómo ayuda Spring Boot a reducir el tiempo de arranque y desarrollo?
Ofrece una configuración predeterminada.

## Ecosistema:
1. ¿Qué otros proyectos forman parte del ecosistema de Spring junto con Spring Boot?
Spring Framework, Spring Data, Spring Security, entre otros.

3. ¿Cómo facilita Spring Boot la creación de aplicaciones independientes y arquitecturas de microservicios?
Despliegue Independiente y microservicios.

## MVC (Modelo-Vista-Controlador):
1. Describe el rol del Modelo en una aplicación Spring Boot.
Consiste en objetos que llevan datos y la lógica relacionada con estos datos.

3. ¿Cómo se maneja la capa de datos en el modelo utilizando Spring Boot?
Se gestiona típicamente mediante JPA (Java Persistence API) para mapear estos objetos a registros de base de datos.

5. Explica cómo se genera la Vista en una aplicación Spring Boot.
en el caso de spring boot, usa plantillas que suelen ser thymeleaf, JSP o Mustache, en general cualquier plantilla compatible

7. ¿Qué tecnologías de plantillas son compatibles con Spring Boot para generar la Vista?
8. ¿Cuál es la función del Controlador en el patrón MVC y cómo se implementa en Spring Boot?
9. ¿Qué diferencia hay entre un @Controller y un @RestController en Spring Boot?
10. Describe el flujo de trabajo de solicitud/respuesta en una aplicación Spring Boot.

## Maven:
1. ¿Qué es Maven y para qué se utiliza en proyectos Spring Boot?
2. ¿Qué tipo de información se define en el archivo `pom.xml` de un proyecto Spring Boot?

## Configuración de un Proyecto Básico:
1. ¿Qué es Spring Initializr y cómo facilita la generación de un proyecto Spring Boot?
2. ¿Qué directorios y archivos son importantes en la estructura de un proyecto Spring Boot?
3. ¿Cuál es el propósito del archivo `application.properties` en un proyecto Spring Boot?
4. ¿Qué anotación se utiliza para marcar la clase principal de una aplicación Spring Boot y qué funciones realiza?

## Ejemplo Práctico:
1. Describe la estructura de un proyecto Spring Boot utilizando Mustache para las vistas.
2. Explica el propósito del controlador `SaludoControlador.java` en el ejemplo proporcionado.
3. ¿Cómo se define una plantilla Mustache y cómo se enlaza con el controlador en Spring Boot?


# Sistema de subsidios
## Introducción
Proyecto en desarrollo para la cátedra de Diseño de Base de Datos, perteneciente a la maestría en Ingeniería de Software (UNLP).

La aplicación Web simula la carga de subsidios para proyectos en la universidad, con el objectivo de crear una aplicación cuyo modelo sea agnóstico de la capa de persistencia utilizada. El modelo será lo más completo posible, sin embargo, la implementación de funcionalidades será acotada a los casos de interés.

Desarrollado utilizando Java, Spring Boot.

## Pre-requisitos
- Instalar Java 1.8+ (http://www.oracle.com/technetwork/java/javase/downloads/index.html)
- Instalar Maven (https://maven.apache.org/download.cgi). Elegir el bin apache-maven-3.5.0-bin.zip, descomprimirlo y agregarlo al path de Windows (Ir a sistema > Opciones avanzadas > Variables de entorno).
	Para probar si la instalación fue correcta probar mvn -v en la línea de comandos.
- Instalar IDE (Spring STS, es una versión basada en Eclipse, se puede bajar de https://spring.io/tools/sts/all)

## Configuración
- En el archivo de Maven pom.xml se pueden agregar dependencias que sean necesarias
- En application.properties también podemos modificar diferentes configuraciones por defecto de Spring
- Hay otros dos application.properties para ambientes de dev y prod, que podrían sobreescribir el application.properties original con algún otro cambio: puerto, db, etc.
- Para cambiar el ambiente en el que se está ejecutando, ir al menú Run>Run Configurations. Elegir Java Application>App, y dentro de este el tab Arguments. En el texto VM arguments cambiar -Dspring.profiles.active=dev por lo que corresponda.
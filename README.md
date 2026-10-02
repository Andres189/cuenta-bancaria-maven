# Cuenta bancaria — Maven

**Autor:** Andrés Juárez Garduño

## Cómo construir y correr

    ./mvnw clean package
    java -jar target/cuenta-bancaria-maven-1.0.0.jar

## Qué hay en este proyecto

| Qué | Dónde |
|---|---|
| El programa (estado de cuenta en texto y en JSON) | `src/main/java/com/academia/banco/App.java` |
| Las pruebas | `src/test/java/com/academia/banco/` |
| La evidencia de cada mini-práctica | `evidencia/` |
| Los 5 errores de Maven que encontré | `evidencia/errores-maven.md` |

## Boleto de salida

1. ¿Qué diferencia hay entre `./mvnw package` y `./mvnw install`?
package compila, ejecuta pruebas y empaquete el proyecto e install hace todo lo anterior y copia él .jar localmente.

2. ¿Por qué `compile` pasó pero `java -jar` falló en la MP-3?
Por qué maven no tiene por defecto las dependencias externas (las de <Dependency>) dentro de los archivos .jar

3. En tu proyecto de Spring Boot, ¿de dónde sale la versión de una dependencia que no tiene `<version>`?
Salen del <dependencyManagement>

4. ¿Qué va en `settings.xml` y no en `pom.xml`? ¿Por qué?
settings.xml se usa para configuración, credencias e infraestructura (NO se sube a git) y el punto del pom es son dependencias y plugins (este se sube a git)
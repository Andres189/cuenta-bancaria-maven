# Errores de Maven que encontré

| Queja | La línea clave que dijo Maven | La causa | Cómo lo arreglé |
|---|---|---|---|
| 1 | linea 24 | tag name </dependencia> must match start tag name <dependency> | cambiando el tag de cierre de dependecia por dependency |
| 2 | (default-compile) | cambio de java 17 a java 21 | regresandolo a la version 17 |
| 3 | Could not find artifact com.fasterxml.jackson.core:jackson-databind:jar:2.22.30 in central | cambio la version de jackson | borre el cero extra que tenia la version |
| 4 | src/main/java/com/academia/banco/EstadoDeCuenta.java:[6,34] package com.fasterxml.jackson.core does not exist | Se pueso el scope de la dependecia en test | solamente borrar la linea de scope |
| 5 | Could not find or load main class com.academia.banco.Aplicacion | cambiaron donde encontrar la clase main | cambiar Aplicacion por App en <mainClass> |
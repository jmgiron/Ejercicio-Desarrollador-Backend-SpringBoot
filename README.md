
# Ejercecio Desarrollador Backend SpringBoot
Ejercicio Desarrollador Backend SpringBoot



## Descripcion.

El proyecto consiste en la creación de un servicio RESTfull para el mantenimiento de usuarios usando el Framework SpringBoot y Java 8+.

## Tecnologias usadas

- SpringBoot.
- Java 8+ (OpenJDK 17).
- Spring Security.
- Swagger.
- Base de datos H2.
- SpringBoot OAuth2 Resource server.
- Mockito.
- Maven.

# Descarga del repositorio.

Para descargar el repositorio use el comando:
```
git clone -b master https://github.com/juancgalvez/spring-usuarios-restfull.git](https://github.com/jmgiron/Ejercicio-Desarrollador-Backend-SpringBoot.git
```

## Realización de pruebas.

### Generar JAR:

```
mvn package
```

### Pruebas unitarias:

```
mvn tests
```

### Ejecutar el micro servicio:

```
mvn spring-boot:run
```

### Pruebas con POSTMAN:

Para probar con Postman importe [este archivo](https://github.com/postman_collection.json).

Al autenticar el usuario para solicitar el token, un script guarda en una variable global el JWT regresado. Esta variable se toma al momento de enviar las demás peticiones de mantenimiento del usuario, agregandolo en el encabezado Authorization como Bearer.


### Acceso a UI de SWAGGER:

Para acceder a la interfaz de usuario de SWAGGER use el URL:

[http://localhost:8089/swagger-ui/](http://localhost:8089/swagger-ui/).

Antes de invocar Endpoints debe presionar el botón ![](https://github.comoton-authorize.jpg) y autenticarse ingresando el JWT generado por Postman para el usuario **jcgalvezv@localhost.cl** y la contraseña **P@ssw0rd** (Usuario inicial en la base de datos).

### Acceso a UI de H2:

Para acceder a la interfaz de usuario de H2 use el URL:

[http://localhost:8089/h2-ui/](http://localhost:8089/h2-ui/)


## Diagramas.

### Diagrama de base de datos:


![](https://github.com/juob/master/Diagrama%20Base%20de%20Datos.jpg)


### Diagrama de secuencia para obtener token:


![](https://github.com/juen.jpeg)


### Diagrama de secuencia generalizado para dar mantenimiento a los usuarios:


![](https://github.cg)


### Diagrama UML de clases JAVA:


![](https://git)

## Notas finales:

El servicio se expone en el puerto 8089 para evitar conflictos con otros que puedan usar el 8080 por defecto.



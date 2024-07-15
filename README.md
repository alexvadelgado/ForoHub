
<p> Badge de finalizacion del challenge </p>

<h1 align="center">Tech Foro Hub</h1>
 Tech Foro Hub es una aplicación de foro backend desarrollada como proyecto desafío para el curso Oracle Next One Education. Permite a los usuarios crear publicaciones, comentar en publicaciones e interactuar entre ellos en un entorno similar a un foro.

# Tabla de Contenidos

1. Requisitos Previos
2. Instalación
3. Uso
4. Endpoints
5. Funcionalidades
6. Configuración
7. Desarrollado Con
8. Documentación
9. Licencia

## Requisitos Previos
Antes de comenzar, asegúrate de tener instalado lo siguiente:

* Java 17 JDK
* Maven
* Spring Boot
* Spring Security con JWT
* Spring JavaDoc Swagger
* Base de datos MySQL (nombre del esquema: forohub)
* Herramientas de desarrollo (se recomienda IntelliJ IDEA)
* Opcional: Insomnia u otra herramienta similar para pruebas de API
* Opcional: MySQL Workbench para gestión de bases de datos

## Instalación
Para instalar y ejecutar Tech Foro Hub:

Clona el repositorio desde GitHub:

_bash_
``` 
git clone https://github.com/your-username/tech-foro-hub.git
``` 
**Abre el proyecto en tu IDE preferido (por ejemplo, IntelliJ IDEA).**

Compila y ejecuta la aplicación desde tu IDE.

## Uso
Tech Foro Hub es una aplicación backend. Después de ejecutar la aplicación localmente, puedes acceder a la documentación de Swagger UI en http://localhost:8080/swagger-ui/index.html#/. Esta interfaz proporciona detalles sobre los endpoints de la API disponibles.

## Endpoints

### :white_check_mark: Controlador de Usuarios
:flags: GET /users: Obtiene una lista de 10 usuarios.

:scroll: PUT /users/{id}: Actualiza la información del usuario proporcionando el ID del usuario junto con el nombre o el correo electrónico actualizado.

:label: GET /users/{id}: Obtiene los detalles de un usuario por ID.

### :white_check_mark: Controlador de Temas
:flags: GET /topics: Obtiene una lista de temas.

:card_file_box: POST /topics: Crea un nuevo tema proporcionando título, mensaje, estado, ID de usuario y curso.

:label: GET /topics/{id}: Obtiene un tema por ID.

:hotsprings: DELETE /topics/{id}: Elimina un tema por ID.

### :white_check_mark: Controlador de Respuestas
:card_file_box: POST /responses: Publica una respuesta (comentario) a un tema proporcionando solución, ID de usuario y ID de tema.

:flags: GET /responses: Obtiene una lista de respuestas.

:label: GET /responses/{id}: Obtiene una respuesta por ID.

:scroll: PUT /responses/{id}: Modifica una respuesta por ID.

:hotsprings: DELETE /responses/{id}: Elimina una respuesta por ID.

### :white_check_mark: Controlador de Registro

:dependabot: POST /register: Crea un nuevo usuario para el registro.

### :white_check_mark: Controlador de Autenticación

:lock_with_ink_pen: POST /authenticate: Autentica el inicio de sesión del usuario con Spring Security y JWT.
Para acceder a la mayoría de los endpoints, necesitas autenticarte con un token Bearer obtenido del endpoint /authenticate.

## Configuración
> [!IMPORTANT]
> Asegúrate de tener MySQL instalado y crea una base de datos llamada forohub. Configura los detalles de conexión a la base de datos en application.properties o application.yml.

## Funcionalidades
> - Registro y autenticación de usuarios utilizando Spring Security y JWT.
> - Operaciones CRUD para usuarios, temas y respuestas.
> - Documentación de API con Swagger para exploración sencilla de los endpoints.
> - Desarrollado Con
> - Java 17
> - Maven
> - Spring Boot
> - Spring Security con JWT
> - Spring JavaDoc Swagger
> - MySQL con Spring Data JPA y Flyway para gestión de bases de datos
> - Insomnia u otra herramienta similar para pruebas de API
> - MySQL Workbench para visualización y gestión de bases de datos

## Documentación
> [!TIP]
> Explora la API utilizando Spring JavaDoc Swagger en http://localhost:8080/swagger-ui/index.html#/.
<p>  Swagger Map para Spring JavaDoc </p>

![Swagger forohub](https://github.com/luchiobv/Tech-ForoHub/assets/128253160/05bdfa35-2f3c-4f60-b42a-3218bf306a54)

<p> Mapa de la base de datos </p>

![dba foro hub](https://github.com/luchiobv/Tech-ForoHub/assets/128253160/7c1bb9db-2311-4d05-bc6e-adeaacdf2d20)


## Contribución
> [!CAUTION]
> ¡Las contribuciones a Tech Foro Hub son bienvenidas! Por favor, sigue nuestras Directrices de Contribución.

## Licencia
:copyright: Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.



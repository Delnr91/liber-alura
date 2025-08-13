# 📚 LiterAlura - Un Explorador Digital de Libros

¡Bienvenido a **LiterAlura**, una aplicación de consola desarrollada con Spring Boot que te permite explorar una vasta biblioteca digital! Este proyecto se conecta a la API de **Gutendex** para buscar, gestionar y consultar información detallada sobre libros y autores.

## ✨ Características Principales

* **Búsqueda de Libros**: Busca libros por título y guarda la información relevante, incluyendo el autor, idioma y número de descargas.
* **Gestión de Autores**: La aplicación maneja los datos de los autores de manera inteligente, evitando duplicados y guardando información como la fecha de nacimiento y fallecimiento.
* **Listado de Contenido**: Puedes visualizar una lista completa de libros y autores guardados en la base de datos.
* **Autores Vivos por Año**: Consulta qué autores estaban vivos en un año específico.
* **Filtrado por Idioma**: Filtra los libros registrados en la base de datos por idioma (inglés, español, francés).
* **API Gutendex**: La aplicación utiliza la API de Gutendex para obtener los datos de los libros.

## 🚀 Tecnologías y Arquitectura

Este proyecto está construido con una arquitectura sólida y modular utilizando las siguientes tecnologías:

* **Java 21**: Lenguaje de programación principal.
* **Spring Boot 3.5.3**: Framework para el desarrollo de la aplicación.
* **Spring Data JPA**: Abstracción para el acceso a la base de datos, facilitando la persistencia de datos.
* **PostgreSQL**: Base de datos relacional utilizada para almacenar los libros y autores.
* **Maven**: Herramienta de gestión y construcción del proyecto.
* **Jackson**: Librería para el procesamiento de JSON, utilizada para mapear las respuestas de la API a DTOs.
* **API Gutendex**: Servicio externo para la obtención de datos de libros.

## ⚙️ Configuración y Ejecución

Para ejecutar esta aplicación, sigue estos pasos:

1.  **Clona el repositorio** en tu máquina local.
2.  **Configura la base de datos**: Modifica el archivo `src/main/resources/application.properties` con tus credenciales de PostgreSQL.
    ```properties
    spring.datasource.url=jdbc:postgresql://${DB_HOST}/libreria
    spring.datasource.username=${DB_USER}
    spring.datasource.password=${DB_PASSWORD}
    spring.datasource.driver-class-name=org.postgresql.Driver
    spring.jpa.hibernate.ddl-auto=update
    spring.jpa.show-sql=true
    spring.jpa.format-sql = true
    ```
3.  **Ejecuta la aplicación**: Puedes usar tu IDE (como IntelliJ IDEA o Eclipse) o ejecutarla desde la terminal usando Maven.
    ```bash
    ./mvnw spring-boot:run
    ```

## 📧 Contacto

* **Nombre:** Daniel Núñez Rojas
* **GitHub:** [@Delnr91](https://github.com/Delnr91)
* **LinkedIn:** [Daniel Núñez Rojas](https://www.linkedin.com/in/delnr91)
* **Correo:** [danidev33@gmail.com](mailto:danidev33@gmail.com)

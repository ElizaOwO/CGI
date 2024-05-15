# Resumen Ejecutivo

**Descripción:** El Colegio Gastronómico Internacional (CGI) busca mejorar su sistema de gestión de información mediante una aplicación integrada y segura.

**Problema Identificado:** Uso de hojas de Excel para registro de asistencia y calificaciones, falta de eficiencia y seguridad.

**Solución:** Desarrollo de una aplicación de gestión de alumnos, maestros, calificaciones y materias, integrada a una base de datos, con funcionalidades específicas para profesores, alumnos y directivos.

**Arquitectura:** Uso de JavaScript y React para el front-end, SQL para la base de datos, separación entre front-end y back-end.

# Requisitos:
Última versión de lo siguiente:

- **NodeJS**
- **Android Studio**
- **Visual Studio Code**
- **Postgres** instalado y algún manager.
- **Postman**

# Configuración:

1. Abrir en el buscador de Windows SQL Shell (postgres).
2. Presionar Enter hasta que pida la contraseña (no la de la base de datos).
3. Cuando aparezca en la terminal "postgres=#", escribir `create database mycgi;` (con el punto y coma).
4. Abrir DBeaver y en la izquierda hacer clic derecho y seleccionar "Crear nueva conexión".
5. Dejar todo por defecto excepto la contraseña que se ha creado.
6. En el proyecto (el código), cambiar el archivo `database.json` y agregar su contraseña.
7. En el archivo `src/database/db_connect.js`, en la línea 13, cambiar las comillas dobles (`""`) por su contraseña.
8. Ejecutar los siguientes comandos:
    ```bash
    npm i
    npm i -g db-migrate
    db-migrate up
    npm run dev 
    ```
   (En este último tiene que aparecer el mensaje "Server on port: 3002").
9. En Postman, establecer la URL como `http://localhost:3002/api/Login` y asegurarse de que el método sea (GET).
10. En Postman, en la sección de Autorización, agregar una clave "Authorization" (sin comillas) y como valor poner `"Basic YWRtaW46YWRtaW4="` (sin comillas).
11. Hacer clic en "Enviar" o "Send".

# Tabla de Contenido

- NodeJS [Descargar](https://nodejs.org/en/download)
- XCode o Android Studio
- Visual Studio Code [Descargar](https://code.visualstudio.com/download)
- Postgres [Descargar](https://www.postgresql.org/download/)
- DBeaver [Descargar](https://dbeaver.io/)
- Postman [Descargar](https://www.postman.com/downloads/)

🛠️ **Sistema de Gestión de Proyectos y Clientes**
Este proyecto es una API RESTful desarrollada con Spring Boot que permite la gestión integral de 👤 usuarios, 📁 categorías, 🧑‍💼 clientes y 📊 proyectos, con un enfoque en la seguridad, control de acceso por roles y cumplimiento de buenas prácticas de desarrollo.


📋 **Descripción General**
El sistema está diseñado para facilitar el control y seguimiento de proyectos vinculados a clientes, permitiendo gestionar entidades clave como usuarios, categorías, clientes y proyectos. Además, incorpora políticas de seguridad robustas como autenticación con 🔐 JWT, cifrado de contraseñas y bloqueo por intentos fallidos.


🧩 **Módulos Principales**

👤 Gestión de Usuarios:
* ✅ Registro, edición y habilitación/deshabilitación de usuarios.
* 🔐 Inicio y cierre de sesión.
* 🧾 Visualización y edición del perfil personal.
* 🔄 Cambio y recuperación de contraseña.
* 🛡️ Control de acceso por roles (`ADMIN`, `USUARIO_LIMITADO`).

📁 Gestión de Categorías de Proyectos:
* ➕ Crear, listar y actualizar categorías.
* 🔍 Consultar categorías activas.
* 🔄 Habilitar/deshabilitar categorías.

🧑‍💼 Gestión de Clientes:
* ➕ Registro, listado y actualización de clientes.
* 🔍 Consultar clientes activos.
* 🔄 Control de estado (habilitado/deshabilitado).

📊 Gestión de Proyectos:
* ➕ Crear proyectos vinculados a clientes y categorías.
* 📋 Listar y actualizar proyectos.
* 🔍 Consultar proyectos activos.
* 🔄 Control de estado de los proyectos.

🔐 **Seguridad y Autenticación**
* 🔑 Autenticación con JWT (JSON Web Tokens).
* 🛡️ Control de acceso basado en roles:
  * 👑 ADMIN: Acceso completo.
  * 👤 USUARIO\_LIMITADO: Solo lectura de proyectos asignados.
* 🔒 Cifrado de contraseñas con BCrypt.
* 🚫 Bloqueo automático tras 3 intentos fallidos de login (bloqueo por 30 minutos).
* 📧 Recuperación de contraseña vía correo electrónico.

🛠️ **Tecnologías Utilizadas*
* ☕ Spring Boot 3
* 🔐 Spring Security + JWT
* 💾 Spring Data JPA
* 🐬 MySQL
* 🧬 MapStruct
* 🧩 Lombok
* 🧪 Postman (para pruebas)

📁 **Estructura del Proyecto**
src
├── controller
├── dto
├── entity
├── repository
├── service
├── security
└── config
application.properties
README.md


🚀 **Requisitos de Ejecución**
* ⚙️ Java 17 o superior
* 📦 Maven 3.8 o superior
* 🐬 MySQL 8 o superior
* 💻 IDE como IntelliJ IDEA o Spring Tools Suite

🧪 **Pruebas y Postman**
Se incluye una colección de pruebas con Postman para validar:
* ✅ Registro e inicio de sesión
* 🔐 Protección de rutas por rol
* 🔄 CRUD completo para cada entidad

📌 **Estado del Proyecto**
En desarrollo.
Actualmente se están construyendo los módulos de seguridad, gestión de usuarios y funcionalidades CRUD para categorías, clientes y proyectos.

🤝 **Contribuciones**
Si deseas colaborar con mejoras, sugerencias o correcciones, no dudes en hacer un fork y enviar un pull request. ¡Todo aporte es bienvenido!

📄 **Licencia**
Este proyecto está bajo la licencia MIT. Consulta el archivo LICENSE para más detalles.


✉️ **Contacto**
Desarrollado por: **Guero**
Carrera: Ingeniería en Tecnologías de la Información
Correo: alex@gmail.com

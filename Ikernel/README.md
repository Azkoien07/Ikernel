# IKernell Soluciones Software - Sistema de Gestión Empresarial

## Descripción del Proyecto

IKernell Soluciones Software requiere un sistema para automatizar y gestionar sus procesos internos, así como proporcionar información sobre sus servicios a través de Internet. Este software está diseñado para gestionar diferentes tipos de usuarios y optimizar la administración de proyectos dentro de la empresa.

## Tecnologías Utilizadas
- **Backend**: Spring Boot (Java 17)
- **Frontend**: Thymeleaf
- **Base de Datos**: PostgreSQL
- **Gestión de dependencias**: Gradle
- **Seguridad**: Spring Security
- **ORM**: Hibernate (JPA)
- **Otros**: Lombok

## Funcionalidades Principales

### Acceso y Roles de Usuario
- **Interesados**: Acceden de manera anónima y pueden ver información empresarial como:
  - Lineamientos de la empresa
  - Portafolio de servicios
  - Noticias relacionadas con software
  - Preguntas frecuentes
  - Información de contacto
- **Trabajadores**: Tienen credenciales y acceso a funcionalidades avanzadas como:
  - Correo corporativo
  - Chat empresarial
  - Biblioteca de software
  - Tutoriales de programación

### Gestión de Usuarios y Roles
- **Coordinador de Proyectos**:
  - Registrar perfiles de desarrolladores con información detallada.
  - Asignar proyectos a los desarrolladores.
  - Modificar información del desarrollador.
  - Generar reportes de desempeño.
  - Inhabilitar desarrolladores cuando dejen de trabajar con la empresa.

- **Líder de Proyectos**:
  - Registrar y gestionar proyectos.
  - Asignar desarrolladores a proyectos.
  - Gestionar las etapas de un proyecto.
  - Buscar, modificar o inhabilitar proyectos.
  - Generar reportes de interrupciones y actividades de un proyecto.
  - Registrar y modificar actividades de los desarrolladores.

- **Desarrolladores**:
  - Ejecutar actividades asignadas en los proyectos.
  - Registrar errores encontrados en el desarrollo.
  - Registrar interrupciones en el desarrollo de proyectos.
  - En caso de necesidad, un líder puede ser desarrollador en otro proyecto.

### Reportes y Exportaciones
- Los líderes de proyectos pueden generar reportes en formato plano para compartir con empresas aliadas.
- Reportes de desempeño y actividad de desarrolladores.
- Reportes de interrupciones y errores en proyectos.

## Instalación y Configuración
1. **Clonar el repositorio**:
   ```sh
   git clone https://github.com/tuusuario/tu-repositorio.git
   cd tu-repositorio
   ```

2. **Configurar la base de datos PostgreSQL**:
   - Crear una base de datos en PostgreSQL.
   - Configurar las credenciales en `application.properties` o `application.yml`:
     ```properties
     spring.datasource.url=jdbc:postgresql://localhost:5432/nombre_base_datos
     spring.datasource.username=tu_usuario
     spring.datasource.password=tu_contraseña
     spring.jpa.hibernate.ddl-auto=update
     ```

3. **Ejecutar el proyecto**:
   ```sh
   mvn spring-boot:run
   ```
   o si usas Gradle:
   ```sh
   ./gradlew bootRun
   ```

4. **Acceder a la aplicación**:
   - Interfaz web: `http://localhost:8080`

## Contribuciones
Si deseas contribuir a este proyecto, puedes hacer un fork del repositorio, crear una rama con tus cambios y enviar un pull request.

## Licencia
Este proyecto está bajo la licencia MIT. Ver el archivo `LICENSE` para más detalles.
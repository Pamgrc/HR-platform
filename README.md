# HR-platform
plataforma básica para coordinación de recursos humanos

## Descripción

Este proyecto es un sistema web para la gestión interna de recursos humanos. Permite a los empleados gestionar sus solicitudes de vacaciones, ver información general del personal, actualizable en línea, y acceder a información profesional y académica. Además, proporciona a los administradores un panel para aprobar/rechazar solicitudes de vacaciones y gestionar anuncios generales.

### Páginas incluidas:
- **Escritorio:** Información de cumpleaños, personas en home office, anuncios.
- **Personal:** Información de empleados (actualizable en línea).
- **Profesional:** Información profesional y académica de cada empleado.
- **Vacaciones:** Solicitudes de vacaciones de los empleados.
- **Autorizaciones:** Panel para aprobar/rechazar solicitudes de vacaciones.

## Tecnologías Utilizadas

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** PHP, MySQL
- **Framework:** WordPress
- **Servidor:** Apache (o compatible)
- **Gestión de dependencias:** Composer (opcional)
  
## Instalación

1. Clona este repositorio en tu máquina local:

    ```bash
    git clone https://github.com/tu-usuario/proyecto-web.git
    ```

2. Configura el entorno local de desarrollo (asegúrate de tener XAMPP, MAMP o un servidor web similar con PHP y MySQL).
3. Importa el archivo `schema.sql` en tu base de datos MySQL.
4. Configura los detalles de la base de datos en `wp-config.php`.

    ```php
    define('DB_NAME', 'nombre_de_tu_base_de_datos');
    define('DB_USER', 'tu_usuario');
    define('DB_PASSWORD', 'tu_contraseña');
    define('DB_HOST', 'localhost');
    ```

5. Sube el proyecto a tu servidor web y asegúrate de que las carpetas estén correctamente organizadas.
6. Asegúrate de que los enlaces permanentes de WordPress estén configurados para que las páginas funcionen correctamente.

## Estructura de Archivos

El proyecto está organizado en las siguientes carpetas:

- `assets/`: Contiene los archivos CSS, JavaScript y recursos de imagen.
- `templates/`: Plantillas PHP para la cabecera, pie de página y otras partes comunes.
- `inc/`: Archivos PHP donde reside la lógica para gestionar solicitudes, empleados y anuncios.
- `pages/`: Páginas principales del sitio web como "Escritorio", "Vacaciones", "Autorizaciones", etc.
- `database/`: Archivo de esquema de base de datos.
- `docs/`: Documentación técnica adicional.

## Funcionalidades Principales

1. **Escritorio:**
   - Muestra información de cumpleaños, anuncios generales y empleados en home office.
   
2. **Personal:**
   - Página para visualizar y editar la información personal de los empleados.

3. **Profesional:**
   - Página para administrar la información profesional y académica de los empleados.

4. **Vacaciones:**
   - Módulo para que los empleados soliciten vacaciones.

5. **Autorizaciones:**
   - Panel para que los managers autoricen o rechacen las solicitudes de vacaciones.

## Base de Datos

El esquema de base de datos se encuentra en el archivo `database/schema.sql`. Las principales tablas son:

- `vacaciones_solicitudes`: Registra las solicitudes de vacaciones.
- `principal`: Almacena la información personal de los empleados y por ende los cumpleaños.
- `anuncios`: Contiene los anuncios generales y cumpleaños.
- `vacaciones`: Contiene información acerca de los periodos de vacaciones y los gerentes responsables.
- `pro`: Contiene información profesional es bastante útil para prever las suplencias. 
- `ho`: muestra la información relacionada a el/los días de home office de cada empleado. 

## Contribuciones

¡Las contribuciones son bienvenidas! Si deseas contribuir al proyecto, por favor sigue estos pasos:

1. Haz un fork del proyecto.
2. Crea una nueva rama para tu funcionalidad (`git checkout -b nueva-funcionalidad`).
3. Realiza tus cambios y confirma tus commits (`git commit -m 'Agrega nueva funcionalidad'`).
4. Haz push a la rama (`git push origin nueva-funcionalidad`).
5. Abre un Pull Request.

## Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE.md](LICENSE.md) para más detalles.

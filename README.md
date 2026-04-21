## Licencia

Este proyecto está distribuido bajo la **Licencia MIT**. Esto significa que es una licencia permisiva y libre. Puedes clonar, modificar y usar este código estructural e interfaz para tus propios proyectos con una única condición estricta: debes incluir la atribución al autor original **alzari555** dejando intacto el archivo LICENSE y respetando los derechos de autor allí descritos.

## Estructura de la Web

La organización de archivos se compone de lo siguiente:

* **index.html**: Página principal que actúa como carta de presentación mostrando el manifiesto de diseño, los servicios ofrecidos y los canales de contacto.
* **portafolio.html**: Espacio dedicado a exponer los diversos proyectos completados con un diseño reticular.
* **style.css**: Hoja de estilos en cascada que alberga la identidad visual completa, incorporando la paleta monocromática terrosa, variables de tipografía y pautas de diseño adaptativo.
* **assets/**: Carpeta centralizada para recursos visuales, logotipos, fondos y material fotográfico del portfolio.
* **admin/** y **data/**: Carpetas de utilidad y almacenamiento de datos JSON.
* **email-contacto.html** y **email-newsletter.html**: Plantillas adaptables de correo electrónico construidas con el sistema de diseño Emebe para comunicaciones consistentes.

## Despliegue y Uso en GitHub Pages

El proyecto viene preparado con un sistema de trabajo preconfigurado para ser alojado rápida y gratuitamente en los servidores de GitHub de la siguiente manera:

### 1. Publicar el Sitio
Una vez que el proyecto resida en tu propia cuenta de GitHub, dirígete a la pestaña superior llamada **Settings**. En la barra lateral izquierda ingresa a la sección **Pages**.
Bajo el subtítulo **Build and deployment**, debes localizar la opción **Source** y seleccionar la configuración **GitHub Actions**.

### 2. Publicación y Optimización Automática
Un script dentro del repositorio interceptará todos los cambios que envíes a la rama principal. Si tu actualización contempla imágenes subidas a la carpeta de recursos, el servidor automático las comprimirá y convertirá a un formato ligero y veloz, garantizando un peso menor a 200KB sin pérdida perceptible de nitidez. Acto seguido, la nueva versión optimizada será desplegada a la vez.

### 3. Enlaces Internos
Al ser un sistema web basado enteramente en referencias relativas de HTML puro, no resulta imperativo modificar variables de ruteo complejas al mover de un servidor a otro. Los saltos entre diferentes secciones o archivos funcionarán correctamente sobre tu nuevo enlace de GitHub Pages.

## Configuración del Administrador de Contenido Sveltia

El sitio incluye un panel de administración llamado Sveltia CMS ubicado en la carpeta `admin/`. A través de este panel es posible gestionar los contenidos fotográficos y descripciones de los proyectos en tu portafolio. Para que el administrador logre conectar y funcionar correctamente en tu nuevo repositorio forkeado debes actualizar su archivo de configuración:

1. Abre el archivo `admin/config.yml`.
2. Modifica el campo `repo: alzari555/emebe-pagina` y reemplázalo por tu propio usuario y nombre de repositorio siguiendo el formato `tu-usuario/nombre-del-repo`.
3. Adicionalmente es recomendable modificar el campo `site_domain` con tu nuevo dominio temporal o final `tu-usuario.github.io` o tu propia pagina web.

Una vez realizados estos pequeños ajustes y subidos al repositorio principal podrás ingresar a la gestión de contenido añadiendo la terminación `/admin` al final de la dirección principal de tu página web.

Disfruta del ecosistema de la web y mucho éxito gestionando futuros proyectos en tu página.

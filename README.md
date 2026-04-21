# Proyecto Emebe

Este es el repositorio base de la página estática del proyecto Emebe ("emebe-pagina"). Este sitio está construido utilizando HTML, CSS, y JavaScript puro de forma estática para mantenerlo simple y altamente performante.

## Licencia

Este proyecto está distribuido bajo la **Licencia MIT**. Esto significa que es una licencia permisiva y libre, puedes clonarla, modificarla y usarla para tus propios proyectos con una única condición: **debes incluir la atribución al autor original (Emebe/Migue)** dejando intacto el archivo `LICENSE` y los derechos de autor que vienen en él.

## Despliegue y Uso 

### 1. Hacer un Fork
Haz clic en el botón superior derecho de esta página de GitHub que dice **"Fork"** (o "Bifurcar"). Esto copiará todo este repositorio a tu propia cuenta de GitHub de forma segura.

### 2. Configurar GitHub Pages
Una vez que el proyecto esté en tu propia cuenta de GitHub, para visualizar el sitio en la dirección `https://<tu-usuario>.github.io/<nombre-del-repo>` (por ejemplo, hasta que consigas un dominio personalizado):

1. Ve a la pestaña **Settings** (Configuración) dentro de tu repositorio forkeado.
2. En la barra lateral izquierda, selecciona **Pages** (Páginas).
3. En la sección **Build and deployment** (Construcción y despliegue), en la opción **Source** (Origen), selecciona **"GitHub Actions"**.
4. ¡Y listo! El proyecto ya tiene configurado un flujo de trabajo (`deploy-and-optimize.yml`) que publicará tu página automáticamente cada vez que hagas un cambio (como editar un archivo y hacer un *Commit* a la rama `main`).

*(Nota: La primera vez podría tardar un par de minutos en publicar tu sitio. Puedes revisar el progreso en la pestaña **Actions**).*

### 3. Actualización de Enlaces ("Configuración de Subida/Sitio")

Dado que el entorno de desarrollo es HTML puro (no utiliza frameworks como Svelte o React que requieran configurar un `base path`), todos los enlaces internos (`href="portafolio.html"`, etc.) funcionan de manera relativa automáticamente y se adaptarán sin problema al estar bajo tu propio nombre de usuario de GitHub Pages.

Si por algún motivo necesitas enlazar contenido con rutas absolutas, solo asegúrate de actualizar el dominio de `https://...` a tu nuevo `https://<tu-usuario>.github.io/<nombre-del-repo>/` en tus archivos HTML.

### Flujo de optimización automático
Este proyecto cuenta con un bot integrado en GitHub Actions que cada vez que subes una imagen en formato `.jpg` o `.png` a la carpeta `assets/uploads`, él mágicamente y de forma transparente las convertirá a un formato ultra-ligero (`.webp` menores de 200KB) para que tu web cargue a la velocidad de la luz, manteniéndolas en la máxima calidad.

---

**¡Disfruta modificando y lanzando tu página!**

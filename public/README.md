# Carpeta Public en React

Este documento ofrece una descripción detallada de la carpeta `public` en un proyecto React y su uso típico.

## Descripción General

La carpeta `public` contiene los archivos estáticos que se pueden servir sin necesidad de ser procesados por Webpack. Esto incluye el archivo HTML principal (usualmente `index.html`), imágenes, y cualquier otro activo que requiera ser accesible sin importar la ruta de la URL.

## Contenidos de la Carpeta `public`

Aquí hay una descripción de los archivos y directorios comunes que podrías encontrar en la carpeta `public` de un proyecto React:

- `index.html`: Es el archivo HTML base para tu aplicación React. Este es el archivo que se sirve cuando los usuarios acceden a tu aplicación. Contiene un div raíz (`<div id="root"></div>`) donde tu aplicación React será renderizada.
- `favicon.ico`: El favicon de la aplicación que se muestra en la pestaña del navegador.
- `manifest.json`: Es un archivo de manifiesto web que controla cómo tu aplicación aparece y cómo se lanza. Define la apariencia de la aplicación, los iconos en la pantalla de inicio del dispositivo móvil y el arranque inicial de la pantalla completa.
- `robots.txt`: Un archivo de texto que le indica a los motores de búsqueda cuáles partes de tu sitio web deberían y no deberían ser indexadas.
- `logo192.png` y `logo512.png`: Son imágenes de logo que se utilizan en el manifiesto para los íconos en la pantalla de inicio.

## Modificar `index.html`

Puedes personalizar `index.html` para incluir metadatos específicos como títulos de página, descripciones, y metadatos de redes sociales (Open Graph, Twitter Cards). Sin embargo, para títulos de página dinámicos o enlaces de meta específicos de páginas, es posible que necesites una solución de renderizado del lado del servidor o utilizar librerías como React Helmet.

## Añadir Activos Estáticos

Si necesitas incluir imágenes, archivos, o cualquier otro activo estático que no requiere ser procesado por Webpack, colócalos en la carpeta `public` y referéncialos con un enlace absoluto desde el archivo `index.html` o desde tu código React usando `%PUBLIC_URL%` como prefijo. Por ejemplo:

<link rel="icon" href="%PUBLIC_URL%/favicon.ico" />

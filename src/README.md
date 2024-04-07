# Carpeta SRC

Este documento describe la estructura y el contenido de la carpeta `src` en este proyecto de React.

## Estructura de la Carpeta

La carpeta `src` contiene todos los archivos de código fuente para la aplicación React, organizados de la siguiente manera:

- `index.js`: El punto de entrada para la aplicación React. Este archivo renderiza el componente `App` en el DOM.
- `App.js`: El componente raíz de la aplicación React, que contiene la estructura de la página y agrupa otros componentes.
- `components/`: Un directorio para todos los componentes de React reutilizables. Cada componente está en su propia carpeta con su respectivo código y hoja de estilos.
- `assets/`: Carpeta para imágenes, íconos y otros activos estáticos utilizados en la aplicación.
- `styles/`: Contiene archivos de hojas de estilo globales que se pueden utilizar en toda la aplicación.
- `utils/`: Funciones de utilidad que pueden ser importadas y utilizadas en varios componentes.
- `tests/`: Pruebas para los componentes de la aplicación, utilizando Jest y React Testing Library.

## Componentes

Cada componente en `components/` sigue la siguiente estructura:

- `ComponentName.js`: El archivo JavaScript que define el componente de React.
- `ComponentName.module.css`: Una hoja de estilo CSS modular para estilos específicos del componente.

## Estilos

Los estilos globales se encuentran en la carpeta `styles/` y pueden incluir archivos como:

- `main.css`: Estilos generales que afectan a toda la aplicación.
- `variables.css`: Definiciones de variables CSS como colores, fuentes, etc., para mantener la consistencia del diseño.

## Importante

Por favor, no coloques ningún código fuera de esta carpeta que se espera que sea parte del build final, ya que Webpack solo procesará los archivos dentro de `src`.

Si modificas esta estructura, asegúrate de actualizar este documento para reflejar los cambios para futuros colaboradores.
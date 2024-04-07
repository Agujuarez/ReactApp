# Instalación de React

Este `README` describe cómo instalar React para empezar a construir una aplicación.

## Pre-requisitos

Debes tener Node.js y npm instalados en tu máquina. Visita [https://nodejs.org/](https://nodejs.org/) para descargar e instalar Node.js, que incluye npm.

## Paso 1: Crear una Nueva Carpeta para el Proyecto

Abre tu terminal y ejecuta los siguientes comandos para crear una nueva carpeta para tu proyecto y navegar dentro de ella:

mkdir mi-app-react
cd mi-app-react

## Paso 2: Inicializar un Nuevo Proyecto de Node.js
Inicializa un nuevo proyecto Node.js. Esto creará un archivo package.json en tu directorio del proyecto:

~~~
npm init -y
~~~

Paso 3: Instalar React y React DOM
Instala React y ReactDOM con npm. Estos comandos agregarán React y ReactDOM a la lista de dependencias en tu package.json y los instalarán en la carpeta node_modules:

~~~
npm install react react-dom
~~~

Comenzando con React
Con React y ReactDOM instalados, ya puedes comenzar a escribir tu aplicación React. Crea un archivo HTML y un archivo JavaScript:

* index.html: Un archivo HTML que será la página principal de tu aplicación.
* index.js: Un archivo JavaScript donde escribirás tu componente React principal.

### index.html
Crea un archivo index.html en la raíz del proyecto con el siguiente contenido:

~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi App React</title>
</head>
<body>
    <div id="app"></div>
    <script src="index.js"></script>
</body>
</html>
~~~

### index.js
Crea un archivo index.js en la raíz del proyecto con el siguiente contenido para renderizar un componente React básico en la página:

### javascript
~~~
import React from 'react';
import ReactDOM from 'react-dom';

const App = () => {
  return <h1>Hola, mundo!</h1>;
};

ReactDOM.render(<App />, document.getElementById('app'));
~~~

## Paso 4: Ejecutar la Aplicación
Para ver tu aplicación, abre el archivo index.html en tu navegador.
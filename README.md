# Workshop: Portfolio Personal

Este es el repositorio del WorkShop **Portfolio Personal** creado por **Juan Bilardi** 

Conocé más sobre el profe [acá](https://threehdm.github.io/personal_page/#developer)

# ¿Qué tecnologías vamos a usar?

 - NPM (Node Package Manager)
  - [browser-sync](https://www.browsersync.io/)
- [Bootstrap 4](https://getbootstrap.com/docs/4.4/getting-started/introduction/)


Comencemos!

# Creando el ambiente de desarrollo

# Creando nuestro repositorio en GITHUB

-Agregar el README.md

## Instalando Browser-Sync
https://stackedit.io/app
https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

Browser-sync nos permite ver los cambios de código en vivo y nos ahorra tener que refrescar el navegador cada vez que actualicemos nuestro código.

Para instalarlo de forma global en nuestra computadora, debemos correr el siguiente script en la TERMINAL:

```
npm install -g browser-sync
```

Luego debemos correr el siguiente comando, el cual indica a browser-sync qué archivo controlar como así también crea un pequeño servidor para que aloje nuestro proyecto. En este caso le diremos que controle todos nuestros archivos

```
browser-sync start --server --files "*.*"
```

Browser-sync levantará un servidor local y uno externo para que veamos en tiempo real los cambios que guardemos (CTRL+S) en nuestros archivos estáticos.

_Nota: de obtener un error al correr el último script desinstalar y reinstalar node.js de nuestra PC.active_

## Creando nuestra estructura de proyecto

Siempre que comenzamos un nuevo proyecto debemos planear cómo lo vamos a estructurar. Para este workshop utilizremos una estructura básica:

```
Project/
├── css/
│    └── styles.css
├── js/
│   └── main.js
└── img/
│ 
└── index.html
│ 
└── README.md
```

## Estructura del HTML

En nuestro index.html armamos una estructura básica de HTML para comenzar a trabajar

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

## Integrando BOOTSTRAP 4

Bootstrap es un conjunto de herramientas y componentes que nos permiten crear rápidamente aplicaciones responsivas y que respeten la consigna mobile-first.

Una de las formas rápidas de integrarlo a nuestro proyecto es utilizando el  BootstrapCDN. Para ello debemos copiar el siguiente código en nuestro index.html justo antes de la etiqueta `</head>`

```
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
```

Éste código trae a nuestro proyecto los estilos de BOOTSTRAP. Pero también queremos traer la funcionalidad, por lo que para que BOOTSTRAP pueda crear contenido dinámico, agregamos el siguiente código antes de la etiqute `</body>`

```
<script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
```

Toda esta información y más se encuentra en la [documentación oficial](https://getbootstrap.com/docs/4.4/getting-started/introduction/)

## La magia de Bootstrap: el Grid System







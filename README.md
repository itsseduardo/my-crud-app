## Mi Aplicación CRUD con Docker y MongoDB ##

Esta es una aplicación CRUD básica construida con Node.js, Express, MongoDB, Docker y una interfaz de usuario simple con HTML, CSS y Bootstrap.

Requisitos previos
   
Docker instalado en tu sistema: [Instalacion Docker](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04-es)

Docker Compose (solo si no se incluye con Docker en tu sistema):[ Instalacion Docker Compose](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-compose-on-ubuntu-20-04-es)

    
Configuración del proyecto

    Clona este repositorio en tu máquina local:

    bash

git clone https://github.com/itsseduardo/my-crud-app.git

Accede al directorio del proyecto:

bash

    cd mi-aplicacion-crud

Uso
Construir y levantar los contenedores Docker

    Abre una terminal y navega hasta el directorio del proyecto.

    Ejecuta el siguiente comando para construir y levantar los contenedores Docker:

    bash

    docker-compose up --build

Acceder a la aplicación

Una vez que los contenedores estén en funcionamiento, puedes acceder a la aplicación en tu navegador web:

    http://localhost:3000

La aplicación debería mostrarte una interfaz donde puedes agregar y eliminar items.
Detener los contenedores

Para detener los contenedores Docker, simplemente presiona Ctrl + C en la terminal donde se están ejecutando los contenedores.
Estructura del proyecto

El proyecto está estructurado de la siguiente manera:

php

mi-aplicacion-crud/
│
├── src/
│   ├── index.js        # Archivo principal del servidor
│   ├── routes/         # Rutas de la API
│   │   └── items.js
│   └── models/         # Modelos de datos de MongoDB
│       └── item.js
│
├── public/             # Archivos estáticos del frontend
│   └── index.html
│
├── docker-compose.yml  # Archivo de configuración de Docker Compose
├── Dockerfile          # Archivo de configuración de Docker
└── package.json        # Archivo de dependencias del proyecto

Contribuir

Si deseas contribuir a este proyecto, sigue estos pasos:

    Haz un fork del proyecto.
    Crea una rama con tus cambios: git checkout -b feature/nueva-funcionalidad.
    Haz tus cambios y realiza commit: git commit -m 'Añadir nueva funcionalidad'.
    Empuja tus cambios a la rama: git push origin feature/nueva-funcionalidad.
    Abre un pull request en GitHub.

# Marco Teórico

Este repositorio contiene información sobre varias tecnologías fundamentales para el desarrollo web moderno. A continuación, se presenta una breve descripción de cada una de ellas, junto con sus características y ventajas.

## Node.js
![Node.js Logo](https://nodejs.org/static/images/logo.svg)

*¿Qué es Node?*  
Node.js es un entorno de ejecución para JavaScript construido con el motor de JavaScript V8 de Chrome. Permite ejecutar código JavaScript del lado del servidor.

*Características:*
- *Asincrónico y basado en eventos:* Utiliza un modelo de E/S no bloqueante, lo que lo hace ligero y eficiente.
- *Sistema de paquetes NPM:* Tiene un extenso ecosistema de bibliotecas y paquetes a través del gestor de paquetes npm.

*Ventajas:*
- *Alta escalabilidad:* Ideal para aplicaciones que requieren manejar muchas conexiones simultáneas.
- *Desempeño:* Su modelo asincrónico y el uso de V8 lo hacen muy rápido.

## Express.js
![Express.js Logo](https://expressjs.com/images/express-facebook-share.png)

*¿Qué es Express?*  
Express.js es un framework web minimalista para Node.js que proporciona un robusto conjunto de características para aplicaciones web y móviles.

*Características:*
- *Middleware:* Manejo de peticiones y respuestas a través de funciones middleware.
- *Enrutamiento:* Define rutas de aplicación con métodos HTTP y URL.

*Ventajas:*
- *Simplicidad:* Fácil de configurar y usar para crear aplicaciones web rápidas.
- *Flexibilidad:* Amplia capacidad para personalizar el comportamiento de las aplicaciones.

## MongoDB
![MongoDB Logo](https://webassets.mongodb.com/_com_assets/cms/mongodb-logo-rgb-j6w271g1xn.jpg)

*¿Qué es Mongo?*  
MongoDB es una base de datos NoSQL orientada a documentos que utiliza documentos similares a JSON con esquemas dinámicos.

*Características:*
- *Documentos BSON:* Usa un formato binario similar a JSON.
- *Escalabilidad horizontal:* Diseñada para escalar grandes volúmenes de datos y alta disponibilidad.

*Ventajas:*
- *Flexibilidad:* Los esquemas dinámicos permiten una fácil evolución de la base de datos.
- *Desempeño:* Optimizada para operaciones de lectura/escritura de alto rendimiento.

## Docker
![Docker Logo](https://www.docker.com/wp-content/uploads/2023/08/logo-dont-stretch.svg)

*¿Qué es Docker?*  
Docker es una plataforma que permite a los desarrolladores empaquetar aplicaciones y sus dependencias en contenedores, lo que asegura que se ejecuten de manera uniforme en cualquier entorno.

*Características:*
- *Aislamiento:* Contenedores aislados que contienen todo lo necesario para ejecutar una aplicación.
- *Portabilidad:* Los contenedores pueden ser ejecutados en cualquier sistema que tenga Docker instalado.

*Ventajas:*
- *Consistencia:* Garantiza que la aplicación se ejecute de la misma manera en diferentes entornos.
- *Eficiencia:* Menos sobrecarga en comparación con máquinas virtuales tradicionales.

## HTML/CSS/JavaScript
![HTML, CSS, JavaScript Logo](https://w7.pngwing.com/pngs/585/981/png-transparent-html-js-and-css-logo-cascading-style-sheets-javascript-html-css3-jquery-logo-miscellaneous-text-trademark.png)

*¿Qué es HTML, CSS y JS?*  
HTML, CSS y JavaScript son las tecnologías básicas para la creación de páginas web.

*Características:*
- *HTML:* Lenguaje de marcado para estructurar contenido web.
- *CSS:* Lenguaje de hojas de estilo para diseñar y presentar el contenido HTML.
- *JavaScript:* Lenguaje de programación para crear interactividad en páginas web.

*Ventajas:*
- *HTML:* Estructura clara y semántica del contenido.
- *CSS:* Control preciso sobre la presentación visual.
- *JavaScript:* Capacidad de crear experiencias de usuario dinámicas e interactivas.

## Bootstrap
![Bootstrap Logo](https://getbootstrap.com/docs/5.1/assets/brand/bootstrap-logo-shadow.png)

*¿Qué es Bootstrap?*  
Bootstrap es un framework de diseño web de código abierto que facilita la creación de interfaces de usuario responsive y modernas.

*Características:*
- *Componentes predefinidos:* Botones, formularios, tarjetas, etc.
- *Sistema de rejilla:* Layout responsive basado en una cuadrícula de 12 columnas.

*Ventajas:*
- *Rapidez:* Acelera el desarrollo frontend con componentes listos para usar.
- *Consistencia:* Proporciona un diseño uniforme y atractivo.

# Créditos

Este proyecto fue creado por:

- [Jesus Eduardo Aguilar Sarria](https://github.com/itsseduardo)
- [Santiago Beltran Botero](https://github.com/Santibeltranb)
- [Juan Pablo Ceballos Ramirez](https://github.com/JuanCeballos2)

# Licencia

Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo [LICENSE](https://github.com/itsseduardo/my-crud-app/blob/main/LICENSE) para más detalles.

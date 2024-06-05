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

Créditos

Este proyecto fue creado por 
[Jesus Eduardo Aguilar Sarria](https://github.com/itsseduardo)
[Santiago Beltran Botero](https://github.com/Santibeltranb)
[Juan Pablo Ceballos Ramirez](https://github.com/JuanCeballos2)

Licencia

Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.

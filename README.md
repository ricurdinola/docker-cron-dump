<div id="top"></div>
<div align="right">

[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

</div>

<br/>
<div align="center">
  <a href="https://github.com/ricurdinola/docker-alpine-cron">
    <img src="readme/cron.png" alt="Logo" width="500" height="250">
  </a>

<h3 align="center">Docker Alpine Cron</h3>

  <p align="center">
    Alpine Cron Container .
    <br />
    <a href="https://github.com/ricurdinola/docker-alpine-cron"><strong>Explorar el repo »</strong></a>
    <br />
    <br />
    <a href="https://github.com/ricurdinola/docker-alpine-cron/issues">Reportar un Bug </a>
    ·
    <a href="https://github.com/ricurdinola/docker-alpine-cron/issues">Sugerencias </a>
  </p>
</div>

## Sobre el Proyecto
El es un ejemplo de crons sobre Alpine corriendo dentro de un contenedor para Docker.
<p align="right"><a href="#top">Ir al Inicio</a></p>

### Descripción del Proyecto
<div align="center">
    <img src="readme/alpine.png" alt="Logo" width="200" height="200">
</div>

El stack se compone de los siguientes elementos:

* Un contenedor basado en Alpine Linux destinado a correr Crons.
* En el Dockerfile se encuentra comentado la configuración de la zona horaria del contenedor.
* Como ejemplo, se encuentra un cron que se ejecuta cada minuto y muestra la hora en la que se ejecuta. El archivo \cron-server\crons\root posee los comandos a ejecutar. El mismo se copia al contenedor durante su creación.

<p align="right"><a href="#top">Ir al Inicio</a></p>

## Utilizando el Stack
A continuación, se describe brevemente la utilización del proyecto.

### Pre-requisitos
Solo es necesario tener instalado el [Docker](https://www.docker.com/products/docker-desktop) y el [Docker Compose](https://docs.docker.com/compose/install/)

### Estructura de Archivos
* `/cron-server` Contiene el _Dockerfile_ del contenedor.
* `/cron-server/crons` Contiene el archivo _root_ en donde se programa las tareas programadas que se deben ejecutar.

### Configurar el ambiente de desarrollo
En el directorio raíz, existe un archivo .env, el cual contiene los siguientes parámetros configurados.

#### Stack Options
* `COMPOSE_PROJECT_NAME`: Es el nombre del stack de contenedores que se generarán.

#### Server Options
* `SERVER_NAME`: El nombre que le daremos al contenedor del servidor Web.

### Instalar el ambiente de desarrollo
Una vez cambiado los parámetros deseados, se debe ejecutar el archivo `build.sh`

<p align="right"><a href="#top">Ir al Inicio</a></p>

## Licencia
Distribuido bajo Licencia MIT. Para más información, ver el archivo
[LICENSE](https://github.com/ricurdinola/docker-api-gateway/blob/main/LICENSE)

<p align="right"><a href="#top">Ir al Inicio</a></p>

## Contacto
Ricardo Urdinola - ricurdinola@gmail.com - [Mis Repositorios](https://github.com/ricurdinola?tab=repositories)

<p align="right"><a href="#top">Ir al Inicio</a></p>


[license-shield]: https://img.shields.io/github/license/ricurdinola/docker-lamp-stack?style=for-the-badge

[license-url]: https://github.com/ricurdinola/docker-api-gateway/blob/main/LICENSE

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555

[linkedin-url]: https://www.linkedin.com/in/urdinolaricardo/

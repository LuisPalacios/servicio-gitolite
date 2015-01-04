# Introducción

Este repositorio alberga un *contenedor Docker* para poder desplegar un Servidor Git con gitolite. Necesitas tener Docker instalado, te dejo un par de enlaces donde yo mismo empleo el contenido de este repositorio. Como Host uso un [servidor Linux basado en Gentoo](http://blog.luispa.com/index.php?controller=post&action=view&id_post=27) y aquí tienes la documentación sobre la [instalación de Docker](http://blog.luispa.com/index.php?controller=post&action=view&id_post=38)

También me apoyo en el programa [fig](http://www.fig.sh/index.html). Al ejecutarlo y leer el fichero fig.yml se crearán un contenedor con el servicio SSH y Gitolite.

Consulta este [apunte técnico sobre varios servicios en contenedores Docker](http://www.luispa.com/?p=172) para acceder a otros contenedores Docker y sus fuentes en GitHub.


# Instalación

Se emplean una imagen disponible en el [Docker Hub Registry](https://registry.hub.docker.com/)

* [luispa/base-gitolite](https://registry.hub.docker.com/u/luispa/base-gitolite/)

Para instalar primero tienes que tener el fichero fig.yml, así que clona el repositorio

    $ git clone https://github.com/LuisPalacios/servicio-gitolite.git
    :
    $ mv fig-template.yml fig.yml  (edita para adaptar a tu gusto)
    :
    $ fig up -d

# Configuración

Tendrás que elegir entre hacer una instalación nueva o migrar una existente, dejo aquí documentado todo el proceso:

* [Servidor "gitolite" en Contenedor Docker](http://www.luispa.com/?p=184)

Licencia
=========

Este archivo pertenece a la aplicación "practica 3" bajo licencia GPLv2. Copyright (C) 2014 Juan Moral Fernández.

Este programa es software libre. Puede redistribuirlo y/o modificarlo bajo los términos de la Licencia Pública General de GNU según es publicada por la Free Software Foundation, bien de la versión 2 de dicha Licencia o bien (según su elección) de cualquier versión posterior.

Este programa se distribuye con la esperanza de que sea útil, pero SIN NINGUNA GARANTÍA, incluso sin la garantía MERCANTIL implícita o sin garantizar la CONVENIENCIA PARA UN PROPÓSITO PARTICULAR. Véase la Licencia Pública General de GNU para más detalles.

Debería haber recibido una copia de la Licencia Pública General junto con este programa. Si no ha sido así, escriba a la Free Software Foundation, Inc., en 675 Mass Ave, Cambridge, MA 02139, EEUU.


Práctica 1:  Creación y despliegue de una aplicación en un PaaS.
===========

Para esta práctica utilizaré OpenShift. Openshift es un PaaS perteneciente a Red Hat, que usa además git 
para la gestión de aplicaciones.

Inicialmente, debemos registrarnos en OpenShift, tal como hice en el ejercicio 13 del tema 1. Una vez registrado, debemos tener instalado en nuestro sistema git, con el comando:

>sudo apt-get install git

Una vez instalado y configurado git, sincronizamos el repositorio donde se aloja la aplicación con nuestra máquina local a través del comando que OpenShift nos proporciona al crear una app. En el siguiente pantallazo podemos apreciarlo:

![im1](https://dl.dropbox.com/s/nex58rc3jds1ib4/Captura%20de%20pantalla%20de%202014-01-16%2023%3A55%3A56.png)


Tenemos el repositorio en nuestro ordenador, concretamente en la carpeta ~/practica1iv. La aplicación es una simple página web que muestra una imagen, que para el propósito de la práctica, nos vale. Ahora introducimos en
~/practica1iv/php nuestra aplicación php y sincronizamos con OpenShift a través de los siguientes comandos:

> git commit -m "confirmado"
> git push

Ya tenemos nuestra aplicación subida a OpenShift. Para acceder a ella entramos en:

>http://practica1iv-app1jm91.rhcloud.com/

![im2](https://dl.dropbox.com/s/03aufp4hurrvb56/Captura%20de%20pantalla%20de%202014-01-17%2001%3A18%3A23.png)



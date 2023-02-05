##### DevOps Project by: sziinocolanino@gmail.com

                                        <ReactJs, Django and Docker project>

### ReactJs
[![My Skills](https://skillicons.dev/icons?i=react)](https://skillicons.dev)
 >Con nuestro frontend en ReactJs nos comunicamos con Django a travez de Axios. De esta forma consumimos el puerto :8000/wel. De esta forma mostramos en pantalla la request que carguemos en Django a travez de los inputs: usuario y password.

### Django
[![My Skills](https://skillicons.dev/icons?i=django)](https://skillicons.dev)

--Usamos Django para realizar una *REST API* facil y simple, donde podemos llenar dos inputs: usuario y password, esto se almacena en la *DBSQLite*, para luego consumirlo con el frontend-reactjs.

--Creamos un entorno virutal para mantener las versiones que necesitemos sin colisionar con los demas. Pero vamos a ignorarlo en el .dockerignore. para luego instalar las librerias necesarias dentro del contenedor a la hora de buildear y correr el proyecto.

-Librarie & version installed in docker container:
 - djangorestframework 3.12.4
 - django-cors-headers 3.7.0
 - asgiref 3.3.1
 - Django 3.1.7
 - pytz 2021.1
 - sqlparse 0.4.1

# ¿Como arrancar el proyecto en localhost?

##### Para correr este proyecto en tu local necesitamos instalado localmente:
- Docker:latest
- Docker-compose:latest

>   En el folder 'deploy' por un lado tenemos el docker-compose.yml que esta preparado para buildear y/o correr las dos imagenes que generamos con el frontend-reactjs y el backend-django.
 
### /deploy

Cuando nos posicionamos en la carpeta /deploy ejecutamos en terminal el siguiente comando 'chmod +x init.sh', 
de esta forma le das a tu ordenador los permisos necesarios para ejecutar los scripts.

 El archivo lo ejecutamos escribiendo './init.sh' en la terminal y automaticamente va a buildear el Frontend y el Backend, una vez finalizado va a correr las dos imagenes.

###  PORTS
>Los puertos expuestos seran:
    - python-django: 8000
    - reactjs: 3000

---
[![My Skills](https://skillicons.dev/icons?i=docker)](https://skillicons.dev)
Install docker:latest
Install docker-compose:latest

#### In /frontend-reactjs
>In frontend-reactjs folder build Dockerfile with: docker build --tag frontend-reactjs
build image and we can run the image.
In the same folder script: docker run --publish 3000:3000 frontend-reactjs
arrancamos la imagen llamada "frontend-reactjs" en el puerto 3000:3000 publicamente

#### In /backend-django/project
> build Dockerfile with next script: docker build --tag  backend-django
build image and install requirements.txt, all libraries necesarys
In backend-django/project folder build Dockerfile with next script: docker run --publish 8000:8000 backend-django

---



![https://www.linkedin.com/in/stefano-ziino-colanino-199898160/][linkedin-shield]

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555





<!-- 


## DevOps Project by: sziinocolanino@gmail.com

ReactJs, Django and Docker project

Para correr este proyecto en tu local necesitas tener docker y docker-compose instalados localmente.

En el folder 'deploy' por un lado tenemos el docker-compose.yml que esta preparado para buildear o correr las dos imagenes que generamos con el frontend-reactjs y el backend-django. 


## ¿Como arrancar el proyecto en localhost?

 ## /deploy

Cuando nos posicionamos en la carpeta /deploy ejecutamos en terminal el siguiente comando 'chmod +x init.sh', de esta forma le das a tu ordenador los permisos necesarios para ejecutar los scripts.
 El archivo lo ejecutamos escribiendo './init.sh' en la terminal y automaticamente va a buildear el Frontend y el Backend, una vez finalizado va a correr las dos imagenes.

con el que automatizamos el build y el run del frontend-reactjs y backend-django docker y docker-compose
Pass 1: give you permissions init.sh file with the next command in terminal ' chmod +x init.sh '
Pass 2: script ./init.sh in terminal to execute sh
with he we make a build and run the images: python-django y frontend-reactjs

## PORTS

Los puertos expuestos seran:
    - python-django: 8000
    - reactjs: 3000


## DOCKER
[![Docker][Docker.yml]][https://www.docker.com/]

install docker
install docker-compose
creamos nginx.conf 

Nginx is a web server that can also be used as a reverse proxy, load balancer, mail proxy and HTTP cache.



## DJANGO
[![Django][Django.py]][https://www.djangoproject.com/start/]

Usamos Django para realizar una REST API facil y simple, donde podemos llenar dos inputs: usuario y password, esto se almacena en la DBSQLite, para luego consumirlo con el frontend-reactjs.

Con pip vamos a instalar virtualenv para generar nuestro entorno virtual y mantener las versiones que necesitemos sin colisionar con los demas entornos.

Ignoramos en .dockerignore. la carpeta 'env' que es nuestro entorno virtual creado para desarrollar en localhost, luego instalamos las siguientes librerias que son necesarias para que funcione dentro del contenedor.

Librarie & version, installed in VE in build:
 - djangorestframework 3.12.4
 - django-cors-headers 3.7.0
 - asgiref 3.3.1
 - Django 3.1.7
 - pytz 2021.1
 - sqlparse 0.4.1

## REACT
[![React][React.js]][https://reactjs.org/docs/getting-started.html]

reactjs show users created on backend.
 Con nuestro simple frontend en reactJs podemos comunicarnos con el backend-django a travez de Axios. De esta forma consumimos el puerto :8000/wel donde recibiremos la request con el Json que se carga en django a travez de los inputs: usuario y password.


[![LinkedIn][linkedin-shield]][https://www.linkedin.com/in/stefano-ziino-colanino-199898160/]
[![][]]

   -->

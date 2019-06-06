This project was bootstrapped with Create React App.

## Proyecto 1 de la materia Topicos Especiales en Telematica

### Enunciado
Se requiere el desarrollo de una aplicación de registro de posición (tracking-gps) en tiempo real (tipo IoT) utilizando un framework web moderno (javascript, angular, nodejs, o ruby, django-python, etc), utilizando mejores prácticas DevOps para integración y entrega continua distinguiendo los diferentes ambientes.

### Ambientes Utilizados
#### Desarrollo
#### Pruebas (DCA IP Privada y Docker con dominio correspondiente)
#### Produccion (Maquina CentOs7 de AWS)
#### Implemetacion

### 0. Requisitos
##### Docker
##### Docker-compose
##### Node

### 1. Log-in y Sign-in
Para la parte de autenticacion del usuario se uso Google Firebase ya que era la manera mas rapida y facil de conectar al framework del proyecto (React.js)

### 2. Mapa y Tracking
Para la parte del tracking se uso una API de Google Maps y unas funciones en el framework para que usara la localizacion actual del usuario, esta se actualiza cada 3 segundos y al darle el boton Empezar, se imprimira la localizacion en la pagina hasta que el usuario le de en el boton Parar

### 3. Configuración de Firebase

Crear una cuenta de Google Firebase:

![Input](misc/unknown.png)

Crear un proyecto:

![Input](misc/unknown2.png)

Seleccionar el tipo de proyecto:

![Input](misc/unknown3.png)

![Input](misc/unknown4.png)

![Input](misc/unknown5.jpeg)

Ubicar la configuración de Firebase resultante en /src/config/Fire.js:

![Input](misc/unknown6.jpeg)

### 4. Configuración Google Cloud / Kubernetes 

Crear un proyecto en Google Cloud

![Input](misc/unknown7.jpeg)

Entrar al menu principal e ingresar a la región de compute

![Input](misc/unknown8.jpeg)

Se puede desplegar el proyecto en una VM

![Input](misc/unknown9.jpeg)

Aqui, se puede seguir esta guía para terminar la configuración: 
https://cloud.google.com/kubernetes-engine/docs/quickstart

![Input](misc/unknown10.jpeg)

### 5. Correr la app

Para construir la aplicación despues de clonar el repositorio, se usa el comando ```` $ docker-compose up --build````

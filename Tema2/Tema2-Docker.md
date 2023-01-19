## Tares 2 - Imágenes

1. Descarga las siguientes imágenes: ubuntu:18.04, httpd, tomcat:9.0.39-jdk11,jenkins/jenkins:lts, php:7.4-apache.

Descargamos las imágenes, una a una:

```bash
docker pull ubuntu:18.04
```
```bash
docker pull httpd
```
```bash
docker pull tomcat:9.0.39-jdk11
```
```bash
docker pull jenkins/jenkins:lts
```
```bash
docker pull php:7.4-apache
```
![](assets/ejercicio1-parte1.png)
![](assets/ejercicio1-parte2.png)

2. Muestras las imágenes que tienes descargadas.

Mostramos la imágenes en el registro local: 

```bash
docker images
```
![](assets/tema2-ejercicio2.png)

3. Crea un contenedor demonio con la imagen php:7.4-apache.

Creamos un contenedor demonio con la imagen php que acabamos de descargar con la opción -d para que siga activo incluso sin estar en él y con la opción --name para darle el nombre que queramos, en este caso se llamara "contenedor-php".

```bash
docker run -d --name contenedor-php php:7.4-apache
```
Comprobamos que se ha creado bien: 

```bash
docker ps -a
```

![](assets/ejercicio3.png)



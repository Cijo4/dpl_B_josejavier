# Practica 2.3

## José Javier Sánchez

## 1. Instalar Nginx

Para instalar nginx primero hacer un apt update para listar los paquetes
disponibles y luego apt install nginx para instalarlo

~~~
sudo apt update
sudo apt install nginx
~~~

![update](update.png)

![install](instalNginx.png)

## Configurar firewall

Para este punto nos recomiendan tener habilidato el perfil mas restrictivo.
En mi caso tengo habilitado el 80.
Para habilitarlo usaremos el siguiente comando:

`sudo ufw allow 'Nginx HTTP'`

![allow](allow.png)

Podemos comprobar que se ha realizado el cambio con:

`sudo ufw status`

![status1](status1.png)

## 3. Comprobar el estado del servidor web.

Posteriormente comprobamos el estado del servicio con:

`sudo systemctl status nginx`

![status](status2.png)

Podemos comprobar que el servicio esta activo yendo a la maquina de windows
y poniendo nuestra ip en el navegador.

![nginx](nginx2.png)

Como se ve en la imagen tuve que cambiar el index predeterminado en ubuntu server
dado que, incluso con el apache deshabilitado, me seguia saliendo la pagina de 
apache. De esta manera hacemos que el index predeterminado sea el de nginx.

## 4. Administrar el proceso de Nginx

Por último comprobaremos el funcionamiento de algunos de los comandos básicos 
de administracion.

> Para detener el servidor web:

`sudo systemctl stop nginx`

> Para iniciar el servidor web cuando no esta activo:

`sudo systemctl star nginx`

> Para detenerlo e iniciar el servicio de nuevo:

`sudo systemctl restart nginx`

> Recargar el servicio sin cerrar conexiones:

`sudo systemctl reload nginx`

> Para deshabilitar el servicio:

`sudo systemctl disable nginx`

> Para habilitar el servicio:

`sudo systemctl enable nginx`

  



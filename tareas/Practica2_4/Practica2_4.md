# Práctica 2.4 Instalacion de Tomcat en Ubuntu Server

## José Sánchez

## Instalar Tomcat 9

Para la instalacion de Tomcat haremos como en anteriores ocasiones, acutalizaremos
las listas de paquetes con

`sudo apt update`

y instalaremos Tomcat 9 con

`sudo apt install -y tomcat9 tomcat9-admin`

> imagen

> imagen

## Configurar el firewall

Para acceder al Tomcat en Ubuntu deberemos añadir la siguiente regla:

`sudo ufw allow 8080/tcp`

> imagen

## Configuración de Tomcat9 en ubuntu server

 

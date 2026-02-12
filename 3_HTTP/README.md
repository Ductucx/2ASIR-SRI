#  TAREA HTTP/HTTPS

## ÍNDICE

1. [Bloque 1 - Apache como servidor principal](#bloque-1---apache-como-servidor-principal)
2. [Bloque 2 - HTTPS](#bloque-2---https)
3. [Bloque 3 - Startups](#bloque-3---startups)
4. [Bloque 4 - Extras](#bloque-4---extras)
  - 4.1. [Headers](#headers)
  - 4.2. [Error 404](#error-404) 
  - 4.3. [Comprobaciones](#comprobaciones) 
  - 4.3.1. [No autorizado](#no-autorizado) 
  - 4.3.2. [Autorizado](#autorizado) 
5. [Bloque 5 - Clientes](#bloque-5---clientes)
6. [Bloque 6 - Nginx](#bloque-6---nginx)
7. [Bloque 7 - Caddy](#bloque-7---caddy)

</br>

## Bloque 1 - Apache como servidor principal

Para instalar apache2:

```sh
sudo apt update
sudo apt install apache2
```

![alt image](./IMG/captura1-1.png)

En AWS copiamos nuestra IP pública para el ssh y habilitamos puertos para que no de problemas el "firewall":

![alt image](./IMG/captura1-2.png)

![alt image](./IMG/captura1-3.png)

![alt image](./IMG/captura1-4.png)

![alt image](./IMG/captura1-5.png)

Instalamos lo siguiente

```sh
sudo apt update
sudo apt install ddclient
```

![alt image](./IMG/captura1-6.png)

![alt image](./IMG/captura1-7.png)

![alt image](./IMG/captura1-8.png)

![alt image](./IMG/captura1-9.png)

![alt image](./IMG/captura1-10.png)

![alt image](./IMG/captura1-11.png)

![alt image](./IMG/captura1-12.png)

Y si hacemos un ping a nuestro dominio, vemos que encuentra la IP pública:

![alt image](./IMG/captura1-13.png)

Vamos a crear una página de ejemplo para comprobar su correcto funcionamiento:

![alt image](./IMG/captura1-14.png)

![alt image](./IMG/captura1-15.png)

![alt image](./IMG/captura1-16.png)

![alt image](./IMG/captura1-17.png)

![alt image](./IMG/captura1-18.png)

![alt image](./IMG/captura1-19.png)

![alt image](./IMG/captura1-20.png)

## Bloque 2 - HTTPS

Ejecutamos:

```sh
sudo apt update
sudo apt install certbot python3-certbot-apache
```

![alt image](./IMG/captura2-1.png)

![alt image](./IMG/captura2-2.png)

![alt image](./IMG/captura2-3.png)

![alt image](./IMG/captura2-4.png)

![alt image](./IMG/captura2-5.png)

![alt image](./IMG/captura2-6.png)

![alt image](./IMG/captura2-7.png)


## Bloque 3 - Startups

![alt image](./IMG/captura3-1.png)

![alt image](./IMG/captura3-2.png)

![alt image](./IMG/captura3-3.png)

![alt image](./IMG/captura3-4.png)

![alt image](./IMG/captura3-5.png)

![alt image](./IMG/captura3-6.png)

![alt image](./IMG/captura3-7.png)

![alt image](./IMG/captura3-8.png)

![alt image](./IMG/captura3-9.png)

![alt image](./IMG/captura3-10.png)

![alt image](./IMG/captura3-11.png)


## Bloque 4 - Extras

![alt image](./IMG/captura4-1.png)

![alt image](./IMG/captura4-2.png)

![alt image](./IMG/captura4-3.png)

![alt image](./IMG/captura4-4.png)

---
### Headers

![alt image](./IMG/captura4-5.png)

En `/etc/apache2/sites-available/terraformadoresasired-le-ssl.conf` :

![alt image](./IMG/captura4-6.png)

![alt image](./IMG/captura4-7.png)

![alt image](./IMG/captura4-8.png)

![alt image](./IMG/captura4-9.png)

---
### Error 404

Dentro del archivo de configuración de `/etc/apache2/sites-available/terraformadoresasired-le-ssl.conf` :

![alt image](./IMG/captura4-10.png)

![alt image](./IMG/captura4-11.png)

![alt image](./IMG/captura4-12.png)


---
### Comprobaciones

![alt image](./IMG/captura4-13.png)

---
#### No autorizado

![alt image](./IMG/captura4-14.png)

---
#### Autorizado

![alt image](./IMG/captura4-15.png)


## Bloque 5 - Clientes

![alt image](./IMG/captura5-1.png)

![alt image](./IMG/captura5-2.png)

![alt image](./IMG/captura5-3.png)

![alt image](./IMG/captura5-4.png)

![alt image](./IMG/captura5-5.png)

![alt image](./IMG/captura5-6.png)

![alt image](./IMG/captura5-7.png)

![alt image](./IMG/captura5-8.png)

![alt image](./IMG/captura5-9.png)


## Bloque 6 - Nginx

![alt image](./IMG/captura6-1.png)

![alt image](./IMG/captura6-2.png)

![alt image](./IMG/captura6-3.png)

![alt image](./IMG/captura6-4.png)

![alt image](./IMG/captura6-5.png)

![alt image](./IMG/captura6-6.png)

![alt image](./IMG/captura6-7.png)

![alt image](./IMG/captura6-8.png)

![alt image](./IMG/captura6-9.png)

![alt image](./IMG/captura6-10.png)

![alt image](./IMG/captura6-11.png)


## Bloque 7 - Caddy

```sh
sudo apt install -y debian-keyring debian-archive-keyring apt-transport-https curl
```

![alt image](./IMG/captura7-1.png)

![alt image](./IMG/captura7-2.png)

![alt image](./IMG/captura7-3.png)

![alt image](./IMG/captura7-4.png)
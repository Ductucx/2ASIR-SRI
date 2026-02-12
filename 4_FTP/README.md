#  TAREA FTP

## ÍNDICE

1. [Bloque 8 - Acceso mediante SFTP](#acceso-mediante-sftp)
2. [Bloque 9 - FTPS](#bloque-9---acceso-mediante-sftp)
3. [Bloque 11 - File Browser](#bloque-11---acceso-mediante-sftp)


</br>

## Bloque 8 - Acceso mediante SFTP

![alt image](./IMG/captura8-1.png)

![alt image](./IMG/captura8-2.png)

![alt image](./IMG/captura8-3.png)

En el cliente:

![alt image](./IMG/captura8-4.png)

![alt image](./IMG/captura8-5.png)

![alt image](./IMG/captura8-6.png)

Dentro del archivo de configuración de ftp:

![alt image](./IMG/captura8-7.png)

![alt image](./IMG/captura8-8.png)

Ejecutamos:

```sh
sudo systemctl restart ssh
```
![alt image](./IMG/captura8-9.png)

![alt image](./IMG/captura8-10.png)


## Bloque 9 - Acceso mediante SFTP

```sh
sudo apt update
sudo apt install vsftpd -y
```

![alt image](./IMG/captura9-1.png)

![alt image](./IMG/captura9-2.png)

![alt image](./IMG/captura9-3.png)

Esto crea:
- Clave privada → vsftpd.key
- Certificado → vsftpd.crt

```sh
sudo cat /etc/ssl/certs/vsftpd.crt /etc/ssl/private/vsftpd.key | sudo tee /etc/ssl/private/vsftpd.pem
```

![alt image](./IMG/captura9-4.png)

```sh
sudo nano /etc/vsftpd.conf
```

![alt image](./IMG/captura9-5.png)

![alt image](./IMG/captura9-6.png)

![alt image](./IMG/captura9-7.png)

![alt image](./IMG/captura9-8.png)

![alt image](./IMG/captura9-9.png)

![alt image](./IMG/captura9-10.png)

![alt image](./IMG/captura9-11.png)

```sh
“sudo systemctl restart vsftpd”
```

Y luego cambiamos reglas firewall aws

![alt image](./IMG/captura9-12.png)

![alt image](./IMG/captura9-13.png)

![alt image](./IMG/captura9-14.png)

![alt image](./IMG/captura9-15.png)


## Bloque 11 - Acceso mediante SFTP

![alt image](./IMG/captura11-1.png)

![alt image](./IMG/captura11-2.png)

![alt image](./IMG/captura11-3.png)

![alt image](./IMG/captura11-4.png)

![alt image](./IMG/captura11-5.png)

![alt image](./IMG/captura11-6.png)

![alt image](./IMG/captura11-7.png)

![alt image](./IMG/captura11-8.png)

![alt image](./IMG/captura11-9.png)

![alt image](./IMG/captura11-10.png)

![alt image](./IMG/captura11-11.png)

![alt image](./IMG/captura11-12.png)

![alt image](./IMG/captura11-13.png)

![alt image](./IMG/captura11-14.png)

![alt image](./IMG/captura11-15.png)

![alt image](./IMG/captura11-16.png)

![alt image](./IMG/captura11-17.png)

![alt image](./IMG/captura11-18.png)

![alt image](./IMG/captura11-19.png)
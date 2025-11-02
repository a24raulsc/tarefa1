### 1. Tomaremos a máquina darthsidious, e configuraremola para ser servidor secundario, tanto da zona primaria de resolución directa como de resolución inversa. Captura os ficheiros de configuración en ambalas dúas máquinas. Fai unha captura onde se vexa o reinicio da máquina darthsidious, no que se vexa no log dos dous equipos e que se fixo a transferencia de zona.
---

- Ficheiro named.conf.local de darthsidious

![alt text](imagenes3/darthsidious.png)
- Ficheiro named.conf.local de darthvader

![alt text](imagenes3/darthvader.png)
- Ficheiro named.conf.options (igual para ambos servidores)

![alt text](imagenes3/named.conf.png)

- Salida dos logs

![alt text](imagenes3/Imagen3.1.png)
![alt text](imagenes3/imaxen3.1.png)

### 2.Engade un rexistro tipo A (Chewbacca 192.168.20.28) na zona de resolución directa e tamén na de resolución inversa.  Fai unha captura no momento do reinicio do equipo darthvader, no que se vexa o log dos dous equipos e que se amose que se fixo a transferencia de zona. Adxunta tamén unha captura do ficheiro de zona no servidor secundario.
---

- Salida dos logs
![alt text](imagenes3/logs2sidious.png)
![alt text](imagenes3/logs2vader.png)

- Ficheiro de darthsidious
![alt text](imagenes3/ficheroSidious.png)


### 3.Comproba que o servidor secundario pode resolver ese nome.
---

![alt text](imagenes3/3.3.png)

### 4.Fai os cambios necesarios para que as trasferencias se fagan de forma segura empregando chaves.  Repite as capturas e vídeos do punto 2, engadindo o rexistro r2d2 (192.168.20.29)
---

- Salida dos logs
![alt text](imagenes3/logs3sidious.png)
![alt text](imagenes3/logs3vader.png)

- Ficheiro de darthsidious
![alt text](imagenes3/ficherosidious2.png)
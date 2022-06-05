archivo modificable en github

Creo el usuario diana con el comando adduser
![image](https://user-images.githubusercontent.com/105672800/172033549-3493851e-1eca-4274-bd57-d2eb1dda5a9f.png)

Creo el usuario Claudia adduser
![image](https://user-images.githubusercontent.com/105672800/172033561-32834102-92eb-4570-a817-e9457c6a8018.png)

Creo el usuario Laura adduser
![image](https://user-images.githubusercontent.com/105672800/172033566-88df013e-ab56-4811-b8cd-67d5acf9e5dd.png)

Listo los usuarios con el comando cat /etc/paswd

![image](https://user-images.githubusercontent.com/105672800/172033595-5b2bd2ec-c338-408b-a92c-ecd4c60b2328.png)

Creo el grupo profesor y estudiante con el comando addgroup
![image](https://user-images.githubusercontent.com/105672800/172033599-1b2c77dd-0e58-45a8-b321-3cff7b810791.png)
Ingreso a diana y Claudia al grupo de profesor con el comando usermod -a -G estudiante laura usermod -a -G profesor Claudia usermod -a -G profesor diana y lo listo con el comando cat /etc/group

![image](https://user-images.githubusercontent.com/105672800/172033604-a3ff2463-e103-49cb-a8f9-7c2e569e98ce.png)

Ingreso con los tres usuarios en diferentes terminales 

![image](https://user-images.githubusercontent.com/105672800/172033613-18528c25-20fc-44db-acbd-ff10f637f5fa.png)

Creo los directorios y les asigno el grupo al que pertenece con el comando chgrp estudiante soloEstudiantes y chgrp profesor soloProfesores y lo listo con ls –l para ver los permisos

![image](https://user-images.githubusercontent.com/105672800/172033619-0f268d10-40e6-47fe-bf6c-f00ccbc7a424.png)

Pruebo que Claudia crea un archivo1.txt vacio y Claudia como pertenece al mismo grupo puede leer y con el cat y escribir con el echo  en ese archivo


![image](https://user-images.githubusercontent.com/105672800/172033623-912c6036-b552-4472-973f-531cf9a88412.png)

Pruebo que laura puede leer el archivo de diana pero al momento de escribir sale permiso denegado por que no pertenece al mismo grupo y no cuenta con permiso de escritura 
![image](https://user-images.githubusercontent.com/105672800/172033628-9d99f9f7-142d-4afc-a267-f83c7828786c.png)


Creo archivos en cada usuario  
![image](https://user-images.githubusercontent.com/105672800/172033638-73def231-6203-4211-a43c-1d6d4d27b721.png)

Con el usuario root cambio dueño de propietario del arvhico 2 inicialmente de laura con el comando chown
![image](https://user-images.githubusercontent.com/105672800/172033645-3df6f046-94bd-4946-8d22-60d54c8d6380.png)

Cambio de propietario del archivo1 de diana al usuario de laura y del archivo de Claudia le cambio el propietario al usuario diana con el comando chown

![image](https://user-images.githubusercontent.com/105672800/172033655-d81387d3-993d-46cb-b354-0898289ef115.png)
En diferentes terminales trato de ingresar con contraseñas erróneas
![image](https://user-images.githubusercontent.com/105672800/172033660-967eee8f-7e48-465e-ada6-e1e4a5174700.png)

Utilizo comando sudo utmpdump /var/log/btmp
![image](https://user-images.githubusercontent.com/105672800/172033733-b8257c91-d51b-4c29-8e7b-9d5ae4a1fe06.png)Utilizo sudo utmpdump /var/log/wtmp
![image](https://user-images.githubusercontent.com/105672800/172033739-11b06dbf-76d4-42c0-a8d4-63706ecdea17.png)
Comprimo contenido del archivo de directorio de estudiantes con el comando zip -r Docs.zip
![image](https://user-images.githubusercontent.com/105672800/172033744-e7c5bc1e-6c52-4451-bbfa-5bbc5642e958.png)

Creo un alias para eliminar clave del usuario diana
![image](https://user-images.githubusercontent.com/105672800/172033747-39be218f-28c7-4cce-b177-fd2bc9a513ee.png)



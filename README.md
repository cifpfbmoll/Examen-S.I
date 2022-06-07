# Examen-S.I

## 1- Introducción.
Vamos a Dockerizar nuestro proyecto partiendo de una imagen de Docker HUB de tomcat

![image](https://user-images.githubusercontent.com/91556752/172448800-1b420cf5-dda1-4e3a-b7de-829926ef39e4.png)


    docker pull tomcat


![image](https://user-images.githubusercontent.com/91556752/171200982-ee431408-eee3-40d9-a030-637c79fabb87.png)

Como se puede ver en Docker desktop ya aparece nuestra imagen de Tomcat.

![image](https://user-images.githubusercontent.com/91556752/171201239-cfd4008a-eccb-46d1-98ab-0613b05f5fa7.png)



        docker run -d --name PiZhop -p 80:8080 tomcat



En Desktop 

![image](https://user-images.githubusercontent.com/91556752/171203694-00f40240-5d53-4786-adbe-250be3a772f4.png)

En este caso lo ejecutaremos por terminal.

![image](https://user-images.githubusercontent.com/91556752/171204505-bb24d069-8f68-4a1f-aeb7-ca9763dc18b4.png)
Ya lo tenemos creado y arrancado.

  




------
## 2- Configuración del archivo docker-compose.yml.
## 3- Pasos para el despliegue de la aplicación.
## 4- Preparación y subida de la imagen a dockerhub.
## 5- Conclusiones
## 6- Annexos (si lo consideráis necesario)

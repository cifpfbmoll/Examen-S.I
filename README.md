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

  


### Vamos a crear tanto dockerfile como docker-compose.yml con la ayuda de la extension de Visual Studio Code.

Una vez tenemos la extension creada, veremos este menu que nos permite ver mucha informacion de las imagenes, los contenedores y los volumenes de docker,la extension esta conectada ya con nuestra cuenta de Docker-Hub.



![image](https://user-images.githubusercontent.com/91556752/172450756-294b0273-23d7-47da-b9fe-61164223d7ce.png)






------
## 2- Configuración.

Con la extension de Docker del visual studio code nos vamos a la carpeta del proyecto que queremos dockerizar.


![image](https://user-images.githubusercontent.com/91556752/172451323-35165e5d-9518-4cca-9869-8b4771878ac4.png)


Vamos a hacer cmd+shift+p para desplegar el command panel.

![image](https://user-images.githubusercontent.com/91556752/172451785-729ecff2-9e0c-40cd-9647-322ad704db08.png)

![image](https://user-images.githubusercontent.com/91556752/172452338-10580270-24da-49c5-9f98-49841c95851e.png)


![image](https://user-images.githubusercontent.com/91556752/172452403-92fbf16f-ffc6-42ad-b7a3-c45ce9c571d3.png)



![image](https://user-images.githubusercontent.com/91556752/172452480-b173a849-648b-4672-a863-89731dc8b8ee.png)





Por ultimo nos pide si queremos el docker-compose.yml


![image](https://user-images.githubusercontent.com/91556752/172452718-b70df4e6-4964-4c10-ac2c-fb1bc0040c9b.png)



Con todo esto nos aparecera lo siguiente.

![image](https://user-images.githubusercontent.com/91556752/172453542-8661f1cc-a76a-45bc-9ff5-56640caaa147.png)


- Podemos ver que se han generado nuevos ficheros de docker, incluidos el dockerfile y el docker-Compose.



## 3- Pasos para el despliegue de la aplicación.

Una cosa muy a tener en cuenta es que en este proyecto hemos añadido las dependecias con Maven por lo cual nos ahorramos problemas con las dependencias del proyecto y tambien nos faciloita a la hora de dockerizar la aplicacion.

Anteriormente hemos hecho los pasos de descargar una imagen de docker-hub en este caso una de Tomcat pero no la vamos a utilizar ya que estamos utilizando la extension de Visual Studio Code y con el POM.XML vamos a indicar todas las dependencias necesarias a docker para que el proyecto pueda ir sin ningun problema.



Por este caso es muy recomendable tener un proyecto con Maven ya que nos va a ahorrar un monton de tiempo en la creacion de las dependencias y configuracion.

Este es nuestro docker-compose.yml

![image](https://user-images.githubusercontent.com/91556752/172455732-1daf2998-d3d6-41fe-afdc-4beb7f25cc4a.png)




## 4- Preparación y subida de la imagen a dockerhub.


Dentro del dokerfile
![image](https://user-images.githubusercontent.com/91556752/172458443-710ab779-948a-4bf3-820c-3270d8cc0df5.png)


![image](https://user-images.githubusercontent.com/91556752/172458600-65fccfb2-a09b-4a3d-bc6e-73d7f9706510.png)


![image](https://user-images.githubusercontent.com/91556752/172462752-1428ced1-c585-47fc-8d32-cf82085674e0.png)




Hcemos click derecho en el docker-compose.yml y selecionamos Compose Up -Select Services
![image](https://user-images.githubusercontent.com/91556752/172456545-120d0ce7-6a40-4d1b-b27e-41d326c68e37.png)

Selecionamos la opcion de nuestro proyecto.

![image](https://user-images.githubusercontent.com/91556752/172457694-dcfc49b8-ee31-4a0a-b2e3-e7fd8cf040b9.png)



![Uploading image.png…]()


## 5- Conclusiones
## 6- Annexos (si lo consideráis necesario)

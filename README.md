# Azure-WebPage-AppService
Creación de Página Web con el servicio de App Service de Azure

![Logo de WebPage](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-31.PNG)

## Requisitos

- Cuenta de [Azure](https://portal.azure.com/) con suscripción activa
- Cuenta de [Github](https://github.com/). Si no se tiene, es necesario seguir las instrucciones en el sitio para crear una nueva cuenta con su e-mail
- Computadora con Windows, Linux o MacOs
- [VSCode](https://code.visualstudio.com/) instalado
- [GIT](https://git-scm.com/downloads) instalado

---------------------------------------------------------

## Pasos

- Se inicia sesión en la página de [Azure](https://portal.azure.com/)

![Inicio Azure](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/inicio%20Azure.PNG)

- Se busca "App Services" y se presiona enter

![P6-1](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-1.PNG)

- En la nueva ventana seleccionamos "crear"

![P6-2](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-2.PNG)

- En el apartado "grupo de recursos" se selecciona "crear nuevo", se lecoloca un nombre y se presiona "aceptar"

![P6-3](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-3.PNG)

- Se le coloca un nombre al sitio web (debe ser único y estar disponible en el dominio) y se selecciona de pila "PHP 8.0" y SO Linux

![P6-4](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-4.PNG)

- En el apartado "SKU y tamaño" se da click en "cambiar el tamaño"

![P6-5](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-5.PNG)

- Se abrirá otra pestaña donde debemos seleccionar "1 GB de memoria gratis" y le damos en "aplicar"

![P6-6](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-6.PNG)

- Después presionamos "revisar y crear"

![P6-7](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-7.PNG)

- Esperamos a que se complete la validación y se habilite el botón "crear". Una vez habilitado, lo presionamos

![P6-8](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-8.PNG)

- Se mostrarará una ventana mientras se implementa el recurso 

![P6-9](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-9.PNG)

- Minimizamos la ventana y abrimos el administrador de archivos de windows, creamos una nueva carpeta vacia, la abrimos y seleccionamos la parte que muestra su ruta

![P6-10](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-10.PNG)

- Borramos lo que contiene, escribimos "cmd" y damos enter

![P6-11](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-11.png)

- Se abrirá una terminal de windows donde debemos escribir "git clone https://github.com/josejesusguzman/lab-subir-app-service-azure" y dar enter. Esto hará que se clone el proyecto de página web desde ese repositorio a nuestra carpeta.

![P6-12](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-12.PNG)

- Al terminar, nos mostrará algo como lo siguiente

![P6-13](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-13.PNG)

- Ahora abrimos Visual Studio Code, seleccionamos en la parte superior izquierda la pestaña "archivo" y luego "abrir carpeta"

![P6-14](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-14.png)

- Navegamos con el explorador de archivos hasta llegar a la carpeta que creamos anteriormente, la seleccionamos con un colo click y abajo le damos en "seleccionar carpeta"

![P6-15](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-15.PNG)

- Entramos a [Github](https://github.com/) e iniciamos sesión con nuestra cuenta

![P6-16](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-16.PNG)

- Ya dentro de nuestra cuenta, en la parte izquierda seleccionamos "nuevo" en el apartado de repositorios

![P6-17](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-17.PNG)

- Le damos un nombre, colocamos una pequeña descripción, desmarcamos la casilla de crear archivo "README.md" y damos click en "crear repositorio"

![P6-18](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-18.PNG)

- Se abrirá una página como la siguiente

![P6-19](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-19.PNG)

- Copiamos el link que se muestra en la imagen (único y diferente para cada usuario)

![P6-20](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-20.PNG)

- En Visual Studio Code, en la parte izquierda se da click derecho en donde dice "paginaweb" y después en "abrir en terminal integrada"

![P6-21](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-21.png)

- Se abrirá una terminal negra en la parte inferior, allí debemos escribir cada uno de los siguientes comandos y presionar entre después de cada uno:


git init

git add .

git commit -m "first commit"

git branch -M main

remote add origin <Aquí va tu link copiado anteriormente de github, por ejemplo: https://github.com/AlanAlvaradoR/Azure-WebPage-AppService.git>
  
git push -u origin main


- Ahora si volvemos a nuestra cuenta de github en el repositorio que creamos deberían aparecer los siguientes archivos

![P6-22](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-22.PNG)

- Ahora volvemos a la página del recurso de Azure que habíamos creado anteriomente, y debe mostrar un anuncio como el siguiente. Damos click en el botón de "ir al recurso"

![P6-23](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-23.PNG)

- En el menú lateral de la izquierda damos click en "centro de implementación"

![P6-24](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-24.PNG)

- En la opción de "origen" seleccionamos "github"

![P6-25](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-25.PNG)

- Se da click en el botón "autorizar" con lo que nos mandará a otra ventana donde debemos iniciar sesión con nuestra cuenta de github y otorgar los permisos correspondientes

![P6-26](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-26.PNG)

- Después nos mostrará la ventan anterior de Azure, aquí seleccionamos organización "ID de github", repositorio "nombre de tu repositorio" y rama "main"

![P6-27](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-27.PNG)

- Se da click en la parte superior en el botón de "guardar"

![P6-28](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-28.PNG)

- En el menú lateral izquierdo damos click en el apartado "introducción"

![P6-29](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-29.PNG)

- Nos desplegará un menú como el siquiente, donde debemos dar click en el link de "URL"

![P6-30](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-30.PNG)

- Nos abrirá otra pestaña donde ya esta creada y alojada nuestra página web de prueba

![P6-31](https://github.com/AlanAlvaradoR/Azure-WebPage-AppService/blob/main/imagenes/P6-31.PNG)


# Hello world with python

## Results
<p align="center">
    <img src="./public/img/results.png" alt="Hello from javascript">
</p>

## :open_book: How to use
* Clonar repositorio
    ```
    git clone
    ```
* Abrir el programa en un editor de codigo de su preferencia
* Posicionarse en la raiz del proyecto desde la terminal de su editor de codigo
* Ejecutar el comando: 
    ```
    uvicorn app:app --reload
    ```
* Visitar el `localhost` de su computador puerto `8000`
> [!TIP]
> Verificar que este en desuso el puerto seleccionado

## :rocket: How to run in docker
Visitar el siguiente enlance para conocer el proceso de generacion de la imagen del proyecto
### Como crear la imagen
```html
docker build -t <NEWIMAGENAME> .
<!-- Example -->
<!-- docker build -t pythonhello . -->
```
### Como ejecutar la imagen (Contenedor)
* Descargar del repositorio remoto la imagen

    `docker pull pamendeza/python_docker_project `
* Crear el contenedor a partir de la imagen
    ```html
    docker run -d --name <NEWDOCKERNAME> -p <PORT>:8000 <IMAGENAME>

    <!-- Example -->
    <!-- docker run -d --name pyhello -p 7000:8000 pamendeza/python_docker_project:v1.0 -->
    ```
    > [!TIP]
    > Si se desea mapear a un puerto diferente la aplicacion, unicamente se debe cambiar el numero de puerto que se encuentra a la izquierda debido a que el de la derecha es propio del contenedor y no se puede modificar.
### Como subir al repositorio remoto la imagen
* Colocar un tag a la imagen, en la cual se especifica el nombre o id de la imagen que deseamos subir seguido de el nombre de usuario de dockerhub, nombre del repositorio y version de la imagen
    ```html
    docker tag <IMAGENAME>||<IDIMAGE> <USERNAME>/<REPOSITORIENAME>:<VERSION>
    docker push  <USERNAME>/<REPOSITORIENAME>:<VERSION>
    <!-- Example -->
    <!-- docker tag pythonhello pamendeza/python_docker_project:v1.0 -->
    ```
* Subir la imagen tageada la cual consiste del nombre de usuario de dockerhub, el nombre del repositorio y la version de la imagen. Hacia el repositorio remoto
    ```html
    docker push  <USERNAME>/<REPOSITORIENAME>:<VERSION>
    <!-- Example -->
    <!-- docker push pamendeza/python_docker_project:v1.0 -->
    ```
    [View results](#results)
## :light_rail: PAAS Deploy (Railway)

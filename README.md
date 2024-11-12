# Hello world with python

## Results
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
```
docker pull 
docker run -d --name <NEWDOCKERNAME> -p <PORT>:8000 <IMAGENAME>
```
## :rocket: Como crear la imagen
```
docker build -t <NEWIMAGENAME> .
```
## :rocket: Como subir la imagen
```
docker tag <IMAGENAME>||<IDIMAGE> <USERNAME>/<REPOSITORIENAME>:<VERSION>
docker push  <USERNAME>/<REPOSITORIENAME>:<VERSION>
```
## :light_rail: PAAS Deploy with docker (Railway)
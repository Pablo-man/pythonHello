# Hello world with python

## Results
<p align="center">
    <img src="./public/img/results.png" alt="Hello from python">
</p>

## :open_book: How to use
### Pre-requisites
   * python
   * pip
   * Code editor
---
* Clone repository
    ```
    git clone
    ```
* Open the program in a code editor of your choice
* Position yourself at the root of the project from the terminal of your code editor
* Run the command:
    ```
    pip install requirements.txt

    uvicorn app:app --reload
    ```
* Visit your computer's `localhost` port `8000`
> [!TIP]
> Verify that the selected port is deprecated

## :rocket: How to run with docker
### Pre-requisites
* Docker - DockerDesktop installed
* DockerHub account
---
Visit the following link to learn about the process of generating the project image

:whale2: [GO](https://hub.docker.com/repository/docker/pamendeza/python_docker_project "Docker steps")

## :tennis: PAAS Deploy(Render) without Docker
Type of deployment was:

![Render Service](./public/img/type.png "Service")

Configurations:
* Build and start commmands to compile and execute the web application on render.

![Render Config](./public/img/conf.png "Configuration")

![Render Config](./public/img/conf1.png "Configuration")


State:

![Render Service](./public/img/renderDeploy1.png "Service")

![Render Service](./public/img/renderDeploy.png "Service")


:cake:[Hello World](https://go-docker-project.onrender.com/ "click for visit")
# <p align="center">DOCKER_Intro_by_David</p>


<div align="center" > 
 
<a href="#" >[![Buy Me A Coffee](https://img.shields.io/open-vsx/stars/redhat/java?color=D8B024&label=buy%20me%20a%20coffee&style=plastic)](https://www.buymeacoffee.com/DebtanuKhanra)‎</a>
 
</div>

<img width="1000" height="450" src ="https://user-images.githubusercontent.com/102660203/184363078-791e0da1-78fa-4b59-9db4-fad9e65e64d9.png" >

# <p align="center"> Introduction to Docker </p>

### Docker Overview:

Docker is an open platform for developing, shipping, and running applications. Docker enables you to separate your applications from your infrastructure so you can deliver software quickly. With Docker, you can manage your infrastructure in the same ways you manage your applications. By taking advantage of Docker’s methodologies for shipping, testing, and deploying code quickly, you can significantly reduce the delay between writing code and running it in production.


### Docker Architecture: 
Docker uses a client-server architecture. The Docker client talks to the Docker daemon, which does the heavy lifting of building, running, and distributing your Docker containers. The Docker client and daemon can run on the same system, or you can connect a Docker client to a remote Docker daemon. The Docker client and daemon communicate using a REST API, over UNIX sockets or a network interface. Another Docker client is Docker Compose, that lets you work with applications consisting of a set of containers.

<img width="1000" height="500" src="https://user-images.githubusercontent.com/102660203/184369704-f47f459d-250a-4ca0-8b6b-8a8deb36ad7d.png">

### 📌The Docker Daemon:
The Docker daemon (dockerd) listens for Docker API requests and manages Docker objects such as images, containers, networks, and volumes. A daemon can also communicate with other daemons to manage Docker services.

### 📌The Docker Client:
The Docker client (docker) is the primary way that many Docker users interact with Docker. When you use commands such as docker run, the client sends these commands to dockerd, which carries them out. The docker command uses the Docker API. The Docker client can communicate with more than one daemon.

### 📌Docker Desktop:
Docker Desktop is an easy-to-install application for your Mac or Windows environment that enables you to build and share containerized applications and microservices. Docker Desktop includes the Docker daemon (dockerd), the Docker client (docker), Docker Compose, Docker Content Trust, Kubernetes, and Credential Helper. For more information, see Docker Desktop.

### 📌Docker Registries: 
Docker registry is a storage component for Docker images. We can store the images in either public or private repositories. DockerHub is famous public cloud repository.
A Docker registry stores Docker images. Docker Hub is a public registry that anyone can use, and Docker is configured to look for images on Docker Hub by default. You can even run your own private registry.
When you use the docker pull or docker run commands, the required images are pulled from your configured registry. When you use the docker push command, your image is pushed to your configured registry.
Use of Docker Registries : We can control where your images are being stored. Integrate image storage with your in-house development workflow.

### 📌Docker Objects:
When you use Docker, you are creating and using images, containers, networks, volumes, plugins, and other objects. This section is a brief overview of some of those objects.

### 📌Docker images:
Docker images are read only template that can be used to create containers out of it. These docker images contains all the dependencies for a particular application or any microservice. You can create your own image and upload that onto the DockerHub and at the same time you can also pull the images which are available in the public repositories.

### 📌What are Docker containers:
Docker containers are nothing but the runtime instances of docker images. It contains everthing that is required to run an application or any microservice. It is also possible that more than one image is required to create a container. Docker containers can be referred to as isolated application platform built from one or more docker images.

### Problems before Docker:
A developer develops and runs an application. Now that application works in developer’s laptop but not in testing or production. This problem is arised due to difference in computing environment between developer, test and production team. In development environment there can be a software that is upgraded and in testing and production environment, the older version of software might be present.

### What is Docker?
Docker is a tool designed to make it easier to create, deploy, and run applications by using containers. Docker containers are lightweight alternatives to Virtual Machines and it uses the host OS. You don't have to pre-allocate any RAM in containers.

Dockerfile builds a docker image and that image contains all the project's code. You can run that image to create as many docker containers as you want. Then this image can be uploaded on DockerHub, from DockerHub anyone can pull the image and build a container.

<img width="1000" height="500" src="https://user-images.githubusercontent.com/102660203/184245024-32855f22-e625-49a4-8fff-cd81b580bb04.png">

Docker images are huge in size and requires a lot of network bandwidth. So in order to save that network bandwidth, we use Jenkins server or any continuous integration server to build an environment that contains all the dependencies for a particular application or a microservice and that build environment is deployed onto various teams like testing, staging and production.

<img width="1000" height="500" src="https://user-images.githubusercontent.com/102660203/184244756-3a3da576-8730-4b81-aedf-bdeca4961568.png">

Create complex requirements for a microservice within an easy-to-write Dockerfile. Then push the code to the Git repository. CI server pull it down and build the exact environment that will be used in production to run the test suite without needing to configure the CI server at all. Deploy it out to a staging environment for testers. Roll exactly what you had in development, testing, and staging into production.

<!--### What is Docker registry?
Docker registry is a storage component for Docker images. We can store the images in either public or private repositories. DockerHub is famous public cloud repository.

### Why use Docker Registries?
You can control where your images are being stored. Integrate image storage with your in-house development workflow.

What are Docker images?
Docker images are read only template that can be used to create containers out of it. These docker images contains all the dependencies for a particular application or any microservice. You can create your own image and upload that onto the DockerHub and at the same time you can also pull the images which are available in the public repositories.

What are Docker containers?
Docker containers are nothing but the runtime instances of docker images. It contains everthing that is required to run an application or any microservice. It is also possible that more than one image is required to create a container. Docker containers can be referred to as isolated application platform built from one or more docker images-->



### Docker Compose:
Suppose you have multiple applications on various containers and all those containers are linked together. So you don’t want to actually execute each of those containers one by one but want to run those containers at once with a single command. So here docker compose comes into picture.
Docker compose makes it easier to configure and run applications made up of multiple containers. For example, you define four containers in one YAML file and then run those four containers with a single command.

<img width="1000" height="500" src="https://user-images.githubusercontent.com/102660203/184245008-eaaa2d60-c752-4c8b-b8cb-0a2e61076c0d.png">



# 📝Note: 
  ***I try to make a note on Docker and also i want to declare that many topics are taken by me from difeerents type of sources.***<br>
<br>
<div align="center">

<img  height="40" src="https://img.shields.io/badge/😊Thanks🙏to%20all❤️‍🔥-000000?style=plastic&logoColor=white">

</div>











<!--![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
<img width="560" height="200" src="https://user-images.githubusercontent.com/102660203/184346168-cd92e109-a6ed-4101-bf94-76085a96bb3d.jpg">
<img  width="560" height="400" src="http://apachebooster.com/kb/wp-content/uploads/2017/09/docker-architecture.png">
<img width="560" height="400" src="https://user-images.githubusercontent.com/102660203/184245036-35a24369-d9e1-474b-a377-011894841259.png">
<img width="1000" height="450" src="https://user-images.githubusercontent.com/102660203/184245024-32855f22-e625-49a4-8fff-cd81b580bb04.png">
<img width="1000" height="450" src="https://user-images.githubusercontent.com/102660203/184244756-3a3da576-8730-4b81-aedf-bdeca4961568.png">
<img width="1000" height="450" src="https://user-images.githubusercontent.com/102660203/184245008-eaaa2d60-c752-4c8b-b8cb-0a2e61076c0d.png">
<!--![<Badge Name>](https://img.shields.io/badge/<Badge Text>-<Background Color>?style=for-the-badge&logo=<Icon Name>&logoColor=<Logo Color>)
![Buy me a coffee](https://img.shields.io/badge/buy%20me-000000?style=plastic&logoColor=white)
[![Buy Me A Coffee](https://img.shields.io/open-vsx/stars/redhat/java?color=D8B024&label=buy%20me%20a%20coffee&style=plastic)](https://www.buymeacoffee.com/DebtanuKhanra)‎ -->

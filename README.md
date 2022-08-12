# <p align="center">DOCKER_Info_by_David</p>

<img width="1000" height="450" src ="https://user-images.githubusercontent.com/102660203/184363078-791e0da1-78fa-4b59-9db4-fad9e65e64d9.png" >

# <p align="center"> Introduction to Docker </p>

<a href="#">![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) </a>




### Problems before Docker:-
A developer develops and runs an application. Now that application works in developer’s laptop but not in testing or production. This problem is arised due to difference in computing environment between developer, test and production team. In development environment there can be a software that is upgraded and in testing and production environment, the older version of software might be present.

### What is Docker?
Docker is a tool designed to make it easier to create, deploy, and run applications by using containers. Docker containers are lightweight alternatives to Virtual Machines and it uses the host OS. You don't have to pre-allocate any RAM in containers.

Dockerfile builds a docker image and that image contains all the project's code. You can run that image to create as many docker containers as you want. Then this image can be uploaded on DockerHub, from DockerHub anyone can pull the image and build a container.

<img width="1000" height="500" src="https://user-images.githubusercontent.com/102660203/184245024-32855f22-e625-49a4-8fff-cd81b580bb04.png">

Docker images are huge in size and requires a lot of network bandwidth. So in order to save that network bandwidth, we use Jenkins server or any continuous integration server to build an environment that contains all the dependencies for a particular application or a microservice and that build environment is deployed onto various teams like testing, staging and production.

<img width="1000" height="500" src="https://user-images.githubusercontent.com/102660203/184244756-3a3da576-8730-4b81-aedf-bdeca4961568.png">

Create complex requirements for a microservice within an easy-to-write Dockerfile. Then push the code to the Git repository. CI server pull it down and build the exact environment that will be used in production to run the test suite without needing to configure the CI server at all. Deploy it out to a staging environment for testers. Roll exactly what you had in development, testing, and staging into production.

### What is Docker registry?
Docker registry is a storage component for Docker images. We can store the images in either public or private repositories. DockerHub is famous public cloud repository.
Why use Docker Registries?
You can control where your images are being stored. Integrate image storage with your in-house development workflow.

### What are Docker images?
Docker images are read only template that can be used to create containers out of it. These docker images contains all the dependencies for a particular application or any microservice. You can create your own image and upload that onto the DockerHub and at the same time you can also pull the images which are available in the public repositories.

### What are Docker containers?
Docker containers are nothing but the runtime instances of docker images. It contains everthing that is required to run an application or any microservice. It is also possible that more than one image is required to create a container. Docker containers can be referred to as isolated application platform built from one or more docker images.

### Docker Compose:
Suppose you have multiple applications on various containers and all those containers are linked together. So you don’t want to actually execute each of those containers one by one but want to run those containers at once with a single command. So here docker compose comes into picture.
Docker compose makes it easier to configure and run applications made up of multiple containers. For example, you define four containers in one YAML file and then run those four containers with a single command.

<img width="1000" height="500" src="https://user-images.githubusercontent.com/102660203/184245008-eaaa2d60-c752-4c8b-b8cb-0a2e61076c0d.png">




















## 1. Docker Architecture

![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)

<img width="560" height="200" src="https://user-images.githubusercontent.com/102660203/184346168-cd92e109-a6ed-4101-bf94-76085a96bb3d.jpg">

<img  width="560" height="400" src="http://apachebooster.com/kb/wp-content/uploads/2017/09/docker-architecture.png">
<img width="560" height="400" src="https://user-images.githubusercontent.com/102660203/184245036-35a24369-d9e1-474b-a377-011894841259.png">
<img width="1000" height="450" src="https://user-images.githubusercontent.com/102660203/184245024-32855f22-e625-49a4-8fff-cd81b580bb04.png">
<img width="1000" height="450" src="https://user-images.githubusercontent.com/102660203/184244756-3a3da576-8730-4b81-aedf-bdeca4961568.png">
 <img width="1000" height="450" src="https://user-images.githubusercontent.com/102660203/184245008-eaaa2d60-c752-4c8b-b8cb-0a2e61076c0d.png">

# Springboot-Docker

Implementation of Java application and deployment of docker image of spring boot application within docker container.

Docker is a Linux container management toolkit with a “social” aspect, letting users publish container images and consume those published by others. A Docker image is a recipe for running a containerized process. In this implementation, we build one for a simple Spring boot application.

Docker helps you containerize your Java app — letting you bundle together your complete Spring application, runtime, configuration, and OS-level dependencies. This includes everything needed to ship a cross-platform, multi-architecture web application.
Docker uses a Dockerfile to specify each image’s “layers.” Each layer stores important changes stemming from the base image’s standard configuration. Create the following empty Dockerfile in your Spring Boot project.
Docker simplifies and accelerates your workflows by letting you freely innovate with your choice of tools, application stacks, and deployment environments for each project. You can run your Spring Boot artifact directly within Docker containers. This is useful when you need to quickly create microservices.


1. Run main method of SpringbootDockerDemoApplication.java
Now we can run the application without the Docker container (that is, in the host OS): we can now access your “Hello World” page through our web browser at http://localhost:8080/welcome

2. In the command prompt in root directory type: 

```
docker run -p 8081:8080 springboot-docker-demo .
```

Note that there is a dot (.) at the end, denoting the current directory.

3. You can see it pulls the image openjdk:11 from registry-1.docker.io, copies the WAR file and creates the image. To verify, type:

```
docker images
```


Go to Docker Dashboard and open your app in your browser: 

http://localhost:8081/welcome

Here we have mapped the application to 8081. You can map to same port like 8080 too.


We’ve demonstrated how to containerize our Spring Boot application, and why that’s so conducive to smoother deployment. We’ve also harnessed Docker Compose to construct a simple, two-layered web application. This process is quick and lets you devote precious time to other development tasks — especially while using Docker Desktop. No advanced knowledge of containers or even Docker is needed to succeed.

You can view the whole execution here: https://drive.google.com/file/d/1J8HzPgapuIH409KlwoGLs1ifhscD-zJF/view?usp=sharing

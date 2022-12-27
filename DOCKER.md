# Docker

* Docker is a tool designed to make it easier to create, deploy, and run applications by using containers. Containers allow a developer to package up an application with all of the parts it needs, such as libraries and other dependencies, and ship it one package.

* Docker is useful because it allows developers to create and manage containers on a single machine, making it easier to develop and test applications. It also allows applications to be easily transferred from one environment to another.

* Docker uses a client-server architecture. The Docker daemon (the server) listens for Docker API requests and manages Docker objects, such as images, containers, networks, and volumes. A command line interface (CLI) client, such as docker, allows users to interact with the Docker daemon through the command line.

* Here are some key terms to understand when working with Docker:

  * Image: A lightweight, stand-alone, executable package that includes everything needed to run a piece of software, including the application code, libraries, dependencies, and runtime.
  
  * Container: A running instance of a Docker image. A container is a lightweight, stand-alone, and executable package that includes an application and all of its dependencies.

  * Registry: A place where Docker images are stored and distributed. Docker Hub is a public registry that contains a large number of images, but you can also set up your own private registry.

  * Dockerfile: A text file that contains instructions for building a Docker image.

* Using Docker, developers can build, test, and deploy applications quickly and easily, making it a popular choice for modern development pipelines.

## Docker Image

* A Docker image is a lightweight, stand-alone, executable package that includes everything needed to run a piece of software, including the application code, libraries, dependencies, and runtime.

* An image is created by writing a set of instructions in a file called a Dockerfile. This file specifies the base image to use, any dependencies that need to be installed, and any additional commands that need to be run to set up the environment. Once the Dockerfile is complete, you can build the image using the docker build command.

* Once an image is built, it can be used to create and run Docker containers. A container is a running instance of an image, and it allows you to run the software in the image on any machine that has Docker installed.

* One of the benefits of using Docker images is that they are easy to share. You can push an image to a registry, such as Docker Hub, where it can be stored and accessed by others. This makes it easy to distribute applications and share them with other developers.

* Docker images are also useful for creating reproducible environments. Because an image includes everything needed to run the software, you can be sure that the environment will be the same wherever the image is run. This makes it easier to test and debug applications, as well as to deploy them to different environments.

## Docker Container

* A Docker container is a running instance of a Docker image. It is a lightweight, stand-alone, and executable package that includes an application and all of its dependencies.

* Containers allow you to package an application and its dependencies together, making it easy to deploy and run the application in any environment. Because the container includes everything needed to run the application, you can be sure that the environment will be the same wherever the container is run. This makes it easy to test and debug applications, as well as to deploy them to different environments.

* Containers are created from Docker images, which are templates for creating containers. To create a container, you can use the docker run command and specify the image you want to use. You can also pass in any additional arguments or configuration options that you want to use when running the container.

* Once a container is running, you can stop, start, or delete it using the appropriate Docker commands. You can also use the docker exec command to run additional commands inside the container, or the docker attach command to connect to the container and view its output in real-time.

* Docker containers are useful for a variety of applications, including microservices, continuous integration and delivery (CI/CD), and cloud-native applications. They are widely used in modern development pipelines because they allow developers to easily create and manage portable, reproducible environments for building, testing, and deploying applications.

## Dockerfile

* A Dockerfile is a set of instructions that tells Docker how to build the image. It consists of a series of command-line statements that are executed in order. Each statement begins with a command, followed by any arguments or options needed for that command.

* Here is a breakdown of some common Dockerfile commands:

  * FROM: Specifies the base image to use as the starting point for the build.
  * COPY: Copies files or directories from the host file system into the image.
  * ADD: Similar to COPY, but also supports extracting tar archives and fetching files from remote URLs.
  * RUN: Executes a command in a shell and commits the result to a new image layer.
  * ENV: Sets an environment variable in the image.
  * EXPOSE: Exposes a port to be used by the container at runtime.
  * WORKDIR: Sets the working directory for subsequent commands.
  * USER: Sets the user to use when running subsequent commands.
  * VOLUME: Creates a mount point for external volumes or bind mounts.
  * ENTRYPOINT: Specifies the default command to run when the image is run as a container.
  * CMD: Specifies the default arguments to pass to the ENTRYPOINT command.

* Note that the order of the commands in a Dockerfile is important, as each command is executed in order and the resulting image is built up layer by layer. It is also possible to use variables and conditionals in a Dockerfile, using the ARG and ONBUILD commands, respectively.

## Virtual Machine vs Container

* Virtual machines (VMs) and containers are both ways to isolate and run applications in a self-contained environment. However, they differ in how they achieve this isolation and the level of abstraction they provide.

* A VM is a software implementation of a physical computer that runs on top of a host operating system. It includes a full copy of the operating system, as well as a virtual hardware stack, including virtual CPUs, memory, and storage. This allows you to run multiple operating systems and applications on a single physical machine, each with its own isolated environment.

* A container, on the other hand, is a lightweight and portable package that includes an application and its dependencies, but not a full operating system. Instead, it relies on the host operating system to provide the necessary runtime environment and shared libraries. This means that containers are typically much smaller and faster to start than VMs, as they do not need to include a full operating system.

* Here are some key differences between containers and VMs:

  * Isolation: VMs provide full isolation at the hardware level, while containers provide isolation at the application level. This means that VMs can run multiple applications and operating systems in separate environments, while containers share the host operating system but isolate the application and its dependencies.
  
  * Abstraction: VMs provide a higher level of abstraction, as they include a full operating system and virtual hardware stack. Containers, on the other hand, provide a lower level of abstraction, as they rely on the host operating system and only include the application and its dependencies.
  
  * Size and performance: VMs are typically larger and slower to start than containers, as they include a full operating system and virtual hardware stack. Containers are smaller and faster to start, as they only include the application and its dependencies.

* Both VMs and containers have their own benefits and use cases. VMs are useful for running multiple operating systems and applications on a single physical machine, while containers are useful for creating lightweight and portable environments for deploying applications.

## Docker Compose

* Docker Compose is a tool for defining and running multi-container Docker applications. It allows you to use a docker-compose.yml file to define the services that make up your application, as well as the relationships between them and any associated dependencies. You can then use the docker-compose command to start, stop, and manage the services in your application.

* Here is an example of a docker-compose.yml file for a simple web application:

```yml
version: '3'
services:
  web:
    build: .
    ports:
      - "5000:5000"
    volumes:
      - .:/app
    depends_on:
      - db
  db:
    image: postgres
    environment:
      POSTGRES_USER: user
      POSTGRES_PASSWORD: password
      POSTGRES_DB: db
```

* In this example, the web service is built from the current directory (.) and exposes port 5000 on the host machine to port 5000 in the container. It also mounts the current directory as a volume in the container at /app, and depends on the db service. The db service is based on the postgres image, and sets environment variables for the PostgreSQL user, password, and database.

* With this docker-compose.yml file, you can use the docker-compose command to start the application and all of its services with a single command:

```cli
docker-compose up
```

* This command will build the web service, start the web and db services, and print their logs to the console. You can also use other docker-compose commands to stop, restart, or scale the services in your application.

* Docker Compose is useful for simplifying the process of defining and managing multi-container applications. It allows you to define all of the services and dependencies in a single file, making it easier to deploy and manage applications in different environments.

## Docker Workflow

![Docker Workflow via Microsoft](images/life-cycle-containerized-apps-docker-cli.png)

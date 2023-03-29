# Assessment


## Tools and Technologies used

* Spring boot 
* MongoDB
* Java
* Docker
* Kubernetes

## Quick start

### Clone the repository

```
git clone git@github.com:Swoyam1/Java-Project.git
```

### Build the project

```
cd "task-path"
docker-compose build
```

The project includes a ``web`` service, running the Java code, and a ``db`` service, running a MongoDB database.
See the ``docker-compose.yml`` file for details.

### Run the project

```
docker-compose up
````

Containers for both services will be launched. The project can be reached at http://localhost:8000.


## How to

### Run the local project on a different port

The container runs a Tomcat server listening on port 8080. The ``docker-compose.yml`` file is set up to
expose this port to the Docker host at port 8000, but you are free to change it as you wish - edit the ``ports`` directive:

```
services:
  web:
    [...]
    ports: 
      - 8000:8080
```



### External how-to guides

* [Spring Boot Integration with MongoDB](https://www.mongodb.com/compatibility/spring-boot/)
* [Securing a Web Application](https://spring.io/guides/gs/securing-web/)
* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/bookmarks/)

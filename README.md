# board
Service Link: http://springbootboardservice-env.eba-xppdbmk5.ap-northeast-2.elasticbeanstalk.com/posts/list

Running on local machines using Docker: type on the CLI docker pull igh9410/board:ver_1 


id: test
password: dummy

Spring Boot Web Board Service
View Templates: Thymeleaf
Language: Java
Framework: Spring Boot, Spring Security
Database: MySQL
APIs: JPA (Java Persistence API), Lombok, etc..


# Description
A simple CRUD board service made from scratch using Spring Boot Framework, Spring Security and JPA.
Not-logged-in users can only view posts.
Logged-in users can write, update, and delete their OWN posts.
Non-admins will be redirected to the access-denied page if they try to update or delete other users posts.
Admin is accessible to all CRUD operations.

Users can search posts by titles and contents.

# ERD          
![boardServiceERD](https://user-images.githubusercontent.com/31177070/178195912-df5f3e57-8156-46f0-a488-db85dae7aa1e.png)

# Update Logs
7/7/2022 - Added GlobalExceptionHandler class using @ControllerAdvice.
         - Added Custom Error Pages for Each Exception.
         
7/10/2022 - Migrated from Amazon Linux environment to Docker Environment


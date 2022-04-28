# Building RESTful API with Spring

<img align="right" length="100" width="350" src="https://user-images.githubusercontent.com/78484194/165760173-8d112485-b42b-40cd-bb35-8c447ce67475.png">

A service for managing a company's employee payroll and order status. 

## What I Have Learned?

This tutorial was my second contact with Spring and I found very enlightening to understand the difference between a common sense "REST" and  a full REST, as defined more or less by Roy Fielding. Just using URLs like "/employees/3", HTTP methods and having all CRUD operations is not enough to define a REST application. The core lies in creating hypelinks that enable relavant operations and drive client usage, by preventing users from hard-coding the URLs to navigate the API. To facilitate this, Spring provides a powerful dependency: Spring HATEOAS.

More specifically, I started to better assimilate some basic components of the Spring framework: Entity model, Controller, Repository. 
  
- **Entity model** defines an object that is available to be stored within a database, persting data in a SQL store.

- **Controller** handles inputs and tranforms it into a model. Specifically, the @RestController takes the data returned by the methods and places it directly in the response. Inside the controller, routes for the HTTP methods are created by using: @GetMapping, @PostMapping, @PutMapping and @DeleteMapping.

- **Repository** is a way of dealing with storing, retrieving, searching and deleting objects. In this apllication, we extended JpaRepository and specified the domain type as Employee and the id type as Long.


## References

[Spring Tutorial  -  Building REST services with Spring](https://spring.io/guides/tutorials/rest/)

[Spring Data JPA - Reference Documentation | Repositories](https://docs.spring.io/spring-data/jpa/docs/current/reference/html/#repositories)

[REST API Tutorial  -  What is REST](https://restfulapi.net/)

[Red Hat  -  What is REST API](https://www.redhat.com/en/topics/api/what-is-a-rest-api)


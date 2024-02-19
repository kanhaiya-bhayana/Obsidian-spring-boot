
#### Microservice
- Microservice is an approach to developing a single application as a suite of small services, each running in its own process and communicating with lightweight mechanism, built around business capabilities and independently deployable by fully automated deployment machinery.


#### Spring Bean
	Spring Bean is nothing special, **any object in the Spring framework that we initialize through Spring container is called Spring Bean.**

#### Spring - IoC Containers

The Spring container is at the core of the Spring Framework. The container will create the objects, wire them together, configure them, and manage their complete life cycle from creation till destruction. The Spring container uses DI to manage the components that make up an application. These objects are called Spring Beans.

#### Java Bean: Classes adhering to 3 constraints:
1. Having default (no-argument) constructor
2. Allow access to their properties using getter and setter
3. Implement java serializable 
#### POJO : Plain Old Java Object
1. No constraint
2. Any Java object is a POJO!

#### Spring Bean: Any Java object that is managed by Spring 
- Spring uses IOC containers (Bean Factory or Application Context) to manage these objects.

---
#### Difference B/w PUT & PATCH
- PUT & PATCH both performs modifications on existing data, but they do so differently because of idempotency.
- PUT modifies a record's information and creates a new record if one is not available. (Complete)
- PATCH updates a resource without sending the entire body in the request. (partially)

#### Implementing REST Services
REST (Representational state transfer) services are one of the most often encountered wats to implement communication between two web apps. 
REST offers access to functionality the server exposes through endpoints a client can call.

---
#### DTO (Data Transfer Object) pattern
- DTO pattern is a design pattern that allows you to transfer data b/w different part of your application.
- Are simple objects that contain only data, and they do not contain any business logic.
- This makes them ideal for transferring data b/w different layers of your application, such as the ***presentation layer*** and the ***data access layer***.

#### Benefits
	1. Reduce n/w traffic: can be used to batch up multiple pieces of data into a single object, which can reduce the number of n/w requests that need to be made.
		1. This can improve performance and reduce the load on your servers.
	2. Encapsulates serialization: can be used to encapsulate the serialization logic for transferring data over the wire.
		1. This makes it easier to change the serialization format in the future, without having to make changes to the rest of your application.
	3. Decouples layers: can be used to decouple the presentation layer from the data access layer.
		1. This makes it easier to change the presentation layer without having to change the data access layer.










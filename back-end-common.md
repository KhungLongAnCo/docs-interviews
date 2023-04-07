# Back end interview questions

1. **Example of a security threat in coding?**
    "One example of a security thread in coding is SQL injection attack. 
    It occurs when attacker inserts malicious code into a SQL statement, allow them to access and manipulate
    sensitive data stored in database. To prevented, developers must use parameterized and input validation.

    The second is Cross-site scripting(XSS) attacks: This occurs when an attackers injects malicious code into a website,
    which is then executed by unsupecting users who visit the site. This can allow the attacker steal sensitive 
    information, such as login credential or personal data."

2. **Prefer SQL or NoSQL? pros and cons of each type?**
    "I prefer using SQL and also I have more experience working with it

    SQL databases are relational databases that store data table with predefined database.
    Pros:
    + ACID compliance: It ensures data consistency and integrity even in the event of hardware or software failures.
    + Strong data consistency:  SQL databases enforce strict data consistency rules
    + Large ecosystem of tools and resources available
    Cons: 
    + Limited scalability: difficult to scale horizontally => limit their ability to handle large volumes of data or
    high traffic loads.
    Complex schema management: require a predefined schema -> difficult to manage in applications with rapidly changing data structures.
    + Limited flexibility:structured data ->  disadvantage in applications that require more flexibility.

    NoSQL are non-relational databases that store data in a variety of formats, including key-value, document and graph
    databases.
    Pros:
    Scalability: designed to scale horizontally, Flexibility, High availability
    Cons:
    + Limited consistency, Limited tooling"

3. **When to use SQL NoSQL?**
    "It depends on the specific needs and requirements of your business.
    The decision to use SQL or NoSQL databases should be based on factors such as the type of data you are storing, 
    the volume of data, the complexity of your queries, and the need for scalability and flexibility. It's important 
    to evaluate the pros and cons of each type of database and choose the one that best meets the needs of your business.
    In some cases, a combination of both SQL and NoSQL databases may be the best solution."

4. **What is Rest API?  POST/PUT? PATCH**
    - REST (Representational State Transfer) is an architectural style for building web services.
    - A RESTful API (Application Programming Interface) is a web service that follows the REST architecture.
    - It provides the API that clients can  interact with these resources using standard HTTP methods such as 
    GET, POST, PUT, and DELETE.The API returns data in a format such as JSON or XML.

    POST is used to create new resources.
    PUT is used to update existing resources
    PATCH is used to modify specific fields of existing resources.

5. **SQL injection - what is high availability**
    "SQL Injection is a type of security vulnerability that occurs when an attacker is able to inject malicious SQL
    code into a database query, allow them to access or modify data.

    High availability is the ability of system to still working even the hardware or software failure.
    Several way to achieve high availability in a database system: 
    + Replication: creating multiple copies of the database and keeping them in sync with each other. 
    If one copy of the database becomes unavailable, the system can switch to another copy to maintain availability.
    + Load balancing:  distributing incoming requests across multiple servers to ensure that no single server becomes 
    overloaded. If one server becomes unavailable, the load balancer can redirect traffic to another server to maintain
    availability.
    + Failover: switching to a backup system in the event of a failure. For example, if the primary database server fails,
    a backup server can take over to maintain availability."

6. **What is Redis? Application?**
    Redis is an open source, in-memory, key-value data store most commonly used as a primary database, cache, message broker, and queue. Redis delivers sub-millisecond response times, enabling fast and powerful real-time applications in industries such as gaming, fintech, ad-tech, social media, healthcare, and IoT 1. Redis is the de facto solution for caching in almost every application. Because Redis can handle millions of queries per second and offers high availability and scalability, it is used as a cache to reduce the load on a relational or NoSQL database

7. **What is microservice?**
    Microservices (or microservices architecture) is a cloud-native architectural approach in which a single application is composed of many loosely coupled and independently deployable smaller components, or services. Each service runs in its own process and communicates with clients, and often each other, using lightweight protocols, often over messaging or HTTP

8. **How do microservices talk to each other?**
    - Microservices communicate with each other by inter-service communication on network level. Each microservice has its own instance and process. Therefore, services must interact using an inter-service communication protocols like HTTP, gRPC or message brokers AMQP protocol
    - A microservice-based application will often use a combination of these communication styles. The most common type is single-receiver communication with a synchronous protocol like HTTP/HTTPS when invoking a regular Web API HTTP service. Microservices also typically use messaging protocols for asynchronous communication between microservices

9. **What is API gateway?**
    An API gateway is a server that acts as an API front-end, receives API requests, enforces throttling and security policies, passes requests to the back-end service and then passes the response back to the requester 
    API gateways sit between a user and a collection of microservices, providing three key services:
    -  Request routing: An API gateway receives a new API request, turns it into multiple requests, consults a routing map that determines which microservices are needed to fulfill the request, aggregates the results and sends them back to the requester.

    - API composition: The API gateway provides workflow orchestration as it combines multiple requests into a single request.

    -  Protocol translation: The API gateway translates between web protocols such as HTTP and WebSocket and web-unfriendly protocols that are used internally 

10. **Strict mode**
    Strict mode is a way to opt-in to a restricted variant of JavaScript . It is a subset of JavaScript that intentionally has different semantics from normal code . Strict mode makes several changes to normal JavaScript semantics 3. It eliminates some JavaScript silent errors by changing them to throw errors . It fixes mistakes that make it difficult for JavaScript engines to perform optimizations: strict mode code can sometimes be made to run faster than identical code that's not strict mode . It prohibits some syntax likely to be defined in future versions of ECMAScript.

    In strict mode, this will throw an error, making it impossible to accidentally create a global variable. In normal JavaScript, a developer will not receive any error feedback assigning values to non-writable properties. In strict mode, any assignment to a non-writable property, a getter-only property, a non-existing property, a non-existing variable, or a non-existing object will throw an error 

11. **RESTful API**
    A RESTful API is an architectural style for building web services that are scalable, flexible, and easy to maintain. REST stands for Representational State Transfer, and it is a set of guidelines for creating web services that use HTTP methods to perform CRUD (Create, Read, Update, Delete) operations on resources.

    Here are some key characteristics of a RESTful API:

    - **Stateless**: A RESTful API is stateless, meaning that each request contains all the information necessary for the server to understand and process the request. The server does not store any client context between requests.

    - **Resource-based**: A RESTful API is resource-based, meaning that it uses resources (such as users, products, or orders) to represent the data that is being manipulated. Each resource is identified by a unique URI (Uniform Resource Identifier).

    - **CRUD Operations**: A RESTful API uses HTTP methods (such as GET, POST, PUT, and DELETE) to perform CRUD operations on resources. For example, a GET request is used to retrieve a resource, while a POST request is used to create a new resource.

    - **Uniform Interface**: A RESTful API has a uniform interface, meaning that it uses a consistent set of rules and conventions for interacting with resources. This makes it easy for developers to understand and use the API.

    - **Hypermedia-driven:** A RESTful API is hypermedia-driven, meaning that it uses hyperlinks to navigate between resources. This allows clients to discover and interact with resources dynamically.

    In summary, a RESTful API is a web service that uses HTTP methods to perform CRUD operations on resources. It is stateless, resource-based, has a uniform interface, and is hypermedia-driven. RESTful APIs are widely used in web development and are considered a best practice for building scalable and flexible web services.
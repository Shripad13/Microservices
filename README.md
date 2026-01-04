# Monolith Project:
Multiple application Services/features will be in one Binary.
Lead to Big Application & Needs high Computing server.
For everytime entire server computing power required for processing request.
We dont have control of upsizing & downsizing a needed feature in Peak business hours.
Whenever release happens then entire Application will have impact.
Usually Legacy Application hosted as Monolith.

UI -- Business Logic -- Data Access Layer
   -----------------------------
              |
              |
          DB Server

# Microsevices Project:
    An Application is built as independent components that run each application process as a service.
1. Microservice allow developers to become language & tech agnostic.
2. 
3. In this case we have luxury to run different services using different technologies such as java, nodejs, pyhton etc
4. We can upsize & downsize specific service independently.
5. If one servie fails then Entire Application will not have outage, only specific service will have outage.
6. UI can talk to Multiple Services with each having different DB
7. How are you enable the communication between services.


# Interview Answer- 
Monolithic architecture is simple and suitable for small applications but becomes hard to scale and maintain as the system grows. Microservices architecture breaks the application into independent services, improving scalability and fault tolerance but increasing system complexity.  


> Frontend Tech - AngularJS, Flutter
> Backend Tech - Java, Python, nodejs, go
> DB Tech - MySQL, NoSql(MongoDB), Postgress

When to Use Sql - 
1. If your workload are transactional
2. If your data needs a standard format.
3. Ex- BankPassbook
   
When to use NoSql - (MongoDB)
1. When data is unstructured & not transactional
2. set of records, collection

Mater Data/ Business Data - Inject to DB for business needs.


## ROboSHop Project - 
11 servers, 11 security Groups, 11 DNS records
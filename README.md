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


> Problem with Monolith:
1. Scalability Issues: Scaling a monolithic application often means duplicating the entire application, which can be resource-intensive and inefficient.
2. Deployment Challenges: A small change in the codebase requires redeploying the entire application
3. Limited Technology Stack: Monolithic applications are typically built using a single technology stack, which can limit the ability to adopt new technologies or frameworks for specific components.
4. Tight Coupling: Components within a monolithic application are often tightly coupled, making it difficult to isolate and fix issues without affecting other parts of the application.
5. Slower Development Cycles: As the codebase grows, it can become more complex and harder to manage, leading to slower development cycles and increased risk of bugs.

# Microsevices Project:
    An Application is built as independent components that run each application process as a service.
1. Microservice allow developers to become language & tech agnostic.
2. 
3. In this case we have luxury to run different services using different technologies such as java, nodejs, pyhton etc
4. We can upsize & downsize specific service independently.
5. If one servie fails then Entire Application will not have outage, only specific service will have outage.
6. UI can talk to Multiple Services with each having different DB
7. How are you enable the communication between services.

> Microservices is the application architecture.

# Why microservices were great:
Scale only what you need
Isolated failures while other services are still running
Use Python for AI, Go for speed, Java for APIs
Each team owns its service(build, deploy, manage)
Fast deployments


# The problems with microservices:

Hard to manage many services: Deploying and monitoring 50+ services manually
Services keep crashing: No automatic restart when something fails
Difficult scaling: Manually adding/removing servers based on traffic
Complex networking: Services can’t find each other when IPs change
No health monitoring: Don’t know which services are healthy or sick

# Kubernetes solved the running containers at scale problem
We run microservices in Kubernetes
We run AI agents in Kubernetes
We run production databases in Kubernetes
Netflix, Uber, OpenAI, Medium, and a lot of top companies live on K8s


# Why Kubernetes won?
Perfect timing. Docker had made containers popular, so millions needed a solution to manage them. Kubernetes solved that exact problem.
Kubernetes Solved the Problems We Had with Microservices
Automatic service management: Kubernetes handles deploying and monitoring all your services
Auto-healing: When a service crashes, Kubernetes instantly starts a new one
Automatic scaling: Kubernetes adds/removes containers based on traffic automatically
Service discovery: Services can always find each other, even when IPs change
Health monitoring: Kubernetes constantly checks if services are healthy and replaces sick ones
Load balancing: Automatically distributes traffic across multiple copies of your service

# Should You Use Kubernetes?
Use Kubernetes when:
You have multiple services (5–10+)
You need to scale different parts independently
You need zero-downtime deployments
Your app needs high availability
You’re already using containers

# Don’t use Kubernetes when:
You have a simple app with 1–3 services
Your team is small (1–2 developers)
You’re just getting started with containers
You don’t need high availability

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
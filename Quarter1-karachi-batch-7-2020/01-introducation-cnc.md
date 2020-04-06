# Introduction to Cloud Native Computing


## Monolithic Computing

<p align="center">
  <img  src="https://raw.githubusercontent.com/etechlearner/cloud-native-mobile-web-computing/master/images/monolithic-architecture.png">
</p>

    Traditional way of computing called monolithic Architecture
    when we start Cloud native computing, let's look at what was heppening as a traditainal way of computing.
    Monolithic is defined in single line (very large,united design and diffecult to change problem)
  - composed all in one piece
  - self-contained 
  - tightly-coupled 
  - redeploy entire application on each update
  - slow down the start-up time
  - if bug in any module its bring down the entire process
  - its barrier to adopting new technologies and dependancy updated versions
  - application change become extremely expensive in both time and cost
-------------------------------------------------------------------------------------------------
## Microservices - also known as the microservice architecture

<p align="center">
  <img  src="https://raw.githubusercontent.com/etechlearner/cloud-native-mobile-web-computing/master/images/microservices-architecture.png">
</p>
    In this architectural style that structures an application as a collection of services that are. Highly maintainable and testable. Loosely coupled. Independently deployable. Organized around business capabilities.
   
   ### Microservices do have distinct advantages:
   #### Better Organization:
   - Microservice Architectures are typically better organized.
   - Each microservice has a very specific job, and it is not concerned with the jobs of other components.
   #### Decoupled:
   - Decoupled service are also easire to change, update and re-configure to serve te purposes of defferent apps.
   - They also allow for fast, independent delivery of individual parts within a larger, intergrated system.
   #### Performance:
   - Under the right circumstances, microserives can also have performance advantages depending on how they're origanized.
   - it's possible to isolate hot services and scale them independently of the rest of the app
-------------------------------------------------------------------------------------------------
## What is Cloud? 

<p align="center">
  <img  src="https://raw.githubusercontent.com/etechlearner/cloud-native-mobile-web-computing/master/images/cloud-c.jpg">
</p>

```
The word "cloud" refers to servers that are accessed over the Internet, and the software and databases that run on those servers. Cloud servers are located in data centers all over the world
```
```
In single line cloud can be describe as a "communications network".
```
```
A Cloud can be a wide area network (WAN) linke the public Internet or a private, national or global network. The term can also refer to a local area network (LAN) within an origanization.
```
   ### Type of Cloud:
   #### Private CLoud:
   - Deploying cloud computing internally.
   - Private cloud employs cloud computing with a company's own local or wide area networks
   #### Public CLoud:
   - A cloud computing service on the internet that is available to the general public
   - Commercial cloud providers like Amazon, Google Cloud, Azure etc
   #### Hybrid CLoud:
   - The user of both private and public clouds to provide an organization's computing needs

-------------------------------------------------------------------------------------------------

## Cloud Native Commputing Foundation (CNCF)


<p align="center">
  <img  src="https://raw.githubusercontent.com/etechlearner/cloud-native-mobile-web-computing/master/images/cloud-native-computing.jpg">
</p>


```
which is an open source software fundation dedicated to making cloude native computing universal and sustaninable describe cloud native as,
```
   *"Cloud native technologies empower organizations to build and run scalable applications in modern, dynamic enviroments such as public, private and hybird clouds"*
```
other defination of Cloud Native Computing could be
```
```
Let's get into detail and simpify to understand what we just heard  
```
   *"An Approach that builds software applications as microservices and runs them on a containerized and dynamically orchestrated platform to utilze the advantages of the cloud computing model"*
```
Cloud Native is about How applications are created and deployed, NOT WHERE  
```
   #### Cloud-native app development typically 
   - Devops
   - Agile mothodology
   - Microservice
   - Cloud computing platforms
   - Containerize application
   - Orchestration system
   - Continuous delivery

   *"  In short, every new and modern method of application deployment
"*

-------------------------------------------------------------------------------------------------

<p align="center">
  <img  src="https://raw.githubusercontent.com/etechlearner/cloud-native-mobile-web-computing/master/images/devops-whatisdevops.png">
</p>

## DevOps
    DevOps is an IT mindset that encourages communication, collaboration, integration and automation among software developers and IT operations in order to improve the speed and quality of delivering software.
   #### DevOps Lifecycle:
   #### Developer Task
   - **PLAN** Initially plan yourself regarding the type of application you need to develop. Make the rough picture regarding the development process

   - **CODE** the application as per the client requirement.  with the plan, you have made in the initial step.

   - **BUILD** the application by performing the integration of various codes you have done in the previous step. 

   - **TEST** This is the heart of the application. Test the application that you have built so far. And the rebuilt the application if necessary.
   
   #### Oprations Task
   - **RELEASES** If you succeed in the Test phase, then its time to release the application into Live.

   - **DEPLOY** the code into a cloud environment for further usage. It is performed in such a manner any changes made should not affect the functioning of high traffic website.

   - **OPERATE** Perform the operation on the code if any have.

   - **MONITOR** Monitor the performance of the application as per the client requirement. Keep a note on the performance of the application. Make modifications if any to satisfy the clients. And if does not reach up to the mark make changes in that particular area to satisfy the client.
   -------------------------------------------------------------------------------------------

## Agile 


<p align="center">
  <img  src="https://raw.githubusercontent.com/etechlearner/cloud-native-mobile-web-computing/master/images/Benefits-of-Agile.png">
</p>

    “Agile is a term used to describe approaches to software development emphasizing incremental delivery, team collaboration, continual planning, and continual learning. The term “Agile” was coined in 2001 in the Agile Manifesto.” Some people will say that it is just a mindset or way of thinking.

   #### Agile principles:
   - Agile methodology is described as an "iterative" and "incremental" approch
   - Agile developer visualize the software as a combination of complex parts that interacts with each other rather than a large block of structure
   - Actually, in waterfall method, development team will get only single chance to get each phase (like design, development, testing etc) of project 
   - Whereas in an agile methodology, these phases are continually reevisited  periodically to identify / understand the project's progress and direction 
   - The "inspect-and-adapt" approach from Agile methodology, greatly reduces development costs and time to market the product because here teams can develop the software while gathering changes in requirements
   - The stakeholders can provide feedback to the development team to improve the quality of the product
   - Agile development does save lot of resource which could have spent on something not needed anymore 

   -------------------------------------------------------------------------------------------

## Microservices

<p align="center">
  <img  src="https://raw.githubusercontent.com/etechlearner/cloud-native-mobile-web-computing/master/images/microservices.png">
</p>
    Cloud native provide standerd architecture of applications are built as system of miroservices.  

    Microservices - also known as the microservice architecture - is an architectural style that structures an application as a collection of services that are
   - Highly maintainable and testable
   - Loosely coupled
   - Independently deployable
   - Organized aroud business capabilities
   - Owned by a small team

    The microservice architecture enables the rapid, frequent and reliable delivery of large, complex applications. It also enables an organization to evolve its technology stack. 
   #### Challenges useing microservices:
   - there is a saying: there's no such thing as a free lunch
   - Microservices remove some complexity form the service themseleves and provide btter scalibility, but you're now building a distributed system
   - That adds a lot more complexity on the system level
   - To make sure that dependent services find each other and communicate efficienly its a challenging task when number of microservices are many 

   -------------------------------------------------------------------------------------------


## Twelve Factors App
<p align="center">
  <img  src="https://raw.githubusercontent.com/etechlearner/cloud-native-mobile-web-computing/master/images/The-12factore.png">
</p>
    In the modern era, software is commonly delivered as a service: called web apps, or software-as-a-service. The twelve-factor app is a methodology for building software-as-a-service apps that:

    The twelve-factor methodology can be applied to apps written in any programming language, and which use any combination of backing services (database, queue, memory cache, etc).
   #### Factors:
   - I. **Codebase** One codebase tracked in revision control, many deploys
   - II. **Dependencies** Explicitly declare and isolate dependencies
   - III. **Config** Store config in the environment
   - IV. **Backing services** Treat backing services as attached resources
   - V. **Build, release, run** Strictly separate build and run stages
   - VI. **Processes** Execute the app as one or more stateless processes
   - VII. **Port binding** Export services via port binding
   - VIII. **Concurrency** Scale out via the process model
   - IX. **Disposability** Maximize robustness with fast startup and graceful shutdown
   - X. **Dev/prod parity** Keep development, staging, and production as similar as possible
   - XI. **Logs** Treat logs as event streams
   - XII. **Admin processes** Run admin/management tasks as one-off processes


   -------------------------------------------------------------------------------------------

## Cloud Computing Platforms
## Containers
   - A Container is a runtime instance of an image
   - An Image is an executable package that includes everything needed to run an application
        - the code,
        - a runtime,
        - Libraries,
        - enviroment variables,
        - and configuration files,
   - Making a container using image for any application is called Containerization 
   - Docker is widely use to containerize your application 

    Containerization is iccreasingly popular because containers are:
   - **Flexible** : Even ther most complez applications can be containerized
   - **Lightweight** : Containers leveage and share the host kernel.
   - **Interchnageable** : You can deploy updates and upgrades on-the-fly.
   -  **Portable** : You can build locally, deploy to the cloud, and run anywhere.
   - **Scalable** : You can increase and automatically distribute cantainer replicas.
   - **Stackable** : You can stack services vertically and on-the-fly. 

## Orchestration
    Deploying your application with all dependencies into a container is jus the first step
    Every ease comes with it's own challenges, making ap containerized solves the deployment problems you had previously, but new challenges includes
   - Scaling app based on the current load of you system isn't that easy. You need to 
   - monitor your system 
   - trigger the startup or shutdown of container,
   - make sure that all required configration parameters are in piace,
   - balance the load between the avtive application instances 
   - share authentication secrets between your containers
   - Doing all of that manually requires a lot of effort and is too slow to react to unexpected changes in system load 
   - You need to have the right tools in place that automatically do all of this 
   - This is what the different orchestration solutions are build for 
   - One of the most popular on is **kubernetes**


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

- Agile 
- Microservice
- Cloud Computing Platforms
- Containers
- Orchestration



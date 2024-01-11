# Cloud-computing
Info regarding cloud computing

======
Cloud
======
"The cloud" refers to remote web servers in various data centers that host databases and run application code. Cloud providers deliver their services to customers or end users via the Internet. 

================
Cloud computing
================
In cloud computing, applications and data are hosted in remote servers in various data centers and accessed over the Internet. Data and applications are centralized in the cloud instead of being located on individual client devices (like laptops or smartphones) or in servers within a company's offices. Many modern applications are cloud-based, which is why, for example, a user can access their Facebook account and upload content from multiple devices.

=============
Multitenancy
=============
Multitenancy is when several different cloud customers are accessing the same computing resources, such as when several different companies are storing data on the same physical server. In cloud computing, multitenancy means that multiple customers of a cloud vendor are using the same computing resources. Despite the fact that they share resources, cloud customers are not aware of each other, and their data is kept totally separate. Multitenancy is a crucial component of cloud computing; without it, cloud services would be far less practical. Multitenant architecture is a feature in many types of public cloud computing, including IaaS, PaaS, SaaS, containers, and serverless computing.

In public cloud computing, customers of the cloud vendor use the same infrastructure – the same servers, typically – while still keeping their data and their business logic separate and secure.

The classic definition of multitenancy was a single software instance* that served multiple users, or tenants. However, in modern cloud computing, the term has taken on a broader meaning, referring to shared cloud infrastructure instead of just a shared software instance.

=========
What are the benefits of multitenancy?
Many of the benefits of cloud computing are only possible because of multitenancy. Here are two crucial ways multitenancy improves cloud computing:
1) Better use of resources: One machine reserved for one tenant is not efficient, as that one tenant is not likely to use all of the machine's computing power. By sharing machines among multiple tenants, use of available resources is maximized.
2) Lower costs: With multiple customers sharing resources, a cloud vendor can offer their services to many customers at a much lower cost than if each customer required their own dedicated infrastructure.

=========
What are the drawbacks of multitenancy?
Possible security risks and compliance issues: Some companies may not be able to store data within shared infrastructure, no matter how secure, due to regulatory requirements. Additionally, security problems or corrupted data from one tenant could spread to other tenants on the same machine, although this is extremely rare and should not occur if the cloud vendor has configured their infrastructure correctly. These security risks are somewhat mitigated by the fact that cloud vendors typically are able to invest more in their security than individual businesses can. The "noisy neighbor" effect: If one tenant is using an inordinate amount of computing power, this could slow down performance for the other tenants. Again, this should not occur if the cloud vendor has set up their infrastructure correctly.

======================
Serverless computing
======================
Serverless computing is a model in which applications are broken up into smaller pieces called functions, and each function only runs on demand, separately from the other functions. (This model of cloud computing is also known as function-as-a-service, or FaaS.)

As the name implies, serverless functions do not run on dedicated servers, but rather on any available machine in the serverless provider's infrastructure. Because companies are not assigned their own discrete physical servers, serverless providers will often be running code from several of their customers on a single server at any given time – another example of multitenancy.

======
Some serverless platforms use Node.js for executing serverless code. The Cloudflare serverless platform, Cloudflare Workers, uses Chrome V8, in which each function runs in its own sandbox, or separate environment. This keeps serverless functions totally separate from each other even when they’re running on the same infrastructure.

======
Servers are still used, but a company that gets backend services from a serverless vendor is charged based on usage, not a fixed amount of bandwidth or number of servers.  A company that gets backend services from a serverless vendor is charged based on their computation and do not have to reserve and pay for a fixed amount of bandwidth or number of servers, as the service is auto-scaling. Note that despite the name serverless, physical servers are still used but developers do not need to be aware of them.

=======
What are the main models of cloud computing?
The three main service models of cloud computing are:
1) Infrastructure-as-a-service (IaaS)
2) Platform-as-a-service (PaaS)
3) Software-as-a-service (SaaS)

=======
What is IaaS (infrastructure-as-a-service): Infrastructure-as-a-service (IaaS) refers to servers and storage that are hosted in the cloud.

Infrastructure-as-a-service, or IaaS for short, is when a cloud computing vendor hosts the infrastructure on behalf of their customers. The vendor hosts the infrastructure in "the cloud" – in other words, in various data centers. Their customers access this cloud infrastructure over the Internet. They can use it to build and host web applications, store data, run business logic, or do anything else that could be done on traditional on-premise infrastructure, but often with more flexibility.

======
IaaS vs. PaaS vs. SaaS

IaaS is infrastructure hosted in the cloud. IaaS includes virtual servers and cloud storage, cloud security, and access to data center resources (managed by the IaaS provider).

Platform-as-a-service (PaaS) is the next layer in the cloud computing service model. It provides developers with a platform for building applications. Most PaaS offerings include development tools, middleware, operating systems, databases and database management, and infrastructure. A PaaS provider either manages the infrastructure themselves or purchases it as a service from an IaaS provider.

Software-as-a-service (SaaS) is full applications hosted and managed in the cloud. SaaS users subscribe to an application and access it over the Internet rather than purchasing it once and installing it locally.

======
Multi-cloud deployments and most hybrid cloud deployments involve integrating multiple cloud services. Many businesses taking a multi-cloud approach use one cloud provider for IaaS and integrate with PaaS and SaaS services on top of that. Some companies may also use multiple IaaS providers, either for redundancy or for handling separate computing workloads in parallel.

Businesses using hybrid clouds can integrate IaaS with on-premise infrastructure or private clouds, along with other public cloud services

=============================
Software-as-a-service (SaaS)
=============================
Software-as-a-service, or SaaS for short, is a cloud-based method of providing software to users. SaaS users subscribe to an application rather than purchasing it once and installing it. Users can log into and use a SaaS application from any compatible device over the Internet. The actual application runs in cloud servers that may be far removed from a user's location.

======
A SaaS application may be accessed through a browser or through an app. Online email applications that users access through a browser, such as Gmail and Office 365, are common examples of SaaS applications.

=============================
Platform-as-a-Service (PaaS) 
==============================
Developers essentially rent everything they need to build an application, relying on a cloud provider for development tools, infrastructure, and operating systems. This is one of the three service models of cloud computing. PaaS vastly simplifies web application development; from the developer's perspective, all backend management takes place behind the scenes. Although PaaS has some similarities with serverless computing, there are many critical differences between them.

The main offerings included by PaaS vendors are:
1) Development tools: source code editor, a debugger, a compiler, and other essential tools
2) Middleware: Middleware is software that sits in between user-facing applications and the machine's operating system; for example, middleware is what allows software to access input from the keyboard and mouse.
3) Operating systems: 
4) Database management
5) Infrastructure
Different vendors may include other services as well, but these are the core PaaS services.

=======
PaaS is used to build applications more quickly than would be possible if developers had to worry about building, configuring, and provisioning their own platforms and backend infrastructure. With PaaS, all they need to do is write the code and test the application, and the vendor handles the rest. 

PaaS permits developers to build, test, debug, deploy, host, and update their applications all in the same environment. This enables developers to be sure a web application will function properly as hosted before they release, and it simplifies the application development lifecycle.

============
Multi-cloud
============
Multi-cloud means several different public clouds are used to support one or more applications, instead of just a single public cloud. Instead of a business using one vendor for cloud hosting, storage, and the full application stack, in a multi-cloud configuration they use several. Multi-cloud deployments have a number of uses. A multi-cloud deployment can leverage multiple IaaS (infrastructure-as-a-service) vendors, or it could use a different vendor for IaaS, PaaS (platform-as-a-service), and SaaS (software-as-a-service) services. Multi-cloud can be purely for the purpose of redundancy and system backup, or it can incorporate different cloud vendors for different services.

=======
What is the difference between multi-cloud and hybrid cloud?
A multi-cloud can also be a hybrid cloud, and a hybrid cloud can also be a multi-cloud, but these terms represent two distinct concepts. "Hybrid cloud" describes the mixing of two or more distinct types of infrastructure: it combines a private cloud, an on-premise data center, or both with at least one public cloud. Multi-cloud refers to several different public clouds being deployed, and it doesn't necessarily include a private cloud, although it can.

==========
Shadow IT
==========
A multi-cloud deployment can come about unintentionally, as a result of shadow IT. Shadow IT is when internal teams set up technical systems or use software products without official approval or oversight from the larger organization. A simple example would be if a company's employees use a chat app that is not sanctioned or managed by the company to communicate about business activities.

Shadow IT can find its way into application architecture too. Either as a short cut for getting things done, or out of necessity, employees may incorporate cloud services into a company's technology stack before receiving official approval.

=============
Hybrid cloud 
=============
A hybrid cloud mixes two or more types of cloud environments. Hybrid cloud deployments combine public* and private clouds**, and they may also include on-premise legacy infrastructure. For a cloud to truly be hybrid, these different cloud environments must be tightly interconnected with each other, essentially functioning as one combined infrastructure. Almost all hybrid clouds include at least one public cloud. Hybrid clouds have a number of uses. An organization may use their private cloud for some services and their public cloud for others, or they may use the public cloud as backup for their private cloud. They can also use the public cloud to handle periods of high demand, while keeping most operations within their private cloud.

===========
Containers
===========
A container 'contains' both an application and all the elements the application needs to run properly, including system libraries, system settings, and other dependencies. Like a 'just add water' pancake mix, containers only need one thing – to be hosted and run – in order to perform their function.

Any kind of application can be run in a container. A containerized application will run the same way no matter where it is hosted. Containers can easily be moved around and deployed wherever needed, much like physical shipping containers, which are a standard size and can therefore be shipped anywhere via a variety of means of transport (ships, trucks, trains, etc.) regardless of their contents.

======
In technical terms, containers are a way of partitioning a machine, or server, into separate user space environments such that each environment runs only one application and doesn’t interact with any other partitioned sections on the machine. Each container shares the machine's kernel with other containers (the kernel is the foundation of the operating system, and it interacts with the computer's hardware), but it runs as if it were the only system on the machine. 'Serverless' computing actually runs on servers, but it is up to the serverless vendor to provision server space as it is needed by the application; no specific machines are assigned for a given function or application. On the other hand, each container lives on one machine at a time and uses the operating system of that machine, though they can be moved easily to a different machine if desired. In a container-based architecture, the number of containers deployed is determined by the developer in advance. In contrast, in a serverless architecture, the backend inherently and automatically scales to meet demand.

====
CDN
====
CDN delivers fast, efficient, and secure delivery of content to websites and Internet services. A content delivery network (CDN) is a geographically distributed group of servers that caches content close to end users. A CDN allows for the quick transfer of assets needed for loading Internet content, including HTML pages, JavaScript files, stylesheets, images, and videos. The popularity of CDN services continues to grow, and today the majority of web traffic is served through CDNs, including traffic from major sites like Facebook, Netflix, and Amazon.
A properly configured CDN may also help protect websites against some common malicious attacks, such as Distributed Denial of Service (DDOS) attacks.

=======
Is a CDN the same as a web host?
While a CDN does not host content and can’t replace the need for proper web hosting, it does help cache content at the network edge, which improves website performance. Many websites struggle to have their performance needs met by traditional hosting services, which is why they opt for CDNs. By utilizing caching to reduce hosting bandwidth, helping to prevent interruptions in service, and improving security, CDNs are a popular choice to relieve some of the major pain points that come with traditional web hosting.

======
What are the benefits of using a CDN?
Although the benefits of using a CDN vary depending on the size and needs of an Internet property, the primary benefits for most users can be broken down into four different components:
1) Improving website load times - By distributing content closer to website visitors by using a nearby CDN server (among other optimizations), visitors experience faster page loading times. As visitors are more inclined to click away from a slow-loading site, a CDN can reduce bounce rates and increase the amount of time that people spend on the site. In other words, a faster a website means more visitors will stay and stick around longer.
2) Reducing bandwidth costs - Bandwidth consumption costs for website hosting is a primary expense for websites. Through caching and other optimizations, CDNs are able to reduce the amount of data an origin server must provide, thus reducing hosting costs for website owners.
3) Increasing content availability and redundancy - Large amounts of traffic or hardware failures can interrupt normal website function. Thanks to their distributed nature, a CDN can handle more traffic and withstand hardware failure better than many origin servers.
4) Improving website security - A CDN may improve security by providing DDoS mitigation, improvements to security certificates, and other optimizations.

======
How does a CDN work?
At its core, a CDN is a network of servers linked together with the goal of delivering content as quickly, cheaply, reliably, and securely as possible. In order to improve speed and connectivity, a CDN will place servers at the exchange points between different networks. These Internet exchange points (IXPs) are the primary locations where different Internet providers connect in order to provide each other access to traffic originating on their different networks. By having a connection to these high speed and highly interconnected locations, a CDN provider is able to reduce costs and transit times in high speed data delivery.

=========
DynamoDB
=========
DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:
1) reliable performance even as it scales;
) a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
3) a small, simple API allowing for simple key-value access as well as more advanced query patterns.

DynamoDB is a particularly good fit for the following use cases:
1) Applications with large amounts of data and strict latency requirements. As your amount of data scales, JOINs and advanced SQL operations can slow down your queries. With DynamoDB, your queries have predictable latency up to any size, including over 100 TBs!
2) Serverless applications using AWS Lambda. AWS Lambda provides auto-scaling, stateless, ephemeral compute in response to event triggers. DynamoDB is accessible via an HTTP API and performs authentication & authorization via IAM roles, making it a perfect fit for building Serverless applications.
3) Data sets with simple, known access patterns. If you're generating recommendations and serving them to users, DynamoDB's simple key-value access patterns make it a fast, reliable choice.

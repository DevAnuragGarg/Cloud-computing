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


=============
Cloud-native
=============
Cloud-native is born in the cloud. Cloud-native applications are architected from the ground up to run in a public cloud like in AWS, Azure, or GCP using cloud-based technologies. These cloud technologies allow for accessibility and scalability and allow developers to continue to deliver new services more quickly and easily. Cloud-native is comprised of continuous integration, orchestrators, and container engines. Ultimately, it’s about how applications are created and deployed. Cloud-native is a new way of architecting our applications and infrastructure; we’re breaking services into smaller and smaller pieces and reusing services wherever possible. We’re deploying our apps and infrastructure in someone else’s data center, so we have to always be thinking about failure. Having this mindset allows us to deploy new, flexible, resilient, cloud-native applications.

======
Cloud-native applications are software programs that consist of multiple small, interdependent services called microservices. Traditionally, developers built monolithic applications with a single block structure containing all the required functionalities. By using the cloud-native approach, software developers break the functionalities into smaller microservices. This makes cloud-native applications more agile as these microservices work independently and take minimal computing resources to run. 

============
Cloud-based
============
Cloud-based is the middle ground between cloud-native and cloud-enabled. If you want to leverage some of the capabilities of the cloud such as higher availability and scalability, but don’t want to completely redesign your application to use cloud services, this may be an approach to consider. For example, if you move your in-house web application to AWS or Azure servers, you now have a “cloud-based” application. Once you move your application to a cloud provider, you’re no longer responsible for managing the resources for the application, so there’s no need to maintain a server or worry about backup. You also just pay for what you use. The biggest advantage of moving an application to the cloud is enabling it to quickly scale up to meet surges in demand and increase your application availability.

==============
Cloud-enabled
==============
Cloud-enabled usually refers to applications built traditionally and then migrated to the cloud. These applications were originally designed in a monolithic fashion and depend on local resources and hardware. In the migration of the application to the cloud, the application is refactored to use virtual resources, but the underlying architecture remains the same. The application cannot take advantage of shared services or resource pools and as a result struggles to deliver the scalability and resiliency of other cloud applications. Cloud enabled can be an approach for legacy applications or as the first step towards cloud adoption.

======
Cloud-enabled applications are legacy enterprise applications that were running on an on-premises data center but have been modified to run on the cloud. This involves changing part of the software module to migrate the application to cloud servers. You can thus use the application from a browser while retaining its original features.

============================
Cloud-agnostic architecture
============================
Cloud agnostic refers to a cloud design strategy in which applications, tools, and services are designed to migrate seamlessly between multiple cloud platforms or between on-premises and cloud in a hybrid model without disruption of service. Some of the tenets of a cloud-agnostic approach are to support seamless portability independent of the underlying operating system, to ensure limited disruption of the workloads in migration, and to limit the risk of application downtime while enhancing cost efficiencies.

======
As an example, a common cloud-agnostic strategy involves designing tools, services, or applications to run on two or more cloud platforms. Some of the common public cloud platforms companies leverage to implement a cloud-agnostic strategy include AWS, Azure, and Google Cloud Platform.

======
Benefits:
1) Portability ensures that an application works independently of the platform and can seamlessly migrate from one cloud platform to another.
2) Consistent performance is a valuable characteristic of cloud agnostic, as companies benefit from a standard of performance (speed and scale) independent of the platform or infrastructure the application or service is running on.
3) Cost optimization is a primary tenet of a cloud-agnostic architecture. As pricing models change between cloud providers, cloud-agnostic applications can be migrated easily to run in the cloud platform that delivers the best cost savings.
4) Avoiding vendor lock-in ensures that companies are not subject to one operating platform, but have the freedom to move applications as they see fit.

======
A cloud-agnostic architecture aims to design applications that can run seamlessly across any cloud provider. Unlike cloud-native applications, cloud-agnostic services are not dependent on a single cloud platform’s toolkit. Instead, they integrate with a mix of open-source and vendor-provided tools.

=======
Difference from Cloud Native

Portability: 
Cloud native: Difficult to move applications ported to different cloud providers.	
Cloud agnostic: Applications can be moved anywhere and never locked into a specific provider.

Performance:
Cloud native: Components work on a small segment, increasing performance overall.	
Cloud agnostic: Wide range of features and options that customers can use to maximize performance.

Flexibility:
Cloud native: Applications benefit from a cloud platform's built-in provisions for networking, monitoring, and other underlying architecture concerns that stymie large development efforts.	
Cloud agnostic: Developers are not restricted to one cloud platform's capabilities or tools and can incorporate open-source tools, libraries, and integrations.

Costs:
Cloud native: Customers are charged based on a combination of licensing and data storage requirements, following a pay-as-you-go model.
Cloud agnostic: Cloud-agnostic architecture has greater accessibility to open-source tools, providing more direct control over costs and the ability to make spending adjustments as needed.

Scalability:
Cloud native: Cloud-native systems are easy to scale up or down to meet business needs.
Cloud agnostic: Cloud-agnostic apps and services can move across cloud platforms, which means they can quickly scale up to meet demand.

===========
Redundancy
===========
Redundancy is the practice of deploying system component copies (hardware and software). These copies are not necessary for the services’ ordinary operation but are crucial for guaranteeing its availability, detecting faults, and mitigating them.

=====================================
Fault tolerance vs High availability
=====================================
Both High Availability and Fault Tolerance have the same objective of ensuring that your application runs all the time without any system degradation. These two differ in cost, design, redundancy level, and behavior on component faults or failures.

High Availability aims for your application to run 99.999% of the time. Its design ensures that the entire system can quickly recover if one of its components crashed. It has an ample number of redundant resources to allow failover to another resource if the other one fails. This concept accepts that a failure will occur but provides a way for the system to recover fast. High availability specifies a design that aims to minimize the downtime of a system or service. So, the main objective of high availability is to keep these systems and services continuously available.

======
Fault tolerance relies on specialized hardware to detect a hardware fault and instantaneously switch to a redundant hardware component—whether the failed component is a processor, memory board, power supply, I/O subsystem, or storage subsystem. Although this cutover is apparently seamless and offers non-stop service, a high premium is paid in both hardware cost and performance because the redundant components do no processing. More importantly, the fault tolerant model does not address software failures, by far the most common reason for downtime.

======
Fault Tolerance, on the other hand, has the goal of keeping your application running with zero downtime. It has a more complex design, and higher redundancy to sustain any fault in one of its components. Think of it as an upgraded version of High Availability. As its name implies, it can tolerate any component fault to avoid any performance impact, data loss, or system crashes by having redundant resources beyond what is typically needed. The caveat for implementing a fault-tolerant system is its cost as companies have to shoulder the capital and operating expenses for running its required numerous resources.

======
A system can be highly available but not fault-tolerant, and it can be both. If an application is said to be fault-tolerant then it is also considered highly available. However, there are situations in which a highly available application is not considered fault-tolerant. 

======
The difference between fault tolerance and high availability, is this: A fault tolerant environment has no service interruption but a significantly higher cost, while a highly available environment has a minimal service interruption.

========================
Three-tier architecture 
========================
is a well-established software application architecture that organizes applications into three logical and physical computing tiers: the presentation tier, or user interface; the application tier, where data is processed; and the data tier, where the data associated with the application is stored and managed.
The chief benefit of three-tier architecture is that because each tier runs on its own infrastructure, each tier can be developed simultaneously by a separate development team, and can be updated or scaled as needed without impacting the other tiers.

For decades three-tier architecture was the prevailing architecture for client-server applications. Today, most three-tier applications are targets for modernization, using cloud-native technologies such as containers and microservices, and for migration to the cloud. The most common type of multi-tier architecture in distributed systems is a three-tier client-server architecture.

======
Presentation tier: The presentation tier is the user interface and communication layer of the application, where the end user interacts with the application. Its main purpose is to display information to and collect information from the user. This top-level tier can run on a web browser, as desktop application, or a graphical user interface (GUI), for example. Web presentation tiers are usually developed using HTML, CSS and JavaScript. Desktop applications can be written in a variety of languages depending on the platform.

======
Application tier: also known as the logic tier or middle tier, is the heart of the application. In this tier, information collected in the presentation tier is processed - sometimes against other information in the data tier - using business logic, a specific set of business rules. The application tier can also add, delete or modify data in the data tier. The application tier is typically developed using Python, Java, Perl, PHP or Ruby, and communicates with the data tier using API calls. 

======
Data tier: sometimes called database tier, data access tier or back-end, is where the information processed by the application is stored and managed. This can be a relational database management system such as PostgreSQL, MySQL, MariaDB, Oracle, DB2, Informix or Microsoft SQL Server, or in a NoSQL Database server such as Cassandra, CouchDB or MongoDB.  In a three-tier application, all communication goes through the application tier. The presentation tier and the data tier cannot communicate directly with one another.

======
In web development, the tiers have different names but perform similar functions:

1) The web server is the presentation tier and provides the user interface. This is usually a web page or web site, such as an ecommerce site where the user adds products to the shopping cart, adds payment details or creates an account. The content can be static or dynamic, and is usually developed using HTML, CSS and Javascript.

2) The application server corresponds to the middle tier, housing the business logic used to process user inputs. To continue the ecommerce example, this is the tier that queries the inventory database to return product availability, or adds details to a customer's profile. This layer often developed using Python, Ruby or PHP and runs a framework such as e Django, Rails, Symphony or ASP.NET, for example.

3) The database server is the data or backend tier of a web application. It runs on database management software, such as MySQL, Oracle, DB2 or PostgreSQL, for example.

====================
N-tier architecture
====================
also called or multi-tier architecture - refers to any application architecture with more than one tier. But applications with more than three layers are rare, because additional layers offer few benefits and can make the application slower, harder to manage and more expensive to run. As a result, n-tier architecture and multi-tier architecture are usually synonyms for three-tier architectur

===================
Distributed system
===================
A distributed system contains multiple nodes that are physically separate but linked together using the network. All the nodes in this system communicate with each other and handle processes in tandem. Each of these nodes contains a small part of the distributed operating system software.

Types of Distributed Systems: The nodes in the distributed systems can be arranged in the form of client/server systems or peer to peer systems. Details about these are as follows −

======
Client/Server Systems: In client server systems, the client requests a resource and the server provides that resource. A server may serve multiple clients at the same time while a client is in contact with only one server. Both the client and server usually communicate via a computer network and so they are a part of distributed systems.

Peer to Peer Systems: The peer to peer systems contains nodes that are equal participants in data sharing. All the tasks are equally divided between all the nodes. The nodes interact with each other as required as share resources. This is done with the help of a network.

===========
Web Server
===========
A Web Server is defined as a server which accepts a request for data and sends the relevant document in return. In other words, it is a computer program that accepts a request for a specific document and sends it to the client machine. Web servers are designed to serve HTTP content to the client computer. In most cases, the web servers are the integral parts of the application servers. Web servers accept the HTTP requests and interpret them to serve the requested content. Although Web Servers are designed to serve static content, most Web Servers have plugins to support scripting languages like PHP, Perl, etc. through which they can generate dynamic HTTP content. Web server is useful or fitted for static content.
Example of Web Servers: Apache Tomcat, Resin

===================
Application server
===================
An application server is one that is designed to generate dynamic content. It is a software framework that transforms the data to provide specialized functionalities offered by a business, service, or application. Application servers enhance the interactive parts of a website depending on the context of the request. Application servers contain web containers and EJB(Enterprise Java Beans) containers. Application servers are entirely responsible for creating an environment for enterprise applications. These servers are capable of supporting HTTP as well as RPC/PMI protocols. Application servers consume more resources like CPU, memory as compared to web servers. Most Application Servers have a Web Server as an integral part, which means an Application Server can perform all the tasks that a Web Server does. Whereas application server is fitted for dynamic content.
Examples of Application Server: Weblogic, JBoss, Websphere

===================
Horizontal scaling
===================
Horizontal scaling (aka scaling out) refers to adding additional nodes or machines to your infrastructure to cope with new demands. If you are hosting an application on a server and find that it no longer has the capacity or capabilities to handle traffic, adding a server may be your solution. Distributes multiple jobs across multiple machines over the network, at a go. This reduces the workload on each machine.

=================
Vertical scaling
=================
Vertical scaling (aka scaling up) describes adding additional resources to a system so that it meets demand. How is this different from horizontal scaling? While horizontal scaling refers to adding additional nodes, vertical scaling describes adding more power to your current machines. For instance, if your server requires more processing power, vertical scaling would mean upgrading the CPUs. You can also vertically scale the memory, storage, or network speed. Relies on multi-threading on the existing machine to handle multiple requests at the same time.

==============================================
File storage, block storage or object storage
==============================================
Files, blocks, and objects are storage formats that hold, organize, and present data in different ways—each with their own capabilities and limitations. File storage organizes and represents data as a hierarchy of files in folders; block storage chunks data into arbitrarily organized, evenly sized volumes; and object storage manages data and links it to associated metadata.

File storage, also called file-level or file-based storage, is exactly what you think it might be: Data is stored as a single piece of information inside a folder, just like you’d organize pieces of paper inside a manila folder. When you need to access that piece of data, your computer needs to know the path to find it. (Beware—It can be a long, winding path.) Data stored in files is organized and retrieved using a limited amount of metadata that tells the computer exactly where the file itself is kept. It’s like a library card catalog for data files.

======
Think of a closet full of file cabinets. Every document is arranged in some type of logical hierarchy—by cabinet, by drawer, by folder, then by piece of paper. This is where the term hierarchical storage comes from, and this is file storage. It is the oldest and most widely used data storage system for direct and network-attached storage systems, and it’s one that you’ve probably been using for decades. Any time you access documents saved in files on your personal computer, you use file storage. File storage has broad capabilities and can store just about anything. It’s great for storing an array of complex files and is fairly fast for users to navigate.

======
The problem is, just like with your filing cabinet, that virtual drawer can only open so far. File-based storage systems must scale out by adding more systems, rather than scale up by adding more capacity.

======
Block storage chops data into blocks—get it?—and stores them as separate pieces. Each block of data is given a unique identifier, which allows a storage system to place the smaller pieces of data wherever is most convenient. That means that some data can be stored in a Linux® environment and some can be stored in a Windows unit.

======
Block storage is often configured to decouple the data from the user’s environment and spread it across multiple environments that can better serve the data. And then, when data is requested, the underlying storage software reassembles the blocks of data from these environments and presents them back to the user. It is usually deployed in storage-area network (SAN) environments and must be tied to a functioning server.

======
Because block storage doesn’t rely on a single path to data—like file storage does—it can be retrieved quickly. Each block lives on its own and can be partitioned so it can be accessed in a different operating system, which gives the user complete freedom to configure their data. It’s an efficient and reliable way to store data and is easy to use and manage. It works well with enterprises performing big transactions and those that deploy huge databases, meaning the more data you need to store, the better off you’ll be with block storage.

There are some downsides, though. Block storage can be expensive. It has limited capability to handle metadata, which means it needs to be dealt with in the application or database level—adding another thing for a developer or systems administrator to worry about.

======
Object storage, also known as object-based storage, is a flat structure in which files are broken into pieces and spread out among hardware. In object storage, the data is broken into discrete units called objects and is kept in a single repository, instead of being kept as files in folders or as blocks on servers.

======
Object storage volumes work as modular units: each is a self-contained repository that owns the data, a unique identifier that allows the object to be found over a distributed system, and the metadata that describes the data. That metadata is important and includes details like age, privacies/securities, and access contingencies. Object storage metadata can also be extremely detailed, and is capable of storing information on where a video was shot, what camera was used, and what actors are featured in each frame. To retrieve the data, the storage operating system uses the metadata and identifiers, which distributes the load better and lets administrators apply policies that perform more robust searches.

======
Object storage requires a simple HTTP application programming interface (API), which is used by most clients in all languages. Object storage is cost efficient: you only pay for what you use. It can scale easily, making it a great choice for public cloud storage. It’s a storage system well suited for static data, and its agility and flat nature means it can scale to extremely large quantiti	es of data. The objects have enough information for an application to find the data quickly and are good at storing unstructured data.

======
There are drawbacks, to be sure. Objects can’t be modified—you have to write the object completely at once. Object storage also doesn’t work well with traditional databases, because writing objects is a slow process and writing an app to use an object storage API isn’t as simple as using file storage.

====
DNS
====
The Domain Name System (DNS) is the phonebook of the Internet. Humans access information online through domain names, like nytimes.com or espn.com. Web browsers interact through Internet Protocol (IP) addresses. DNS translates domain names to IP addresses so browsers can load Internet resources.

Each device connected to the Internet has a unique IP address which other machines use to find the device. DNS servers eliminate the need for humans to memorize IP addresses such as 192.168.1.1 (in IPv4), or more complex newer alphanumeric IP addresses such as 2400:cb00:2048:1::c629:d7a2 (in IPv6).


=========================
Multi-Region Application
=========================
AWS Regions are built with multiple isolated and physically separate Availability Zones (AZs). This approach allows you to create highly available Well-Architected workloads that span AZs to achieve greater fault tolerance. This satisfies the availability goals for most applications, but there are some general reasons that you may be thinking about expanding beyond a single Region:

Expansion to a global audience as an application grows and its user base becomes more geographically dispersed, there can be a need to reduce latencies for different parts of the world.
Reducing Recovery Point Objectives (RPO) and Recovery Time Objectives (RTO) as part of a multi-Region disaster recovery (DR) plan.
Local laws and regulations may have strict data residency and privacy requirements that must be followed.

========= 
Security: Creating a security foundation starts with setting proper authentication and authorization rules. The system handling these requests must be highly resilient to verify and authorize requests quickly and reliably. AWS Identity and Access Management (IAM) accomplishes this by creating a reliable mechanism for you to manage access to AWS services and resources. IAM has multi-Region availability automatically, with no configuration required on your part.

Applications that need to securely store, rotate, and audit secrets, such as database passwords, should use AWS Secrets Manager. This service encrypts secrets with AWS Key Management Service (AWS KMS) keys and can replicate secrets to secondary Regions to ensure applications are able to quickly retrieve a secret in the closest Region.

Encryption accross region: AWS KMS can be used to encrypt data at rest, and is used extensively for encryption across AWS services. By default, keys are confined to a single Region. AWS services such as Amazon Simple Storage Service (Amazon S3) cross-Region replication and Amazon Aurora Global Database (both covered in part 2), simplify the process of encryption and decryption with different keys in each Region. For other parts of your multi-Region application that rely on KMS keys, you can set up AWS KMS multi-Region keys to replicate the key material and key ID to a second Region. This eliminates the need to decrypt and re-encrypt data with a different key in each Region. For example, multi-Region keys can be used to reduce the complexity of a multi-Region application’s encryption operations for data that is stored across Regions.

Auditing and observability across Regions
It is a best practice to configure AWS CloudTrail to keep a record of all relevant AWS API activity in your account for auditing purposes. When you utilize multiple Regions or accounts, these CloudTrail logs should be aggregated into a single Amazon S3 bucket for easier analysis. To prevent misuse, the centralized logs should be treated with higher severity, with only limited access to key systems and personnel.

Subnet
When a bigger network is divided into smaller networks, to maintain security, then that is known as Subnetting. So, maintenance is easier for smaller networks. For example, if we consider a class A address, the possible number of hosts is 224 for each network, it is obvious that it is difficult to maintain such a huge number of hosts, but it would be quite easier to maintain if we divide the network into small parts. 

VPC: You can launch AWS resources into a defined virtual network using Amazon Virtual Private Cloud (Amazon VPC). With the advantages of utilizing the scalable infrastructure of AWS, this virtual network closely mimics a conventional network that you would operate in your own data center. /16 user-defined address space maximum (65,536 addresses)
Subnetes: To reduce traffic, the subnet will divide the big network into smaller, connected networks. Up to /16, 200 user-defined subnets.
Route Tables: Route Tables are mainly used to Define the protocol for traffic routing between the subnets.
Network Access Control Lists: Network Access Control Lists (NACL) for VPC serve as a firewall by managing both inbound and outbound rules. There will be a default NACL for each VPC that cannot be deleted.
Internet Gateway(IGW): The Internet Gateway (IGW) will make it possible to link the resources in the VPC to the Internet.
Network Address Translation (NAT):  Network Address Translation (NAT) will enable the connection between the private subnet and the internet.

DynamoDB allows users to create databases capable of storing and retrieving any amount of data and comes in handy while serving any amount of traffic. It dynamically manages each customer’s requests and provides high performance by automatically distributing data and traffic over servers. It is a fully managed NoSQL database service that is fast, predictable in terms of performance, and seamlessly scalable. It relieves the user from the administrative burdens of operating and scaling a distributed database as the user doesn’t have to worry about hardware provisioning, patching Softwares, or cluster scaling. It also eliminates the operational burden and complexity involved in protecting sensitive data by providing encryption at REST.

Amazon VPC is made up of various networking components. Here is the list of a few key components of Amazon VPC:

Subnets
Elastic network interfaces
Route tables
Internet gateways
Elastic IP addresses
VPC endpoints
NAT
VPC peering
Many different services, such as Gateway, Load Balancer, Subnets, and so on, make up the core architecture of a well-operating VPC. To build an isolated virtual environment, these resources are grouped under a VPC. Along with these services, there are numerous degrees of security checks.	

An Amazon EC2 instance is based on an Amazon Machine Image (AMI). An AMI specifies instance configurations such as the instance’s storage, launch permissions, and device mappings. When a new standard image needs to be created and released, EC2 Image Builder simplifies the building, testing, and deployment of new AMIs. It can also help with copying of AMIs to additional Regions to eliminate needing to manually copy source AMIs to target Regions.
Although Amazon Elastic Compute Cloud (Amazon EC2) instances and their associated Amazon Elastic Block Store (Amazon EBS) volumes reside in a single AZ, Amazon Data Lifecycle Manager can automate the process of taking and copying EBS snapshots across Regions. This can enhance DR strategies by providing an easy cold backup-and-restore option for EBS volumes. If you need to back up more than just EBS volumes, AWS Backup provides a central place to do this across multiple services

Microservice-based applications that use containers benefit from quicker start-up times. Amazon Elastic Container Registry (Amazon ECR) can help ensure this happens consistently across Regions with private image replication at the registry level. An ECR private registry can be configured for either cross-Region or cross-account replication to ensure your images are ready in secondary Regions when needed.


AWS Storage Services: AWS offers a wide range of storage services that can be provisioned depending on your project requirements and use case. AWS storage services have different provisions for highly confidential data, frequently accessed data, and the not so frequently accessed data. You can choose from various storage types namely, object storage, file storage, block storage services, backups,, and data migration options. All of which fall under the AWS Storage Services list.

Elastic Block Storage (EBS): From the aforementioned list, EBS is a block type durable and persistent storage that can be attached to EC2-instances for additional storage. Unlike EC-2 instance storage volumes which are suitable for holding temporary data EBS volumes are highly suitable for essential and long term data. EBS volumes are specific to availability zones and can only be attached to instances within the same availability zone. 
EBS can be created from the EC2 dashboard in the console as well as in Step 4 of the EC2 launch. Just note that when creating EBS with EC2, the EBS volumes are created in the same availability zone as EC2, however when provisioned independently users can choose the AZ in which EBS is required.

Features of EBS:
Scalability: EBS volume sizes and features can be scaled as per the needs of the system. This can be done in two ways:
Take a snapshot of the volume and create a new volume using the Snapshot with new updated features.
Updating the existing EBS volume from the console.
Backup: Users can create snapshots of EBS volumes that act as backups.
Snapshot can be created manually at any point in time or can be scheduled.
Snapshots are stored on AWS S3 and are charged according to the S3 storage charges.
Snapshots are incremental in nature.
New volumes across regions can be created from snapshots.
Encryption: Encryption can be a basic requirement when it comes to storage. This can be due to the government of regulatory compliance. EBS offers an AWS managed encryption feature.
Users can enable encryption when creating EBS volumes bu clicking on a checkbox.
Encryption Keys are managed by the Key Management Service (KMS) provided by AWS.
Encrypted volumes can only be attached to selected instance types.
Encryption uses the AES-256 algorithm.
Snapshots from encrypted volumes are encrypted and similarly, volumes created from snapshots are encrypted.
Charges: Unlike AWS S3, where you are charged for the storage you consume, AWS charges users for the storage you hold. For example if you use 1 GB storage in a 5 GB volume, you’d still be charged for a 5 GB EBS volume.
EBS charges vary from region to region.
EBS Volumes are independent of the EC@ they are attached to. The data in an EBS volume will remain unchanged even if the instance is rebooted or terminated.
Single EBS volume can only be attached to one EC2 instance at a time. However, one EC2 can have more than one EBS volumes attached to it.


EBS volumes are specific to availability zones and can only be attached to EC2 in the same availability zone. In case AWS’ availability zone is to go down, access to the EBS volume will be lost.
Can be used for rapidly changing data that needs good I/Ops.
As compared to EC-2 instance storage the control over data and flexibility offered by EBS is far greater.
To provide durability, EBS volumes are replicated in their availability zone but are limited to one availability zone.


EBS can be used to store data for database applications in a number of ways. Some examples include:

As a root volume for a database instance: An EBS volume can be used as the root volume for an Amazon EC2 instance running a database application, such as MySQL or PostgreSQL. This allows the database application to store its data on a persistent and highly available storage volume, rather than relying on the ephemeral storage of the EC2 instance.
As a storage volume for a managed database service: AWS offers several managed database services, such as Amazon RDS and Amazon Aurora, that allow users to easily set up and manage a database without having to worry about the underlying infrastructure. These services allow users to create EBS volumes as the storage for their database, providing persistent and scalable storage for the database data.
As a storage volume for containerized databases: EBS can also be used as the storage for containerized database applications, such as those deployed using Amazon ECS or Amazon EKS. This allows users to store their database data on a persistent and highly available storage volume, while still taking advantage of the benefits of running their database in a containerized environment.
Drawbacks:

EBS is not recommended as temporary storage.
They cannot be used as a multi-instance accessed storage as they cannot be shared between instances.
The durability offered by services like AWS S3 and AWS EFS is greater.


Data replication across the AWS network happens quickly, but keep in mind that a networking packet’s travel time will increase as the physical distance the packet needs to travel increases. For this reason, data consistency must be considered against performance when building multi-Region applications.

When building a distributed system, the consistency, availability, and partition tolerance (CAP) theorem must be considered. This theorem states that an application can only pick 2 out of the 3, and tradeoffs should be considered when making this decision.

Consistency – all clients always have the same view of the data
Availability – all clients can always read and write the data
Partition Tolerance – the system will continue to work despite physical partitions
CAP diagram

Achieving consistency and availability (CA) is common for single-Region architectures. For example, when an application connects to a single in-Region relational database. However, this becomes more difficult with multi-Region applications due to the latency added by transferring data over long distances. For this reason, highly distributed systems typically compromise on strict consistency, favoring availability and partition tolerance (AP). This is commonly referred to as an eventual consistency data model.

The scale, durability, and availability of Amazon Simple Storage Service (Amazon S3) make it an excellent destination to store various assets for your application. To enable quick access of this data to your application regardless of the Region it’s deployed in, you can set up Amazon S3 to replicate data across AWS Regions with one-way or two-way continuous replication. If your application doesn’t require all of the objects in a bucket for optimal functionality, a subset of objects can be replicated with Amazon S3 replication rules. Amazon S3 within a Region offers strong read-after-write consistency; however, replicated objects will be eventually consistent in destination Regions. If maintaining low replication lag is critical, S3 Replication Time Control will replicate 99.99% of objects within 15 minutes, and most within seconds. Observability is critical at all layers of an application, and you can watch over the replication status of objects with Amazon S3 events and metrics.

To simplify connecting to and managing multiple bucket endpoints, Amazon S3 Multi-Region Access Points create a single global endpoint that spans multiple S3 buckets in different Regions. When applications connect to this endpoint, requests will route over the AWS network using AWS Global Accelerator to the bucket with the lowest latency. Failover routing is also handled automatically if the availability of a bucket changes.



How Does EFS Work?
EFS can be created using the EC2-Instance where it will be created in a specific region and distributed across multiple availability zones for the purpose of high availability and durability. You can choose the EFS based on the I/Ops you are going to perform.


Use Cases Of EFS
Secured file sharing: You can share your files in every secured manner and in a faster and easier way and also ensures consistency across the system.
Web Hosting: Well suited for web servers where multiple web servers can access the file system and can store the data EFS also scales whenever the data incoming is increased.
Modernize application development: You can share the data from the AWS resources like ECS, EKS, and any serverless web applications in an efficient manner and without more management required.
Machine Learning and AI Workloads: EFS is well suited for large data AI applications where multiple instances and containers will access the same data improving collaboration and reducing data duplication.
Above are some of the use cases of AWS EFS widely used for handling larger datasets type applications.



Amazon DynamoDB global tables provide multi-Region and multi-writer capabilities to help you build global applications at scale. A DynamoDB global table is the only AWS managed database offering that allows for multiple active writers with conflict detection in a multi-Region topology (active-active and multi-Region). This allows for applications to read and write in the Region closest to them, with changes automatically replicated to other Regions.



Keeping in-memory caches warm with the same data across Regions can be critical to maintain application performance. Amazon ElastiCache for Redis offers global datastore to create a fully managed, fast, reliable, and secure cross-Region replica for Redis caches and databases. With global datastore, writes occurring in one Region can be read from up to two other cross-Region replica clusters – eliminating the need to write to multiple caches to keep them warm.




For applications that require a relational data model, Amazon Aurora global database provides for scaling of database reads across Regions in Aurora PostgreSQL-compatible and MySQL-compatible editions. Dedicated replication infrastructure utilizes physical storage-based replication to achieve consistently low replication lag that outperforms the built-in logical replication database engines offer, as shown in Figure 2.


With Aurora global database, a cluster in one Region is designated as the writer, and secondary Regions are dedicated to reads. While only one instance can process writes, Aurora MySQL supports write forwarding, a feature that will forward write queries from a secondary Region endpoint to the primary Region to simplify logic in application code.



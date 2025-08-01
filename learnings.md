1. The client-server model: The client makes a request to the server, and the server processes the request and sends back the response.
2. Cloud Computing -> On-demand delivery of IT resources over the internet with pay-as-you-go pricing.
3. Cloud deployment types:
     1. Cloud based deployment -> Flexibility to migrate your existing resources to the cloud, design and build new applications within the cloud environment, or use a combination of both.
     2. On-premises deployment -> Deploying resources on premises using virtualization and resource management tools. This has the ability to provide dedicated resources and low latency.
     3. Hybrid deployment -> Cloud-based resources and on-premises infrastructure work together.
4. Key benifits of AWS Cloud:
   1. Businesses can transition from fixed investments to variable costs.
   2. The vast global infrastructure of AWS can result in lower costs for customers.
   3. Customers can dynamically scale AWS Cloud resources up or down based on real-time demand.
   4. Businesses can rapidly deploy applications and services.
   5. Stop spending money to run and maintain data centers.
   6. Businesses don't need to set up their own infrastructure to expand internationally.
5. AWS Regions are physical locations around the world that contain groups of data centers.
6. These groups of data centers are called Availability Zones.
7. Each AWS Region consists of a minimum of three physically separate Availability Zones within a geographic area.
8. Regions and Availability Zones are designed to provide low-latency, fault-tolerant access to services for users within a given area.


## Amazon EC2
1. Amazon Elastic Compute Cloud.
2. Advantages: Highly Flexible, Cost-effective, and Quick.
3. EC2 instances are virtual machines, or VMs.
4. Multi-tenancy allows multiple virtual machines to share resources on the same physical host, with isolation between them.
5. With Amazon EC2, only pay for running instances, not for ones that are stopped or terminated.
6. Choose EC2 instance type (how powerful you want it) and the Amazon Machine Image (AMI), which determines the operating system and software for your instance.

## Amazon EC2 instance types
1. These instances come with varying combinations of CPU, memory, storage, and networking capabilities, so we can choose the right mix of resources to optimize performance for the applications.
2. The different instance families are general purpose, compute optimized, memory optimized, accelerated computing, and storage optimized.
3. General-purpose instances provide a good balance of compute, memory, and networking resources. They can be used for lots of diverse workloads, like web services or code repositories. They’re also a good starting point if you don’t know how your workload will perform ahead of time.
4. Compute-optimized instances are ideal for compute-intensive tasks, like gaming servers, high-performance computing, machine learning tasks, and scientific modeling.
5. Memory-optimized instances are good for memory-intensive tasks. They deliver fast performance for workloads that process large data sets in memory.
6. Accelerated-computing instances are good for floating-point number calculations, graphics processing, or data pattern matching.
7. Storage-optimized instances are ideal for workloads that require high performance for locally stored data.

## AWS resource provision
1. In AWS, tasks such as launching an EC2 instance, stopping an instance, or modifying instance settings are done through API requests.
2. APIs provide predefined methods to interact with, manage, and configure AWS resources efficiently.
3. Three ways to interact with AWS services:
   1. AWS Management Console
   2. AWS Command Line Interface
   3. AWS SDK (Software Development Kit)
4. When we deploy an EC2 instance, you are responsible for configuring security, managing the guest operating system (OS), applying updates, and setting up firewalls (security groups).

## AMI (Amazon Machine Images)
1. AMIs are pre-built virtual machine images that have the basic components needed to start an instance.
2. An AMI includes the operating system, storage setup, architecture type, permissions for launching, and any extra software that is already installed.
3. You can use one AMI to launch several EC2 instances that all have the same setup.
4. To launch an EC2 instance for a web server, configure the AMI to define the operating system and software; select the instance type to allocate CPU, memory, and storage; and set up storage options, including the type and size of the volume.
5. Three ways to use AMIs:
   1. Create your own by building a custom AMI with specific configurations and software tailored to your needs.
   2. Use pre-configured AWS AMIs, which are set up for common operating systems and software.
   3. Purchase AMIs from the AWS Marketplace, where third-party vendors offer specialized software designed for specific use cases.
6. AMI repeatability is provided as generally all the configurations are identical, and deployments are automated and consistent. Helps when scaling, reduces errors, and streamlines managing large-scale environments.

## AWS Pricing options
1. On-Demand Instances: Pay only for the compute capacity you consume with no upfront payments or long-term commitments required.
2. Reserved Instances: Get a savings of up to 75 percent by committing to a 1-year or 3-year term for predictable workloads using specific instance families and AWS Regions.
3. Spot Instances: Bid on spare compute capacity at up to 90 percent off the On-Demand price, with the flexibility to be interrupted when AWS reclaims the instance.
4. Savings Plans: Save up to 72 percent across a variety of instance types and services by committing to a consistent usage level for 1 or 3 years.
5. Dedicated Hosts: Reserve an entire physical server for your exclusive use. This option offers full control and is ideal for workloads with strict security or licensing needs.
6. Dedicated Instances: Pay for instances running on hardware dedicated solely to your account. This option provides isolation from other AWS customers.
7. Dedicated Hosts offer exclusive use of a server with full control, whereas Dedicated Instances provide isolation without server control.

## Scaling and Elasticity
1. Scalability is about a system’s potential to grow over time. Refers to the ability of a system to handle an increased load by adding resources.
2. Scale up (vertical scaling) by adding more power to existing machines, or you can scale out (horizontal scaling) by adding more machines.
3. Elasticity is about the dynamic, on-demand adjustment of resources in response to real-time.
4. A system can then rapidly adjust its resources, scaling out during periods of high demand and scaling in when the demand decreases.
5. Elasticity provides cost efficiency and optimal resource usage at any given moment.
6. Amazon EC2 Auto Scaling automatically adjusts the number of EC2 instances based on changes in application demand, providing better availability.
   1. Dynamic scaling adjusts in real time to fluctuations in demand.
   2. Predictive scaling preemptively schedules the right number of instances based on anticipated demand.
7. Auto scaling group is configured with three key settings:
   1. Minimum capacity
   2. Desired capacity
   3. Maximum capacity

## Elastic Load Balancing
1. Automatically distributes incoming application traffic across multiple resources, such as EC2 instances, to optimize performance and reliability.
2. A load balancer serves as the single point of contact for all incoming web traffic to an Auto Scaling group.
3. ELB advantages:
   1. Efficient traffic distribution: ELB evenly distributes traffic across EC2 instances, preventing overload on any single instance and optimizing resource utilization.
   2. Automatic scaling: ELB scales with traffic and automatically adjusts to changes in demand for a seamless operation as backend instances are added or removed.
   3. Simplified management: ELB decouples front-end and backend tiers and reduces manual synchronization. It also handles maintenance, updates, and failover to ease operational overhead.
4. Routing Methods:
   1. Round Robin: Distributes traffic evenly across all available servers in a cyclic manner.
   2. Least Connections: Routes traffic to the server with the fewest active connections, maintaining a balanced load.
   3. IP Hash: Uses the client’s IP address to consistently route traffic to the same server.
   4. Least Response Time: Directs traffic to the server with the fastest response time, minimizing latency.
5. EventBridge: Route events from sources like custom apps, AWS services, and third-party software to other applications. EventBridge simplifies the process of receiving, filtering, transforming, and delivering events, so you can quickly build reliable applications. Even if one service fails, EventBridge will store the event and process it as soon as the service is available again.
6. Amazon SQS: a message queuing service that facilitates reliable communication between software components. It can send, store, and receive messages at any scale, making sure messages are not lost and that other services don't need to be available for processing. In Amazon SQS, an application places messages into a queue, and a user or service retrieves the message, processes it, and then removes it from the queue.
7. Amazon SNS: Amazon SNS is a publish-subscribe service that publishers use to send messages to subscribers through SNS topics. In Amazon SNS, subscribers can include web servers, email addresses, Lambda functions, and various other endpoints.

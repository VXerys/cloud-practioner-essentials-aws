# AWS Cloud Practitioner Essentials: Introduction to Cloud Computing

## Objectives 📚

In this module, you will learn how to:
- Explain the basic benefits of Amazon EC2.
- Identify differences among types of Amazon EC2 instances.
- Distinguish various billing options for Amazon EC2.
- Summarize the benefits of Amazon EC2 Auto Scaling.
- Outline the benefits of Elastic Load Balancing.
- Provide examples of using Elastic Load Balancing.
- Explain the difference between Amazon Simple Notification Service (Amazon SNS) and Amazon Simple Queue Service (Amazon SQS).
- Present additional compute options available on AWS.

---

## Introduction to Amazon Elastic Compute Cloud (Amazon EC2) 🚀

In this module, we will delve deeply into a service called **Amazon Elastic Compute Cloud (Amazon EC2)**.

### Client-Server Model Analogy 🏠
Recall our coffee shop scenario where the cashier represents the server and the customer represents the client. Clients send requests to the server, the server processes the request, and then sends back a response. This analogy applies similarly to various business models, whether healthcare, manufacturing, insurance, or video content delivery—all rely on the client-server model to serve products, resources, or data to customers.

### Why Do You Need EC2? 🛠️
You need a server that provides computational power to run applications and meets your business needs. In AWS, this server is virtualized. The service that allows you to access these virtual servers is called **Amazon EC2**.

### Benefits of Using EC2 🌈
Using EC2 offers flexible, cost-effective, and fast computational resources compared to running servers in an on-premises data center.

#### Comparison: On-Premises vs. EC2
- **On-Premises**: 
  - Requires extensive research to determine the type and quantity of servers needed.
  - Involves upfront costs and long wait times (weeks to months) for server delivery.
  - After receiving the servers, installation, configuration, and integration are required.
  - Servers remain active even if underutilized, leading to wasted resources and costs.

- **EC2**:
  - AWS handles the complexities, including building and securing data centers, purchasing, configuring, and installing servers.
  - You can request and use EC2 instances within minutes, scaling up or down based on demand.
  - Pay for what you use, avoiding unnecessary costs for idle resources.
  - EC2 runs on virtual machines hosted on AWS-managed physical servers, enabling efficient resource sharing and isolation.

### EC2 Instance Types 🎮
You can choose from various instance types based on your application requirements:
- **Small Instance**: Ideal for lightweight applications.
- **Medium/Large Instance**: Suitable for applications requiring more memory and CPU.
- **Custom Configurations**: Mix and match configurations to support diverse business applications.

### EC2 Features 🛠️
- **Operating Systems**: Choose between Windows or Linux.
- **Software Installation**: Install any software, including business applications, web servers, databases, and third-party software.
- **Vertical Scaling**: Adjust instance size by adding more memory and CPU as needed.
- **Networking Control**: Configure network settings, including public or private access.
- **Virtualization Technology**: EC2 instances run on virtual machines managed by AWS, ensuring isolation and security.

### How Does EC2 Work? 🔍
1. **Launch**: Select a template with a base configuration (OS, application server, etc.) and specify instance type and security settings.
2. **Connect**: Access the instance via SSH, RDP, or API.
3. **Use**: Once connected, install software, add storage, and manage files.

---

## Additional Compute Services on AWS 🌐

AWS offers several additional compute services beyond EC2:

### Amazon EC2 Auto Scaling 🔄
- Automatically adjusts the number of EC2 instances based on demand.
- Ensures optimal performance and cost efficiency.

### Elastic Load Balancing (ELB) ⚖️
- Distributes incoming traffic across multiple EC2 instances.
- Provides high availability and fault tolerance.

#### Example of ELB:
- Suppose you have a web application with high traffic. ELB can distribute the load evenly across multiple instances, ensuring no single instance becomes overwhelmed.

### Amazon Simple Notification Service (SNS) 📣
- A fully managed pub/sub messaging service.
- Sends notifications to multiple endpoints (email, SMS, mobile push, etc.).

### Amazon Simple Queue Service (SQS) 📡
- A fully managed message queuing service.
- Stores messages temporarily until they are processed.

#### Difference Between SNS and SQS:
- **SNS**: Publish-subscribe model for broadcasting messages to multiple subscribers.
- **SQS**: Queue-based model for sending messages to a single recipient.

---

## Next Steps
Continue to the next episode to explore AWS Global Infrastructure and learn how to deliver content to customers worldwide efficiently.

[👉 **Next Episode: Exploring AWS Global Infrastructure**](next-episode.md)
[👈 **Previous Episode: Benefits of Cloud Computing**](previous-episode.md)

---

**References:**
- For more information on cloud computing, see [[1]].
- For an overview of EC2, visit [[6]].
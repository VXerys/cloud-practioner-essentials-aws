# AWS Cloud Practitioner Essentials: Additional Compute Services

## Overview 🌐

In addition to **Amazon EC2**, AWS offers several other compute services that cater to different use cases and levels of infrastructure management. These services range from fully managed serverless options to container orchestration platforms. Let's explore each of these services in detail.

---

## EC2 Instance Review 🚀

**EC2 Instances** are virtual machines that you can use on AWS. They are versatile and suitable for various use cases, from running simple web servers to high-performance computing clusters.

### Responsibilities When Using EC2:
- **Patch Management**: Keeping software packages updated.
- **Scaling**: Managing horizontal and vertical scaling.
- **High Availability**: Designing applications to be highly available.
- **Infrastructure Management**: Handling data centers, servers, and other infrastructure components.

---

## Serverless Computing 🌱

### What is Serverless Computing?
Serverless computing abstracts away the underlying infrastructure, allowing you to focus solely on writing code. AWS handles all the management, scaling, high availability, and maintenance, so you can concentrate on your application.

### AWS Lambda
**AWS Lambda** is a serverless compute service that lets you run code without provisioning or managing servers. It is fully managed, automatically scales, and is highly available.

#### Key Features:
- **Automatic Scaling**: Handles 1 to 1000 triggers.
- **Pay-per-Use**: You only pay for the compute time used.
- **Limited Runtime**: Best suited for short-running tasks (under 15 minutes).

#### How AWS Lambda Works:
1. **Upload Code**: Upload your code to AWS Lambda.
2. **Configure Triggers**: Set up triggers from AWS services, mobile apps, or HTTP endpoints.
3. **Execution**: Code runs only when triggered.
4. **Billing**: Pay based on the compute time used.

**Source**: [AWS Lambda Documentation](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)

---

## Containers 🐳

If you need more control over your infrastructure but want to maintain efficiency and portability, consider using container services like **Amazon Elastic Container Service (Amazon ECS)** and **Amazon Elastic Kubernetes Service (Amazon EKS)**.

### Docker Containers
Containers are lightweight, standalone, executable packages that contain everything needed to run a piece of software, including code, runtime, libraries, and system tools. Docker is a popular platform for building, testing, and deploying containerized applications.

### Container Orchestration
Container orchestration automates the deployment, management, and scaling of containerized applications. AWS offers two primary services for container orchestration:

#### Amazon Elastic Container Service (Amazon ECS)
**Amazon ECS** is a high-performance container management system that allows you to run and scale containerized applications on AWS. It supports Docker containers and provides APIs to launch and stop applications.

**Source**: [Amazon ECS Documentation](https://docs.aws.amazon.com/AmazonECS/latest/userguide/what-is-ECS.html)

#### Amazon Elastic Kubernetes Service (Amazon EKS)
**Amazon EKS** is a fully managed Kubernetes service that enables you to run Kubernetes on AWS. Kubernetes is an open-source tool for deploying and managing containerized applications at scale.

**Source**: [Amazon EKS Documentation](https://aws.amazon.com/eks/)

### AWS Fargate
**AWS Fargate** is a serverless compute engine for Amazon ECS and Amazon EKS. With Fargate, you don't need to provision or manage servers, as AWS handles all the infrastructure for you. You only pay for the resources needed to run your containers.

**Source**: [AWS Fargate Documentation](https://aws.amazon.com/fargate/)

---

## Choosing the Right Compute Service 🧭

- **Amazon EC2**: Ideal for applications requiring full control over the underlying infrastructure.
- **AWS Lambda**: Best for short-running, event-driven functions.
- **Amazon ECS/EKS**: Suitable for containerized applications, offering flexibility and scalability.
- **AWS Fargate**: Provides serverless container management, ideal for those who want to focus on applications rather than infrastructure.

---

## Next Steps
Continue to the next episode to summarize the material covered so far and prepare for the final assessment.

[👉 **Next Episode: Summary and Final Assessment**](next-episode.md)

[👈 **Previous Episode: Messaging and Queueing**](previous-episode.md)

---

**References:**
- [AWS Lambda Documentation](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)
- [Amazon ECS Documentation](https://docs.aws.amazon.com/AmazonECS/latest/userguide/what-is-ECS.html)
- [Amazon EKS Documentation](https://aws.amazon.com/eks/)
- [AWS Fargate Documentation](https://aws.amazon.com/fargate/)
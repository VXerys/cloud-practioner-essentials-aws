# AWS Cloud Practitioner Essentials: Summary of Cloud Computing

## Overview 🌐

We’ve reached the end of the module. Let’s recap what we’ve learned:

---

## Key Takeaways 🧭

### Definition of Cloud Computing
AWS defines cloud computing as the on-demand provision of IT resources over the internet, with pricing based on usage. This means you can request IT resources like compute, networking, storage, analytics, and more, paying only for what you use at the end of each month.

### AWS Services Overview
AWS offers a wide range of services across various categories. So far, we’ve discussed several services, including **Amazon EC2**, which allows you to dynamically create and delete virtual servers called **EC2 instances**.

### EC2 Instance Types
- **General Purpose**: Balanced compute, memory, and networking.
- **Compute Optimized**: High-performance processors for intensive workloads.
- **Memory Optimized**: High memory bandwidth for large datasets.
- **Accelerated Computing**: Hardware-accelerated processing for specific tasks.
- **Storage Optimized**: High throughput for large datasets.

### Scaling EC2 Instances
- **Vertical Scaling**: Adjust the size of an instance.
- **Horizontal Scaling**: Launch additional instances.
- **Automated Horizontal Scaling**: Use **Amazon EC2 Auto Scaling** to scale automatically based on demand.

### Load Balancing
Once you scale horizontally, you need a way to distribute incoming traffic. Use **Elastic Load Balancer (ELB)** to evenly distribute traffic across instances.

### EC2 Pricing Models
- **On-Demand**: Most flexible, with no upfront commitment.
- **Spot Instances**: Use unused capacity at discounted rates.
- **Reserved Instances**: Commit to a specific level of usage for 1 or 3 years to get discounts.
- **Savings Plans**: Commit to a dollar amount of usage over 1 or 3 years for significant savings. Applicable to EC2, **AWS Lambda**, and **AWS Fargate**.

### Messaging Services
Two messaging services were covered:
- **Amazon Simple Queue Service (Amazon SQS)**: Decouples system components by queuing messages. Messages remain in the queue until processed or deleted.
- **Amazon Simple Notification Service (Amazon SNS)**: Sends messages to multiple endpoints, such as email, SMS, push notifications, or HTTP requests. Once published, messages are sent to all subscribers.

### Additional Compute Services
Beyond virtual servers, AWS offers services for containerized applications:
- **Amazon Elastic Container Service (Amazon ECS)**: Manages Docker containers on EC2 instances.
- **Amazon Elastic Kubernetes Service (Amazon EKS)**: Manages Kubernetes clusters on EC2 instances.
- **AWS Fargate**: A serverless compute engine for ECS and EKS, allowing you to run containers without managing the underlying infrastructure.

### AWS Lambda
**AWS Lambda** allows you to upload code and configure it to run based on triggers. You are charged only when the code executes. No need for containers or virtual machines—just code and configuration.

---

## Recap of Key Concepts 🧬

- **Cloud Computing**: On-demand, pay-as-you-go IT resources.
- **EC2 Instances**: Virtual servers with various types optimized for different workloads.
- **Auto Scaling**: Automatically adjusts the number of instances based on demand.
- **Load Balancing**: Distributes traffic evenly across instances.
- **Messaging Services**: Decouples components and ensures reliable communication.
- **Container Services**: Orchestrates Docker containers for scalable applications.
- **Serverless Computing**: Focuses on code execution without managing infrastructure.

---

## Next Steps
Continue to the next episode to wrap up the course and prepare for the final assessment.

[👉 **Next Episode: Final Assessment**](next-episode.md)

[👈 **Previous Episode: Additional Compute Services**](previous-episode.md)

---

**References:**
- [AWS Cloud Computing Overview](https://aws.amazon.com/cloud-computing/)
- [Amazon EC2 Documentation](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html)
- [Amazon EC2 Auto Scaling Documentation](https://docs.aws.amazon.com/autoscaling/ec2/userguide/introduction.html)
- [Elastic Load Balancing Documentation](https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/introduction.html)
- [Amazon SQS Documentation](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/welcome.html)
- [Amazon SNS Documentation](https://docs.aws.amazon.com/sns/latest/dg/welcome.html)
- [Amazon ECS Documentation](https://docs.aws.amazon.com/AmazonECS/latest/userguide/what-is-ECS.html)
- [Amazon EKS Documentation](https://aws.amazon.com/eks/)
- [AWS Fargate Documentation](https://aws.amazon.com/fargate/)
- [AWS Lambda Documentation](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)
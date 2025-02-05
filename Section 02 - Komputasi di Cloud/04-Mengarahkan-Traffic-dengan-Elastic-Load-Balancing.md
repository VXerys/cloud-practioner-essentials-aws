# AWS Cloud Practitioner Essentials: Directing Traffic with Elastic Load Balancing

## Overview 🌐

In the previous module, we successfully addressed the issue of scaling with Amazon EC2 Auto Scaling. However, we still face another challenge: **traffic distribution**.

---

## Problem Statement 🚫

Consider our coffee shop scenario again. We now have 3 cashier instances ready to handle the influx of customers. However, most customers tend to queue up at one cashier, causing uneven distribution and leaving other cashiers idle.

This problem arises because customers are unsure which cashier to approach. To solve this, we could hire a host to direct customers to the shortest queue. This ensures even distribution and efficient service.

Similarly, in an AWS environment, you need to distribute incoming requests evenly across multiple EC2 instances to prevent any single instance from becoming overloaded. This process is known as **load balancing**.

---

## Elastic Load Balancing (ELB) 🛠️

AWS provides a high-performance, cost-effective, highly available, and automatically scalable load balancer called **Elastic Load Balancing (ELB)**. ELB automatically distributes incoming traffic across multiple resources, such as EC2 instances, ensuring optimal performance and availability.

### Key Features:
- **Automatic Distribution**: Evenly distributes traffic across instances.
- **High Availability**: ELB is a regional construct, meaning it runs at the region level, ensuring high availability.
- **Automatic Scaling**: ELB can scale automatically to handle increased traffic without affecting hourly costs.
- **Integration with Auto Scaling**: Works seamlessly with Amazon EC2 Auto Scaling to ensure high performance and availability.

---

## How ELB Works 🔄

### Scenario: Handling Increased Traffic

- **Normal Traffic**: During regular hours, traffic is manageable.
- **Flash Sale Promo**: Suddenly, traffic surges due to a promotional event.
  - **Scaling Out**: EC2 Auto Scaling adds more instances to handle the increased traffic.
  - **Traffic Redistribution**: ELB automatically directs traffic to the newly added instances.
- **Post-Promo**: Traffic decreases, and EC2 Auto Scaling scales in, terminating some instances.
  - **Graceful Shutdown**: ELB stops sending traffic to instances being terminated, ensuring no requests are left hanging.

### Internal Traffic Management

ELB is not just for external traffic. It can also manage internal traffic within an AWS architecture. For example, in a system with separate ordering and production instances, ELB ensures that requests are directed to the least busy production instance.

- **Before ELB**: Each ordering instance knew all production instances, complicating communication and coordination.
- **With ELB**: Ordering instances use a single URL, and ELB directs traffic to the least busy production instance. Production instances register themselves with ELB, simplifying communication and decoupling the architecture.

---

## Benefits of ELB 🌱

- **Even Distribution**: Ensures no single instance is overloaded.
- **High Availability**: Automatically recovers from failures.
- **Scalability**: Scales automatically to handle increased traffic.
- **Decoupled Architecture**: Simplifies communication between different parts of your architecture.

---

## Next Steps
Continue to the next episode to explore AWS Global Infrastructure and learn how to deliver content to customers worldwide efficiently.

[👉 **Next Episode: Exploring AWS Global Infrastructure**](next-episode.md)
[👈 **Previous Episode: Capacity Adjustment in Amazon EC2**](previous-episode.md)

---

**References:**
- For more details on Elastic Load Balancing, visit the official AWS documentation [[11]].
- Learn how to configure and use ELB in your AWS environment [[12]].
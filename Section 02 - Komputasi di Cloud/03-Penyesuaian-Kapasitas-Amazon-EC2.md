# AWS Cloud Practitioner Essentials: Capacity Adjustment in Amazon EC2

## Overview 🌐

In this module, we will explore the concept of **scalability and elasticity** in AWS, focusing on how Amazon EC2 Auto Scaling helps you adjust capacity based on demand. We'll discuss how this capability addresses the challenges of traditional on-premises data centers and how it can improve your application's availability and performance.

---

## Challenges of On-Premises Data Centers 🚧

In a typical business scenario, workloads vary over time. There are periods of high activity and periods of low activity. Using an on-premises data center presents a dilemma:

- **Under-provisioning**: If you buy hardware based on average usage, you risk running out of capacity during peak times, leading to poor customer experience.
- **Over-provisioning**: If you buy hardware to meet peak demand, you end up with underutilized resources, leading to wasted costs.

With AWS, you can configure your workloads to automatically adjust based on conditions you define, ensuring consistent application availability and optimal resource utilization.

---

## Introduction to Scalability and Elasticity 🔄

### What is Scaling?
Scaling refers to the ability to adjust capacity in response to changes in demand. There are two main types of scaling:

- **Horizontal Scaling (Scaling Out)**: Adding more instances to handle increased load.
- **Vertical Scaling (Scaling Up)**: Increasing the capacity of existing instances.

### Why is Scaling Important?
- **Availability**: Ensure applications are always available, even during peak times.
- **Efficiency**: Only pay for the resources you use, avoiding over-provisioning.
- **Performance**: Maintain optimal performance by adjusting resources as needed.

---

## Amazon EC2 Auto Scaling 🚀

Amazon EC2 Auto Scaling automates the process of adding or removing EC2 instances based on demand. This ensures that your applications remain available and responsive.

### Two Approaches:
1. **Dynamic Scaling**: Responds to changes in demand in real-time.
2. **Predictive Scaling**: Automatically schedules the appropriate number of EC2 instances based on predicted demand.

You can use both approaches together for faster and more efficient scaling.

### Scaling Methods:
- **Scaling Up (Vertical Scaling)**: Add more resources (CPU, memory) to existing instances.
- **Scaling Out (Horizontal Scaling)**: Add more instances to handle increased load.

#### Example:
- **Scaling Out**: If your coffee shop gets busier, you can add more cashiers (EC2 instances) to handle the increased number of customers (requests).

---

## Auto Scaling Group (ASG) 🔄

An **Auto Scaling Group (ASG)** is a collection of Amazon EC2 instances that are managed and scaled automatically. To configure an ASG, you need to define the following parameters:

### Minimum Capacity
- **Definition**: The minimum number of instances that must be running at all times.
- **Example**: Setting a minimum of 1 ensures that at least one instance is always available.

### Desired Capacity
- **Definition**: The target number of instances that should be running.
- **Example**: Setting desired capacity to 2 means you aim to have 2 instances running, even if only 1 is required.

### Maximum Capacity
- **Definition**: The maximum number of instances that can be launched.
- **Example**: Setting a maximum of 4 ensures that no more than 4 instances are launched, even if demand increases beyond that.

---

## Configuring Auto Scaling Policies 🛠️

You can configure policies to define how and when scaling occurs. Common policies include:

- **Target Tracking**: Adjusts the number of instances to maintain a target value, such as CPU utilization.
- **Step Scaling**: Triggers scaling actions based on predefined thresholds.
- **Simple Scaling**: Increases or decreases the number of instances by a fixed amount.

---

## Benefits of Amazon EC2 Auto Scaling 🌱

- **Cost Efficiency**: Only pay for the resources you use.
- **High Availability**: Ensure applications are always available, even during peak times.
- **Performance Optimization**: Automatically adjust resources to maintain optimal performance.

---

## Next Steps
Continue to the next episode to explore AWS Global Infrastructure and learn how to deliver content to customers worldwide efficiently.

[👉 **Next Episode: Exploring AWS Global Infrastructure**](next-episode.md)
[👈 **Previous Episode: Pricing for Amazon EC2**](previous-episode.md)

---

**References:**
- For more details on Amazon EC2 Auto Scaling, visit the official AWS documentation [[9]].
- Learn how to configure Auto Scaling Groups and policies [[2]].
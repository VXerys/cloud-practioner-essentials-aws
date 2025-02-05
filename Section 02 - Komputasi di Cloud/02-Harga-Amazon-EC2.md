# AWS Cloud Practitioner Essentials: Pricing for Amazon EC2

## Overview 📚

In the previous module, we explored Amazon EC2 and its various instance types. Now, let's dive into the pricing models available for Amazon EC2. Understanding these pricing models is crucial to optimizing your costs and ensuring you choose the right option for your workload.

---

## On-Demand Instances 🕒

**Description**:
- **On-Demand Instances** allow you to pay for compute capacity by the hour or second, depending on the instance type and operating system you choose.
- **Ideal Use Cases**: Short-term testing, development, unpredictable workloads, and experiments.
- **Key Features**:
  - No upfront commitment or long-term contract required.
  - Flexibility to scale up or down as needed.
  
**Link**: For more details on On-Demand pricing, visit the official AWS documentation [[1]].

---

## Savings Plans 📈

**Description**:
- **Savings Plans** offer significant discounts by committing to a certain dollar amount of usage per hour over a period of 1 or 3 years.
- **Discounts**: Up to 72% savings on AWS compute usage, regardless of instance family, size, OS, tenancy, or region.
- **Additional Benefits**: Also applicable to AWS Fargate and AWS Lambda, which are serverless compute options.

**Link**: Learn more about Savings Plans and how they can help you save on AWS costs [[2]].

---

## Reserved Instances (RI) 🔄

**Description**:
- **Reserved Instances** provide significant discounts on On-Demand pricing by committing to a specific level of usage for 1 or 3 years.
- **Types**:
  - **Standard RI**: Fixed commitment for 1 or 3 years.
  - **Convertible RI**: Allows you to change the instance type within the same family after purchase.
  - **Scheduled RI**: For predictable workloads with specific schedules.
- **Payment Options**:
  - **All Upfront**: Pay the full cost upfront for maximum discount.
  - **Partial Upfront**: Pay part of the cost upfront and the rest monthly.
  - **No Upfront**: No upfront payment, but less discount compared to other options.
- **Post-Expiry**: After the reservation ends, you can continue using the instance at On-Demand rates.

**Link**: Explore Reserved Instances and their benefits in detail [[3]].

---

## Spot Instances ⏳

**Description**:
- **Spot Instances** utilize unused Amazon EC2 capacity and offer significant cost savings—up to 90% off On-Demand pricing.
- **Ideal Use Cases**: Workloads that can tolerate interruptions and have flexible start and stop times.
- **Key Features**:
  - AWS may reclaim instances if capacity is needed elsewhere, providing a two-minute warning.
  - Suitable for batch processing, test environments, and non-critical applications.

**Link**: Get more information on Spot Instances and their pricing [[4]].

---

## Dedicated Hosts ⚙️

**Description**:
- **Dedicated Hosts** provide dedicated physical servers for your exclusive use.
- **Ideal Use Cases**: Meeting compliance requirements or when you need to ensure no one else shares the physical server.
- **Key Features**:
  - Allows the use of bring-your-own-license (BYOL) for software licensing.
  - Suitable for applications with strict licensing requirements tied to physical hardware.

**Link**: Discover more about Dedicated Hosts and their pricing [[5]].

---

## AWS Cost Explorer 📊

**Description**:
- **AWS Cost Explorer** helps you visualize, understand, and manage your AWS costs and usage over time.
- **Features**:
  - Analyze usage patterns for Amazon EC2 over the last 7, 30, or 60 days.
  - Receive recommendations for Savings Plans and Reserved Instances based on your historical usage.

**Link**: Learn how to use AWS Cost Explorer to optimize your costs [[6]].

---

## Next Steps
Continue to the next episode to explore AWS Global Infrastructure and learn how to deliver content to customers worldwide efficiently.

[👉 **Next Episode: Exploring AWS Global Infrastructure**](next-episode.md)
[👈 **Previous Episode: Instance Types of Amazon EC2**](previous-episode.md)

---

**References:**
- [1] https://aws.amazon.com/ec2/pricing/on-demand/
- [2] https://aws.amazon.com/savings-plans/
- [3] https://aws.amazon.com/ec2/reserved-instances/
- [4] https://aws.amazon.com/ec2/spot/
- [5] https://aws.amazon.com/ec2/dedicated-hosts/
- [6] https://aws.amazon.com/aws-cost-management/aws-cost-explorer/
# AWS Cloud Practitioner Essentials: Subnet and Network Access Control List (ACL)

## Overview 🌐

In this module, we will delve deeper into **subnets** and **network access control lists (ACLs)**. These are fundamental concepts in AWS networking that help you manage and secure your resources effectively. Let's explore these concepts in detail.

---

## Subnets 🛡️

### What is a Subnet?
- **Definition**: A subnet is a logical division of a VPC (Virtual Private Cloud) that groups resources based on security or operational needs.
- **Types**:
  - **Public Subnet**: Contains resources that need to be publicly accessible, such as web servers.
  - **Private Subnet**: Contains resources that should only be accessed internally, such as databases or application servers.

### Example Scenario:
- **Coffee Shop Analogy**: In our coffee shop scenario, the cashier (public subnet) interacts with customers, while the barista (private subnet) focuses on making coffee without direct customer interaction.

### Communication Between Subnets
- **Within VPC**: Subnets within the same VPC can communicate with each other.
- **Example**: You can have an application running on an EC2 instance in a public subnet communicating with a database in a private subnet.

### Importance of Subnets
- **Isolation**: Keeps sensitive resources isolated from public networks.
- **Control**: Provides granular control over network configurations.
- **Security**: Enhances security by limiting exposure to the public internet.

---

## Network Access Control Lists (ACLs) 🛡️

### What is a Network ACL?
- **Definition**: A network ACL is a virtual firewall that controls inbound and outbound traffic at the subnet level.
- **Function**: Evaluates each packet entering or leaving a subnet to determine whether it should be allowed or denied based on source, destination, protocol, and port.

### Differences Between Network ACLs and Security Groups:
- **Network ACLs**:
  - **Stateless**: Do not track the state of connections.
  - **Subnet-Level**: Operate at the subnet level.
  - **Default Policy**: Default policy denies all inbound traffic and allows all outbound traffic.
  - **Explicit Denial**: Explicit deny rules are evaluated first, followed by explicit allow rules.
- **Security Groups**:
  - **Stateful**: Track the state of connections.
  - **Instance-Level**: Operate at the instance level.
  - **Default Policy**: Default policy denies all inbound traffic and allows all outbound traffic.
  - **Implicit Denial**: Implicit deny rules apply to any traffic not explicitly allowed.

### Example Scenario:
Imagine you are at an airport, and you need to pass through passport control. The passport officer (network ACL) checks each passenger (packet) to ensure they are on the approved list before allowing them to enter the country (subnet).

---

## Security Groups 🛡️

### What is a Security Group?
- **Definition**: A security group is a virtual firewall that controls inbound and outbound traffic at the instance level.
- **Function**: Evaluates each packet entering or leaving an EC2 instance to determine whether it should be allowed or denied based on source, destination, protocol, and port.

### Example Scenario:
Imagine you have a building with a doorman (security group) who checks each person entering the building to ensure they have permission. Once inside, people can move freely, but the doorman does not check those leaving the building.

### Importance of Security Groups:
- **Granular Control**: Allows you to define rules for each EC2 instance.
- **Stateful**: Tracks the state of connections, ensuring that responses to allowed requests are also allowed.
- **Default Policy**: By default, all inbound traffic is denied, and all outbound traffic is allowed.

---

## Packet Flow Through Subnets and Security Groups 🛡️

### Packet Flow Example:
Let's walk through the journey of a packet from one EC2 instance (Instance A) to another EC2 instance (Instance B) in different subnets within the same VPC.

1. **From Instance A to Instance B**:
   - **Security Group Check**: Instance A's security group allows outbound traffic by default, so the packet passes.
   - **Network ACL Check (Subnet 1)**: The network ACL in Subnet 1 checks the packet and allows it if it matches the allowed rules.
   - **Route Table**: The packet is routed to Subnet 2.
   - **Network ACL Check (Subnet 2)**: The network ACL in Subnet 2 checks the packet and allows it if it matches the allowed rules.
   - **Security Group Check**: Instance B's security group checks the packet and allows it if it matches the allowed rules.

2. **Return Traffic (Instance B to Instance A)**:
   - **Security Group Check (Instance B)**: Instance B's security group allows outbound traffic by default, so the packet passes.
   - **Network ACL Check (Subnet 2)**: The network ACL in Subnet 2 checks the packet and allows it if it matches the allowed rules.
   - **Route Table**: The packet is routed back to Subnet 1.
   - **Network ACL Check (Subnet 1)**: The network ACL in Subnet 1 checks the packet and allows it if it matches the allowed rules.
   - **Security Group Check (Instance A)**: Instance A's security group, being stateful, recognizes the return traffic and allows it.

### Stateful vs. Stateless:
- **Stateful (Security Groups)**: Track the state of connections, ensuring that responses to allowed requests are also allowed.
- **Stateless (Network ACLs)**: Do not track the state of connections, evaluating each packet independently.

---

## Best Practices 🛡️

### Security Best Practices:
- **Use Both Security Groups and Network ACLs**: Combine both for comprehensive network security.
- **Least Privilege**: Grant the minimum necessary permissions to ensure security.
- **Regular Audits**: Regularly review and update security configurations to address vulnerabilities.

---

## Next Steps
Continue to the next episode to explore AWS Global Infrastructure and learn how to deliver content to customers worldwide efficiently.

[👉 **Next Episode: Detailed Overview of AWS Regions and Availability Zones**](https://aws.amazon.com/about-aws/global-infrastructure/)

[👈 **Previous Episode: Connectivity to AWS**](https://aws.amazon.com/vpc/)

---

**References:**
- For more details on subnets, visit [[1]](https://aws.amazon.com/vpc/subnets/).
- For an overview of network ACLs, refer to [[2]](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html).
- For information on security groups, check [[3]](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/security-groups.html).
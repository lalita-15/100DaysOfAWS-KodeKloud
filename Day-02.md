# Day 2 – AWS Security Group Configuration

## Task

Create a Security Group named **devops-sg** in the **default VPC** within the **us-east-1** region.

## Objective

Configure a security group to allow HTTP and SSH access for the Nautilus application servers.

## Steps Performed

1. Logged in to the AWS Management Console.
2. Verified the region was set to **us-east-1**.
3. Navigated to **EC2 → Security Groups**.
4. Created a new Security Group with:

   * **Name:** `devops-sg`
   * **Description:** `Security group for Nautilus App Servers`
   * **VPC:** Default VPC
5. Added the following inbound rules:

   * **HTTP (TCP 80)** → Source: `0.0.0.0/0`
   * **SSH (TCP 22)** → Source: `0.0.0.0/0`
6. Kept the default outbound rule (**Allow All Traffic**).
7. Created and verified the Security Group successfully.

## AWS Concepts Learned

* Virtual Private Cloud (VPC)
* Security Groups
* Inbound vs Outbound Rules
* HTTP (Port 80)
* SSH (Port 22)
* CIDR Block (`0.0.0.0/0`)


## Key Takeaways

* Security Groups act as virtual firewalls for AWS resources.
* Inbound rules define incoming traffic permissions.
* Outbound rules control outgoing traffic.
* Opening ports to `0.0.0.0/0` allows access from any IP address and should be used carefully in production environments.

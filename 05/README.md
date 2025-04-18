#Section 05 : EC2 - Elastic Compute Cloud
## Lesson 34 : AWS Budget Setup

Set up an alarm for cost savings. Click the upper right drop-down and select Billing and Cost Management. IAM Users will need access to billing data - this must be activated for users via the root account.  

Billing and Cost Management > Bills > Charges by service.  

Billing and Cost Management > Budgets > Create Budget. Set a 0$ budget via the template. Add your email and you will be notified when cost exceeds zero.  

## Lesson 35 : EC2 Basics

Elastic Compute Cloud == Infrastructure as a Service. This is a virtual machine. Store your data on EBS volumes. Distribute load across machines using Elastic Load Balancer (EBS). Scale the service usince an anut-scaling group (ASG).  

### Sizing and Configuration :
- OS : Linux, Mac, or Windows.  
- CPU : How much power and how many cores.  
- RAM : How much random access memory.  
- Storage : EBS and EFS are network attached, whereas EC2 Instance Store is hardware.  
- Network : Speed and Public IP.  
- Firewall : Security Group.  
- Bootstrap : EC2 User Data - Configured at first launch.  

### EC2 User Data :
Bootstrap EC2 instances. Launch commands at instance *first start*. Used to automate tasks such as installing updates, install software, download common files, etc. This is run as the root user.  

### Instance Types :
There are a multitude of types. For our purposes, the t2.micro is the one we will be using as it it part of the free tier.  

## Lesson 36 : EC2 Instance with User Data

EC2 Console > Instances > Launch Instances. Name it & Tag it. Select the base image of Amazon Linux 2 AMI, Architecture X86. Select instance type: t2-micro.  

- Create or Add an existing key-pair. 
- Subnet - Use the default subnet in the AZ.  
- Auto assign public IP = Enabled.   
- Security Group - Created for you, ostensibly called "launch-wizard-1".  
- Allow SSH traffic from Anywhere.  
- Allow HTTP traffic from the internet.  
- Configure storage. 8gb gp2 root volume is sufficient.
- Advanced : scroll to the bottom to add user data.  

## Lesson 37 : Instance Types

Different instance types are optimized for different use cases. General purpose, Compute, Memory optimized, Storage optimized, Accelerated computing, etc.  

Naming of instance types is decoded in the following way. m5.2xlarge == m is the intance class, 5 is the generation, and 2xlarge denotes the size.  
General purpose instances have a good balance of compute, memory, networking. We will be using the t2.micro.  

Compute Optimized : Batch processing, Media transcoding, performant web servers, performant computing, scientific modeling, machine learning, dedicated gaming servers. c5, c6.  

Memory Optimized : High performance databses, web cache, big unstructured data. r, x, and z series.  

Storage Optimized : Large datasets, Hight frequency online transactional processing, Relational and NoSQL databases, cache in-memory databases like redis, data warehousing, distributed filesystems. i, d and h series.  

https://instances.vantage.sh for more information.  

## Lesson 38 : Security Groups and Ports`

Security groups are fundamental to network security. They control traffic in and out. Security groups only contain allow rules and these rules can reference by IP or by security group.  

SG's act as a firewall and regulate:
- Access to ports.  
- Authorized IP ranges - ipv4 and ipv6.  
- Control inbound and outbound traffic.  

Type : Protocol : Port Range : Source : Description  

Security groups can be attached to multiple instances. SG's are locked to a region/VPC combo. SG's exist outside the EC2. Maintain a single securtiy group for SSH access. Timeouts typically indicate an issue with your SG's, whereas "connection refused" its either not launched or and application error. By default : all inbound traffic is blocked and all outbound traffic is allowed.  

Referencing other security groups. Authorized security group allow other instances with that security group access to the instance.

Classic ports to know: SSH port 22, FTP port 21, SFTP port 22, HTTP port 80, HTTPS port 443, RDP port 3389.  

## Lesson 39 : Security Groups Hands On

## Lesson 40 : SSH Overview

## Lesson 41 : SSH Mac`

## Lesson 42 : SSH Windows

## Lesson 43 : SSH Windows 10

## Lesson 44 : Troubleshooting

## Lesson 45 : Instance Connect

## Lesson 46 : Instance Roles

## Lesson 47 : Instance Purchasing Options

## Lesson 48 : IP Address Changes

## Lesson 49 : Shared Responsibility EC2

## Lesson 50 : EC2 Summary

## Quiz : EC2 Quiz


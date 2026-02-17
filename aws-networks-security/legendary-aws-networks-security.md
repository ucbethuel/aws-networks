<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# VPC Traffic Flow and Security

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-security)

**Author:** ucbethuel  
**Email:** orjiucbethuel@gmail.com

---

## VPC Traffic Flow and Security

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-security_92b0b0b4)

---

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is Virtual Private Cloud and it is useful because it wrap all your amazon resources making them private and controllable by you.

### How I used Amazon VPC in this project

In today's project, I used Amazon VPC to connect traffic flow and add some security.

### One thing I didn't expect in this project was...

One thing I didn't expect in this project was it easy demonstration and practice.

### This project took me...

This project took me 2 hours.

---

## Route tables

Route tables are are rules that direct how network traffic flows.

Routes tables are needed to make a subnet public because, it is right their we will be able to truly connect the subnet to the internet.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-security_0a07b191)

---

## Route destination and target

Routes are defined by their destination and target, which mean sources of network flow and the subnet or IP within the VPC.

The route in my route table that directed internet-bound traffic to my internet gateway had a destination of 0.0.0.0/0 and a target of igw-xxxxxxxxxxxxxxxxx

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-security_0a07b191)

---

## Security groups

Security groups are like checkpoint which must first we meet before accessing a resources.

### Inbound vs Outbound rules

Inbound rules are rules concerned on how data coming in are to be treated, I  configured an inbound rule that allow HTTP to access or interact with my resources.

Outbound rules are set public, By default, my security group's outbound rule allows sending data to all IP addresses whether in VPC or not. 

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-security_92b0b0b4)

---

## Network ACLs

Network ACLs are securities located at your subnet, that checks for inbound and outbound traffic.

### Security groups vs. network ACLs

The difference between a security group and a network ACL is that, Security group is attached to resources while Network ACL is attached to Subnet.

---

## Default vs Custom Network ACLs

### Similar to security groups, network ACLs use inbound and outbound rules

By default, a network ACL's inbound and outbound rules will allow all traffic wheather inbound or outbound set at rule 100, while every other rule it denies, of which do not actually take effect.

In contrast, a custom ACL’s inbound and outbound rules are automatically set to deny all traffic coming in.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-security_4faeb056)

---

## Tracking VPC Resources

---

---

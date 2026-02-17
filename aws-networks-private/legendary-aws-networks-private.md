<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Creating a Private Subnet

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-private)

**Author:** ucbethuel  
**Email:** orjiucbethuel@gmail.com

---

## Creating a Private Subnet

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-private_afe1fdbd)

---

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is Amazon Virtual Private Cloud, which help us connect internal resource together, without been exposed to the internet by default.

### How I used Amazon VPC in this project

In today's project, I used Amazon VPC to create a private subnet, private route tbale and NACL

### One thing I didn't expect in this project was...

One thing I didn't expect in this project is clearer understanding.

### This project took me...

This project took me 1 hour, 30 min

---

## Private vs Public Subnets

The difference between public and private subnets is that public subnet is expose to the internet while private is only meant for internal connection.

Having private subnets are useful because it helps us connect user data without exposing it to the internet.

My private and public subnets cannot have the same CIDR block.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-private_afe1fdbd)

---

## A dedicated route table

By default, my private subnet is associated with the Network route table earlier connected.

I had to set up a new route table because so to associate my new private subnet and making it private.

My private subnet's dedicated route table only has one inbound and one outbound rule that allows communication internally.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-private_b4b904b5)

---

## A new network ACL

By default, my private subnet is associated with My previous NextWork Network ACL created in the last class.

I set up a dedicated network ACL for my private subnet because, i have to set up the applicable rules that will make the subnet private.

My new network ACL has two simple rules -
1. Block all inbound traffic.
2. Block all Outbound traffic.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-private_1ed2cb07)

---

---

<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Build a Virtual Private Cloud

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-vpc)

**Author:** ucbethuel  
**Email:** orjiucbethuel@gmail.com

---

## Build a Virtual Private Cloud (VPC)

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-vpc_2facf927)

---

## Introducing Today's Project!

In this project, I will demonstrate how to use VPC (Virtual Private Cloud) in AWS

### What is Amazon VPC?

Amazon VPC is a Virtual Private Cloud, and it is useful because it separate our resources privately with AWS Cloud services.

In today's project, I used Amazon VPC to create my own private cloud and also created a subnet.

### Personal reflection

This project took me 1:30 hour

One thing I didn't expect in this project was how easy it was in creating aws vpc.

---

## Virtual Private Clouds (VPCs)

### What I did in this step

In this step, I will access a VPC management console and create my own VPC.

### How VPCs work

VPCs are Virtual Private Cloud, It what makes all our resource created private and protected.

### Why there is a default VPC in AWS accounts

There was already a default VPC in my account ever since my AWS account was created. This is because it enables services like S3 and lambda function to connect to the internet and be used.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-vpc_2facf927)

### Defining IPv4 CIDR blocks

To set up my VPC, I had to define an IPv4 CIDR block, which is the scope of availbale IP Addresses that should be made available with my network.

---

## Subnets

### What I did in this step

In this step, I will creating a subnet, which is like organising our big city into areas and street.

### Creating and configuring subnets

Subnets are grouping of your private network. There are already subnets existing in my account, one for every Availability Zones.

### Public vs private subnets

The difference between public and private subnets are, Public subnet are designed to be connected to the internet while private are not. For a subnet to be considered public, it has to connected to an internet gateway.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-vpc_157c4219)

### Auto-assigning public IPv4 addresses

Once I created my subnet, I enabled the auto-enable assign public IP address. This setting makes sure any resource created with the subnet is given an ip addresses.

---

## Internet gateways

### What I did in this step

In this step, I will connect my VPC to an internet gateway because i want resource to be access over the internet.

### Setting up internet gateways

Internet gateways are what connect our VPC to the internet world.

Attaching an internet gateway to a VPC means I am exposing my VPC to be accessible via the internet.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-vpc_4ae90410)

---

## Using the AWS CLI

### What I'm doing in this extension

### Exploring CloudShell and CLI

### Debugging my setup

### Comparing CloudShell vs AWS Console

---

---

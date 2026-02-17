<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# VPC Peering

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-peering)

**Author:** ucbethuel  
**Email:** orjiucbethuel@gmail.com

---

## VPC Peering

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-peering_88727bef)

---

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is Virtual Private Cloud and it is useful because it helps us create private
network and connect our resources together.

### How I used Amazon VPC in this project

In today's project, I used Amazon VPC in craeting peer connection, that communication between VPC in AWS. and after that test both connection by ping an ec2 instance of one from another.

### One thing I didn't expect in this project was...

One thing I didn't expect in this project was, nothing yet.

### This project took me...

This project took me 2 hours.

---

## In the first part of my project...

### Step 1 - Set up my VPC

In this step, I will be creating two VPC from scratch using Resource map (VPC wizard).

### Step 2 - Create a Peering Connection

In this step, I will be creating a connection link, that will connect my VPC 1 and VPC 2.

### Step 3 - Update Route Tables

In this step, I will configure traffic coming from VPC 1 to get to VPC 2 and vice versa.

### Step 4 - Launch EC2 Instances

In this step, I will launch an ec2 instance, because i need to test if the connectivity worked.

---

## Multi-VPC Architecture

I started my project by launching a 2 VPC with every related such as subnet, route table, internet gateway in two clicks of Create VPC using VPC wizard, where in each VPC i have one subnet connected to internet gateway.

The CIDR blocks for VPCs 1 and 2 are 10.1.0.0/16 and 10.2.0.0/16 respectively.
They have to be unique because there might be VPC Ip overlapping when connecting the two.

### I also launched 2 EC2 instances

I didn't set up key pairs for these EC2 instances as AWS has provided an alternative to launch an instance without the need to manage the keys ourselves rather by themselves.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-peering_11111111)

---

## VPC Peering

A VPC peering connection is a connectivity that exist between two VPC in AWS.

VPCs would use peering connections to connect from one VPC to another.

The difference between a Requester and an Accept-er in a peering connection is, Requestor is the VPC making the request connection and Accept-er the the vpc that the requester is trying to connect to, of which it has the option to accept or decline.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-peering_1cbb1b88)

---

## Updating route tables

After accepting a peering connection, my VPCs' route tables need to be updated because both VPC won't know how to connect with each other, in simple terms, they don't know exactly where they are.

My VPCs 1 new routes have a destination of 10.2.0.0/16 The routes' target was peer connection.

Also My VPCs 2 new routes have a destination of 10.1.0.0/16, the routes' target is also peer connection.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-peering_4a9e8014)

---

## In the second part of my project...

### Step 5 - Use EC2 Instance Connect

In this step, I will use EC2 Instance Connect to connect to your first EC2 instance and resolve possible errors.

### Step 6 - Connect to EC2 Instance 1

In this step, I will use EC2 Instance Connect to connect to Instance 1 (one more time)! and resolve possible errors.

### Step 7 - Test VPC Peering

In this step, I will get Instance 1 to send test messages to Instance 2 and resolve possible errors

---

## Troubleshooting Instance Connect

Next, I used EC2 Instance Connect to to start up our instance directly from AWS console.

I was stopped from using EC2 Instance Connect as there was no public IP addresses associated to it.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-peering_7685490c)

---

## Elastic IP addresses

To resolve this error, I set up Elastic IP addresses. Elastic IP addresses are static IP addresses given that constantly remain the same whenever our instance restart.

Associating an Elastic IP address resolved the error because a public IP addresses was given to our instance, making it easy for us to launch our instance with AWS Instance connect.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-peering_45663498)

---

## Troubleshooting ping issues

To test VPC peering, I ran the command "ping 10.2.10.113" on the terminal

A successful ping test would validate my VPC peering connection because, it makes a request and expect a response, which is a typical way of communicating

I had to update my second EC2 instance's security group because i had to allow ICMP traffic, so therefore I added a new rule that allows all ICMP traffic of IPv4 addresses.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-peering_7a29d352)

---

---

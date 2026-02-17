<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Launching VPC Resources

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-ec2)

**Author:** ucbethuel  
**Email:** orjiucbethuel@gmail.com

---

## Launching VPC Resources

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-ec2_8ee57662)

---

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is Virtual Private Cloud and it is useful because it helps us create private network and connect our resources together.

### How I used Amazon VPC in this project

I used Amazon VPC to connect ec2 instance

### One thing I didn't expect in this project was...

One thing I didn't expect in this project was the misunderstanding i got when creating a new key pair, didn't check out connecting the previous one i once created.

### This project took me...

This project took me 1 hour

---

## Setting Up Direct VM Access

Directly accessing a virtual machine means having ability to do administrative work such as file managment, application lunch, etc.

### SSH is a key method for directly accessing a VM

SSH traffic means secure connection to our ec2, whic communicate via port 22.

### To enable direct access, I set up key pairs

Key pairs are key used in securely connecting to our EC2 instance directly, 

A private key's file format means the extension used in saving you key which also determine the algorithm in used. My private key's file format was ".pem"

---

## Launching a public server

I had to change my EC2 instance's networking settings by connecting my instance to my VPC and the ideal subnet of which i already connected in the last class.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-ec2_88727bef)

---

## Launching a private server

My private server has its own dedicated security group because, it resources are not meant to be access via any computer rather through SSH .

My private server's security group's source is NextWork Security Group, which means only IP addresses belonging to it can communicate with it.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-ec2_4a9e8014)

---

## Speeding up VPC creation

I used an alternative way to set up an Amazon VPC! This time, I use selected VPC and more, then configure the number of subnet and AZ, while on that i look out the resource map to see the reflection of what i was doing.

A VPC resource map is a diagram that shows relationship co existing within your VPC, Subnet, Route table and Internet gateway.

My new VPC has a CIDR block of 10.0.0.0/16. It is possible for my new VPC to have the same IPv4 CIDR block as my existing VPC because they are seperate from each other despite existing in same aws server.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-ec2_1cbb1b88)

---

## Speeding up VPC creation

### Tips for using the VPC resource map

When determining the number of public subnets in my VPC, I only had two options:
1. 0
2. 2 or 1 (if AZ is 1)
 This was because
1. ) if you only want to create an internal network only
2. if you want to connect to the internet

The set up page also offered to create NAT gateways, which are option to connect to aws s3 within your VPC.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-ec2_8ee57662)

---

---

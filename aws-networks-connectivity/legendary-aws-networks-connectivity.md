<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Testing VPC Connectivity

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-connectivity)

**Author:** ucbethuel  
**Email:** orjiucbethuel@gmail.com

---

## Testing VPC Connectivity

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-connectivity_8ee57662)

---

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is Virtual Private Cloud and it is useful because it helps us create private
network and connect our resources together.

### How I used Amazon VPC in this project

In today's project, I used Amazon VPC to test my connectivity within my VPC and the internet.

### One thing I didn't expect in this project was...

Nothing really

### This project took me...

This project took me 1 hour.

---

## Connecting to an EC2 Instance

Connectivity means how well different part of your resources talk to each other.

My first connectivity test was whether I could connect to my ec2 using instance connect, but seems to fail.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-connectivity_88727bef)

---

## EC2 Instance Connect

I connected to my EC2 instance using EC2 Instance Connect, which is an alternative and faster way to connet to ec2, rather then using ssh and taking care of the generated keys.

My first attempt at getting direct access to my public server resulted in an error, because my security group only allows HTTP inbound traffic.

I fixed this error by editing the inbound rules and  added ssh protocol type configuration.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-connectivity_1cbb1b88)

---

## Connectivity Between Servers

Ping is connectivity from two computers or device I used ping to test the connectivity between my public server to my private server

The ping command I ran was "ping 10.0.1.169"

The first ping returned [ec2-user@ip-10-0-0-133 ~]$ ping 10.0.1.169 This meant ICMP might not be allowd or no connectivity.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-connectivity_defghijk)

---

## Troubleshooting Connectivity

I troubleshooted this by checking my inbound and outbound traffic of my NACL, SUbnet and security group.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-connectivity_4a9e8014)

---

## Connectivity to the Internet

Curl is used in transfer and retrieval of data in the internet.

I used curl to test the connectivity between my public server and the internet.

### Ping vs Curl

Ping and curl are different because checks for connectivity and return status, time and amount of time it took while curl is able to transfer or retreive data from the internet.

---

## Connectivity to the Internet

I ran the curl command on my ec2 terminal which returned html response on the console.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-connectivity_8ee57662)

---

---

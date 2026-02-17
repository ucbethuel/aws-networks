<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Access S3 from a VPC

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-s3)

**Author:** ucbethuel  
**Email:** orjiucbethuel@gmail.com

---

## Access S3 from a VPC

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-s3_3e1e79a2)

---

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is Virtual Private Cloud and it is useful because it helps us create private
network and connect our resources together.

### How I used Amazon VPC in this project

In today's project, I used Amazon VPC to to interact with my s3 resource via ec2 instance.

### One thing I didn't expect in this project was...

null

### This project took me...

This project took me 2 hours.

---

## In the first part of my project...

### Step 1 - Architecture set up

In this step, I will
1. Create a VPC from scratch!

2. Launch an EC2 instance into your VPC.

### Step 2 - Connect to my EC2 instance

In this step, I will connect directly to my EC2 instance.

### Step 3 - Set up access keys

In this step, I will give my EC2 instance access to myAWS environment by creating an access key.

---

## Architecture set up

I started my project by launching my VPC using the VPC wizard, and then created an instance known as Instance - NextWork VPC Project, of which i dynamically created a security group along

I also set up aws s3 resource

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-s3_4334d777)

---

## Running CLI commands

AWS CLI is Command Line Interface, I have access to AWS CLI because am using an Instance which command along with the CLI installed.

The first command I ran was aws s3 ls. This command is used to list s3 services connected to my account.

The second command I ran was aws configure. This command is used to set up or login via terminal

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-s3_e7fa8776)

---

## Access keys

### Credentials

To set up my EC2 instance to interact with my AWS environment, I configured my aws cli, providing my access id, secret and region code.

Access keys are like username, modtly used for CLI base login to aws services.

Secret access keys are like the password we provide via terminal that helps us access resources we intend to.

### Best practice

Although I'm using access keys in this project, a best practice alternative is to use AWS CloudShell and AWS CLI V2

---

## In the second part of my project...

### Step 4 - Set up an S3 bucket

In this step, I will lunching aws s2 service, with two files.

### Step 5 - Connecting to my S3 bucket

In this step, I will be try to use my ec2 instance to interact with my s3 resource.

---

## Connecting to my S3 bucket

The first command I ran was aws s3 ls. This command is used to list s3 services connected to my account.

When I ran the command "aws s3 ls" again, the terminal responded with a list of my bucket name, This indicated that my aws configuration was successful and well in sync.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-s3_4334d778)

---

## Connecting to my S3 bucket

Another CLI command I ran was "aws s3 ls s3://nextwork-vpc-project-ucbethuel" which returned a list of object in my buckets.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-s3_4334d779)

---

## Uploading objects to S3

To upload a new file to my bucket, I first ran the command sudo touch /tmp/test.txt This command creates a new file in tmp folder called test.txt.

The second command I ran was "aws s3 cp /tmp/test.txt s3://nextwork-vpc-project-ucbethuel" This command will copy file form a source (i.e /tmp/test.txt) to a destination (i.e s3://nextwork-vpc-project-ucbethuel)

The third command I ran was s3://nextwork-vpc-project-ucbethuel which validated that the test.txt file was copied.

![Image](http://learn.nextwork.org/authentic_vermilion_swift_stingray/uploads/aws-networks-s3_3e1e79a2)

---

---

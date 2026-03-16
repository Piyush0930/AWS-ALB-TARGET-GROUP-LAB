# 🚀 AWS EC2 Advanced Practical Labs

This repository contains **hands-on AWS EC2 advanced labs** covering real-world cloud engineering concepts such as networking, storage, scaling, monitoring, and security.

The goal of this project is to gain **production-level experience with Amazon EC2** and understand how cloud infrastructure works in real environments.

---

# 📌 Topics Covered

* EC2 Instance Launch
* Custom VPC Networking
* Public & Private Subnets
* Bastion Host Architecture
* Security Groups
* EBS Volume Management
* AMI Creation
* Load Balancer
* Auto Scaling
* CloudWatch Monitoring
* IAM Roles for EC2
* Docker Deployment on EC2

---

# 🧠 Architecture Overview

Users → Load Balancer → EC2 Instances → Database

Key Components:

* VPC
* Public Subnet
* Private Subnet
* Internet Gateway
* Route Tables
* EC2 Instances
* Application Load Balancer
* Auto Scaling Group
* CloudWatch

---

# 🧪 Labs

## Lab 1 – EC2 Instance Setup

Steps:

1. Launch an EC2 instance
2. Connect using SSH
3. Install Nginx web server
4. Access the server using the public IP

Command:

sudo apt update
sudo apt install nginx -y

---

## Lab 2 – EBS Volume Attachment

Steps:

1. Create an EBS volume
2. Attach it to the EC2 instance
3. Format the disk
4. Mount it

Commands:

lsblk
sudo mkfs -t ext4 /dev/xvdf
sudo mount /dev/xvdf /data

---

## Lab 3 – Create AMI

Steps:

1. Configure EC2 instance
2. Install required software
3. Create AMI
4. Launch new instance from AMI

Purpose:

Reusable infrastructure image.

---

## Lab 4 – Load Balancer

Steps:

1. Launch two EC2 instances
2. Install Nginx
3. Create Application Load Balancer
4. Register instances to target group
5. Test load balancing

---

## Lab 5 – Auto Scaling

Steps:

1. Create Launch Template
2. Create Auto Scaling Group
3. Attach Load Balancer
4. Configure scaling policies

Example:

CPU > 70% → Scale out
CPU < 30% → Scale in

---

# 📊 Monitoring

CloudWatch is used to monitor:

* CPU Utilization
* Network Traffic
* Disk Usage
* Instance Health

Alerts can be configured using **SNS notifications**.

---

# 🔐 Security Best Practices

* Use **IAM Roles instead of Access Keys**
* Restrict inbound traffic using **Security Groups**
* Use **private subnets for backend servers**
* Enable **CloudWatch monitoring**

---

# 🛠 Tools Used

* AWS EC2
* AWS VPC
* AWS IAM
* AWS CloudWatch
* AWS Load Balancer
* AWS Auto Scaling
* Linux (Ubuntu)
* Nginx
* Docker

---

# 🎯 Learning Outcome

After completing these labs you will understand:

* Real cloud infrastructure design
* High availability architecture
* EC2 production best practices
* Cloud security fundamentals
* Monitoring and scaling

---

# 👨‍💻 Author

Piyush
Cloud & DevOps Learner

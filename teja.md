
# 💻 AWS EC2 Instance Creation - Lab Guide

This guide will walk you through the steps to launch an Amazon EC2 (Elastic Compute Cloud) instance using the AWS Management Console.

---

## 🛠️ Prerequisites

- Active AWS account  
- Basic knowledge of AWS Management Console  
- Internet connection  

---

## 🚀 Step 1: Login to AWS Console

1. Visit [https://aws.amazon.com/console/](https://aws.amazon.com/console/) and log in with your credentials.  
![AWS Login Page](your-image-path/login.png)

---

## 🔍 Step 2: Search and Open EC2 Service

2. In the AWS Console, search for **EC2** in the search bar and click on it.  
![Search EC2 Service](your-image-path/search-ec2.png)

---

## 🖥️ Step 3: Launch a New EC2 Instance

3. Click on the **Launch Instance** button under the "Instances" section.  
![Launch EC2 Instance](your-image-path/launch-instance.png)

---

## 📄 Step 4: Name and OS Image

4. Give a name to your instance and select the Amazon Machine Image (AMI), such as **Amazon Linux 2** or **Ubuntu**.  
![Choose AMI](your-image-path/choose-ami.png)

---

## ⚙️ Step 5: Choose Instance Type

5. Select an instance type like **t2.micro** (eligible for free tier).  
![Choose Instance Type](your-image-path/instance-type.png)

---

## 🔐 Step 6: Create or Select Key Pair

6. Create a new key pair or select an existing one. Download the `.pem` file and store it safely.  
![Create Key Pair](your-image-path/key-pair.png)

---

## 🛡️ Step 7: Configure Network Settings

7. Ensure your instance is in the correct VPC and subnet. Allow SSH (port 22) in the security group settings.  
![Configure Network Settings](your-image-path/network-settings.png)

---

## 🗂️ Step 8: Storage Configuration

8. Use the default 8 GB General Purpose SSD or customize as per need.  
![Configure Storage](your-image-path/storage.png)

---

## ✅ Step 9: Review and Launch

9. Review all configurations and click **Launch Instance**.  
![Review and Launch](your-image-path/review-launch.png)

---

## 🔄 Step 10: Instance Status

10. Wait for the instance to enter **Running** state. Click on the instance ID to view details.  
![Instance Running](your-image-path/instance-running.png)

---

## 🔗 Step 11: Connect to Instance

11. Click on **Connect** and follow the SSH instructions. Use the downloaded `.pem` file and run the command in your terminal:

```bash
ssh -i "your-key.pem" ec2-user@your-public-ip

# Deployement_of_Windows_Server_AWS_EC2
"AWS EC2 website deployment"

## Description:
This project demonstrates how to deploy a **Windows Server** on an **AWS EC2 instance**. The instructions and resources provided will guide you through setting up a Windows Server instance, configuring security settings, and connecting to it using RDP (Remote Desktop Protocol).

## Prerequisites:
Before starting, make sure you have the following:
- An **AWS account**: You’ll need an account on AWS to create and manage EC2 instances.
- Basic knowledge of **AWS EC2** and **RDP** is recommended.
- **RDP client** (e.g., **Microsoft Remote Desktop** for Windows/Mac) or access to an EC2 instance through **SSH**.

## Setup Instructions:

### Step 1: **Create an EC2 Instance**
1. Log in to your **AWS Management Console**.
2. Go to **EC2 Dashboard** and click **Launch Instance**.
3. Choose the **Windows Server AMI** (Amazon Machine Image) for your instance.
4. Select the instance type, e.g., **t2.micro** (eligible for free tier).
5. Configure the instance settings (default settings are usually fine for testing).
6. In the **Security Group** settings, ensure that **RDP (TCP port 3389)** is open to allow remote access.
7. Review and launch the instance. Select or create a key pair to securely access your instance.

### Step 2: **Connect to the EC2 Instance**
1. After your EC2 instance is running, go to the **Instances** tab in the EC2 Dashboard.
2. Select your Windows Server instance and click **Connect**.
3. Follow the instructions to get your **Windows Administrator password** and connect to the instance via **RDP**.

### Step 3: **Configure Windows Server**
1. Once connected to your Windows instance, configure your server as needed.
2. Install any necessary updates, applications, or tools you require for your project.
3. Optionally, set up additional configurations like **static IP addresses**, **Windows Firewall rules**, or **domain settings**.

### Step 4: **(Optional) Automating with Scripts**
- If you have any scripts (e.g., PowerShell scripts) that help automate the setup of Windows Server or EC2 configurations, you can include them here. For example:
  - `setup.ps1`: A PowerShell script that installs necessary software and configurations on the server.

## Files:
- **setup.ps1**: PowerShell script for automated Windows Server setup.
- **config.json**: Configuration file for the EC2 instance (if applicable).
- **readme.md**: Documentation explaining the steps for deploying Windows Server on EC2.

## Troubleshooting:
- **Cannot connect via RDP**: Ensure that your EC2 security group allows **TCP port 3389** for inbound connections.
- **Windows Server not starting**: Check the instance status and logs in the **AWS Management Console**.
- **Windows password issue**: If you forgot your Windows password, you can use the EC2 Instance Connect feature or reset the password through the EC2 console.







## Introduction
Amazon Elastic Compute Cloud (EC2) is a web service that provides resizable compute capacity in the cloud. This document outlines the steps to create an EC2 instance in AWS.

## Prerequisites
- An active AWS account
- AWS Management Console access

## Steps to Create an EC2 Instance

1. **Log in to the AWS Management Console**  
   a. Go to the AWS Management Console  
   b. Enter your credentials to log in.

2. **Navigate to EC2 Dashboard**  
   a. In the AWS Management Console, search for "EC2" in the services search bar.  
   b. Click on EC2 to open the EC2 Dashboard.

3. **Launch Instance**  
   a. Click on the Launch Instance button.

4. **Choose an Amazon Machine Image (AMI)**  
   a. Select an AMI from the list.  
   b. Click **Select**.

5. **Choose an Instance Type**  
   a. Choose an instance type.  
   b. Click **Next: Configure Instance Details**.

6. **Configure Instance Details**  
   a. Set the number of instances (default is 1).  
   b. Configure any additional settings as needed (VPC, subnet, etc.).  
   c. Click **Next: Add Storage**.

7. **Add Storage**  
   a. Adjust the size and type of storage if necessary.  
   b. Click **Next: Add Tags**.

8. **Configure Security Group**  
   a. Create a new security group or select an existing one.  
   b. Add rules to allow inbound traffic.  
   c. Click **Review and Launch**.

9. **Review Instance Launch**  
   a. Review your instance configuration.  
   b. Click **Launch**.

10. **Select a Key Pair**  
    a. Select an existing key pair or create a new one.  
    b. Download the key pair (`.pem` file) and keep it secure.  
    c. Check the acknowledgment box and click **Launch Instances**.

11. **Access Your EC2 Instance**  
    a. Once the instance is running, go back to the EC2 dashboard.  
    b. Select your instance and note the Public IP or Public DNS.  
    c. Connect to your instance using SSH:  
    ```bash
    ssh -i /path/to/your-key.pem ec2-user@your-public-ip
    ```

## Additional Link
[Amazon EC2 Documentation](https://aws.amazon.com/ec2/)

# AWS CloudFormation Automation Lab 

<div style="display: flex; justify-content: center; gap: 15px;">
  <img src="https://github.com/user-attachments/assets/a5c6eb07-013f-4968-9f51-d7373c692bd3" width="200">
  <img src="https://github.com/user-attachments/assets/380d7074-9813-4ebc-8cbb-933b1f8db22f" width="200">
  <img src="https://github.com/user-attachments/assets/bd55efb3-9cb2-4c58-bc08-eb2acfd6a30a" width="200">
</div>

## Overview

This project demonstrates the use of AWS CloudFormation to automate the deployment of AWS infrastructure. The lab consists of multiple CloudFormation templates (`.yaml` files) that define and deploy a Virtual Private Cloud (VPC), Security Groups, an S3 Bucket, and an EC2 instance.

By using Infrastructure as Code (IaC), this project ensures that AWS resources are deployed consistently, efficiently, and in a repeatable manner.

## Features

- **Automated Infrastructure Deployment**: Deploys AWS resources using CloudFormation templates.
- **VPC & Security Group Setup**: Defines network architecture for secure resource communication.
- **Amazon S3 Bucket Creation**: Adds object storage capabilities.
- **Amazon EC2 Instance Deployment**: Launches an instance using a predefined AMI.
- **Stack Updates & Deletion**: Demonstrates how to modify and remove deployed infrastructure.

## Files in This Repository

- `task1.yaml` - Deploys a VPC and Security Group.
- `task2.yaml` - Updates the stack by adding an Amazon S3 Bucket.
- `task3.yaml` - Further updates the stack by adding an EC2 instance.

## Prerequisites

Before using these CloudFormation templates, ensure you have:
- An AWS account with necessary permissions to create CloudFormation stacks.
- AWS CloudFormation enabled in your selected region.
- Basic knowledge of AWS services such as VPC, EC2, and S3.

## Deployment Instructions

### Step 1: Deploy Initial Stack
1. Log in to AWS Management Console.
2. Navigate to **AWS CloudFormation** service.
3. Click **Create Stack** > **With new resources**.
4. Select **Upload a template file**, then choose `task1.yaml`.
5. Click **Next**, enter `Lab` as the stack name.
6. Click **Next** through remaining screens and click **Create Stack**.
7. Wait for the stack status to change to **CREATE_COMPLETE**.

### Step 2: Update Stack with S3 Bucket
1. Open AWS CloudFormation, select the **Lab** stack.
2. Click **Update** > **Replace current template**.
3. Upload `task2.yaml`, then click **Next**.
4. Follow prompts and click **Update Stack**.
5. Wait for status to change to **UPDATE_COMPLETE**.

### Step 3: Update Stack with EC2 Instance
1. Open AWS CloudFormation, select **Lab** stack.
2. Click **Update** > **Replace current template**.
3. Upload `task3.yaml`, then click **Next**.
4. Follow prompts and click **Update Stack**.
5. Wait for **UPDATE_COMPLETE** status.

### Step 4: Delete the Stack
1. Open AWS CloudFormation, select the **Lab** stack.
2. Click **Delete**, then confirm deletion.
3. Wait until the stack is completely removed.

## Future Enhancements
- Add support for AWS Lambda and DynamoDB.
- Automate stack deployment using AWS CLI or Terraform.
- Implement monitoring with AWS CloudWatch.

## License
This project is open-source and available under the [MIT License](LICENSE).




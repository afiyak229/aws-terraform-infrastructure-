AWS Terraform Infrastructure
Overview

This repository contains Terraform configuration files to provision AWS infrastructure. It sets up a Virtual Private Cloud (VPC), EC2 instances, S3 buckets, and an RDS database. The project demonstrates Infrastructure as Code (IaC) principles using Terraform to automate the creation and management of cloud resources.
Project Architecture

This Terraform configuration provisions the following AWS resources:

    VPC (Virtual Private Cloud): Creates an isolated network for your infrastructure.
    EC2 Instance: Launches a virtual machine to host applications.
    S3 Bucket: Provides scalable object storage.
    RDS (Relational Database Service): Sets up a MySQL database.

Features

    Reusable and modular Terraform configuration.
    Automated deployment with GitHub Actions CI/CD pipeline.
    Outputs important infrastructure information (e.g., EC2 public IP).
    Easy to customize for different regions, instance types, or scaling needs.


Getting Started
Prerequisites

Before you begin, ensure you have the following installed:

    Terraform CLI
    AWS CLI
    Git

AWS Credentials

Make sure your AWS credentials are configured locally. You can configure them using the AWS CLI:
aws configure

Clone the Repository :
git clone https://github.com/yourusername/aws-terraform-infrastructure.git
cd aws-terraform-infrastructure/infrastructure


Usage
1. Initialize Terraform
Run the following command to initialize the Terraform environment and download required providers:
terraform init

2. Review the Terraform Plan
This step allows you to review the resources that Terraform will create:
terraform plan

3. Apply the Configuration
Apply the changes to provision the infrastructure on AWS:
terraform apply
You will be prompted to confirm the execution. Type yes to proceed.

4. Outputs
Once the infrastructure is provisioned, you will see output values such as the public IP address of the EC2 instance. You can also find the output information by running:
terraform output

5.Clean Up
To destroy all the resources created by this project, run:
terraform destroy

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

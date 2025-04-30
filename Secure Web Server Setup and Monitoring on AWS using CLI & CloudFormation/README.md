# Secure Web Server Setup and Monitoring on AWS using CLI & CloudFormation

This project demonstrates how to automate the deployment of a secure web server on AWS using **CloudFormation** and set up monitoring via **AWS CLI and CloudTrail**.

## Project Objective
Build a secure, scalable web server environment using:
- **AWS CloudFormation** for infrastructure provisioning
- **AWS CLI** for monitoring setup
- **CloudTrail** for API activity logging
- **Amazon S3** for log storage

## Infrastructure Setup (CloudFormation)
The infrastructure includes:
- **VPC** with public and private subnets
- **EC2 instance** running Apache HTTP server
- **Security Group** for SSH (port 22) and HTTP (port 80)

## Monitoring Setup (AWS CLI)
Steps to enable **CloudTrail** logging:
1. Create an S3 bucket for logs
2. Attach bucket policy for CloudTrail
3. Set up a CloudTrail trail to log AWS API activity

## Project Structure
.
├── infrastructure.yaml        # CloudFormation template
├── monitoring.sh              # AWS CLI script for CloudTrail
├── bucket-policy.json         # S3 bucket policy
└── README.md                  # Documentation

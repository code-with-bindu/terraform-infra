# Terraform Infrastructure as Code

## Project Overview
An Infrastructure as Code (IaC) project using Terraform that 
automatically provisions development and production cloud 
environment configurations — simulating real AWS infrastructure.

## Features
- Auto-generates Dev & Prod environment configs
- Simulates AWS infrastructure setup
- Auto-scaling configuration (1-5 dev, 3-20 prod)
- PostgreSQL database configuration
- S3 storage setup
- Automated infrastructure report generation

## 🛠️ Tech Stack
- Terraform
- HashiCorp Configuration Language (HCL)
- Local Provider

## 📁 Infrastructure Created
- infrastructure/dev/config.json → Development environment
- infrastructure/prod/config.json → Production environment  
- infrastructure/report.md → Auto-generated report

## ▶️ How to Run
1. Install Terraform
2. Clone this repository
3. Run: terraform init
4. Run: terraform apply
5. Type 'yes' to confirm
6. Check infrastructure/ folder for generated files

## 💡 Real World Use Case
In production, this same code would automatically create:
- AWS EC2 instances
- RDS PostgreSQL databases
- S3 storage buckets
- Auto-scaling groups
- All with one command!

## 🌍 Environments
| Environment | Instance | Min | Max |
|---|---|---|---|
| Development | t2.micro | 1 | 5 |
| Production | t3.large | 3 | 20 |

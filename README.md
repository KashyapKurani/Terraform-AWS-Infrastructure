🚀 Terraform AWS Infrastructure (VPC → EC2)
📌 Overview

This project demonstrates Infrastructure as Code (IaC) using Terraform to provision a complete AWS environment including networking and compute resources.

It builds a production-style AWS setup from scratch:

VPC
Public Subnet
Internet Gateway
Route Table
Security Group
EC2 Instance
🏗️ Architecture
Internet
   │
Internet Gateway
   │
Route Table
   │
Public Subnet
   │
EC2 Instance
   │
Security Group
⚙️ Tech Stack
Terraform
AWS (EC2, VPC, Subnets, IGW, Route Tables, Security Groups)
AWS CLI
Linux (Ubuntu)
Git & GitHub
📁 Project Structure
Terraform-AWS-Infrastructure/
│
├── provider.tf
├── variables.tf
├── main.tf
├── outputs.tf
├── terraform.tfvars
├── .gitignore
│
└── screenshots/
    ├── terraform-init.png
    ├── terraform-plan.png
    ├── terraform-apply.png
    ├── vpc-created.png
    ├── subnet-created.png
    ├── ec2-created.png
🚀 Features

✔ Infrastructure as Code using Terraform
✔ Modular AWS networking setup
✔ Public EC2 deployment
✔ Internet access enabled via IGW
✔ Security Group with SSH & HTTP access
✔ Clean variable-driven configuration

🧠 What I Learned
AWS VPC networking (subnets, routing, IGW)
Terraform lifecycle (init, plan, apply, destroy)
State management in Terraform
Security Groups and inbound/outbound rules
Infrastructure automation using IaC principles
🛠️ Setup & Deployment
1. Clone Repo
git clone <your-repo-url>
cd Terraform-AWS-Infrastructure
2. Initialize Terraform
terraform init
3. Validate Configuration
terraform validate
4. Preview Changes
terraform plan
5. Deploy Infrastructure
terraform apply

Type:

yes
6. Destroy Resources (Important)
terraform destroy
📦 Key Terraform Resources Used
aws_vpc
aws_subnet
aws_internet_gateway
aws_route_table
aws_route_table_association
aws_security_group
aws_instance
🔐 Security Notes
SSH is open for learning purposes (0.0.0.0/0)
In production, restrict SSH access to your IP only
📸 Screenshots

Add your screenshots in the /screenshots folder:

Terraform Init
Terraform Plan
Terraform Apply
AWS Console (VPC, EC2, Subnet)
📊 Outputs

After deployment:

EC2 Public IP
EC2 Public DNS
Instance ID
🎯 Outcome

Successfully built a complete AWS infrastructure using Terraform demonstrating real-world DevOps practices.

👨‍💻 Author

Kashyap Kurani
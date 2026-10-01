# AWS VPC Infrastructure using Terraform

## 📌 Project Overview

This project demonstrates how to provision a complete **AWS VPC infrastructure using Terraform**.

The infrastructure is created using **Terraform Modules** to keep the configuration reusable, organized, and maintainable.

## 🏗️ Architecture

The project creates the following AWS resources:

* VPC
* Internet Gateway
* 3 Public Subnets
* 3 Private Subnets
* Public Route Table
* Private Route Table
* Route Table Associations
* NAT Gateway
* Elastic IP for NAT Gateway

## 🛠️ Technologies Used

* **Terraform**
* **Amazon Web Services (AWS)**
* **AWS VPC**
* **AWS EC2**
* **AWS IAM**
* **Git & GitHub**

## 📂 Project Structure

```text
terraform-vpc-project/
│
├── environments/
│   └── networking/
│       └── VPC/
│           └── dev/
│               ├── backend.tf
│               ├── main.tf
│               ├── provider.tf
│               ├── variables.tf
│               ├── terraform.tfvars
│               └── output.tf
│
├── modules/
│   └── networking/
│       └── VPC/
│           ├── main.tf
│           ├── provider.tf
│           ├── variables.tf
│           └── output.tf
│
├── screenshort/
│   ├── vpc.png
│   ├── Public Subnet.png
│   └── Private Subnet.png
│
└── .gitignore
```

## ⚙️ How to Deploy

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
cd terraform-vpc-project
```

### 2. Navigate to the development environment

```bash
cd environments/networking/VPC/dev
```

### 3. Initialize Terraform

```bash
terraform init
```

### 4. Validate the configuration

```bash
terraform validate
```

### 5. Review the execution plan

```bash
terraform plan
```

### 6. Apply the infrastructure

```bash
terraform apply
```

Enter `yes` when prompted.

## 🧹 Destroy Infrastructure

To remove the resources created by Terraform:

```bash
terraform destroy
```

Enter `yes` when prompted.

## 📸 Screenshots

Screenshots of the Terraform EC2 deployment are included in the `screenshort` folder.

## 🎯 Learning Outcomes

Through this project, I learned:

* Creating AWS infrastructure using Terraform
* Working with Terraform modules
* Creating VPC networking components
* Configuring public and private subnets
* Working with route tables and associations
* Configuring Internet Gateway and NAT Gateway
* Managing Terraform variables and outputs
* Structuring Terraform projects using environments and modules
* Using Git and GitHub for infrastructure code

## 👩‍💻 Author

**Sakshi Repale**

Information Technology Engineering Student
Cloud Computing | AWS | Linux | Terraform | DevOps

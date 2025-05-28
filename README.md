# Terraform AWS Assignment

This project is created using **Terraform** to automate AWS infrastructure setup.

---

##  What I Understood in My Words:

Using Terraform, I understood how we can **write code (in .tf files)** to create and manage AWS resources like:

- EC2 (virtual servers)
- EBS (storage)
- VPC (network)
- Security groups (firewall rules)
- Load Balancer (to distribute traffic)
- Auto Scaling (automatic server increase/decrease)

Instead of doing everything manually from AWS Console, I learned how to do it all just by running **terraform commands**. That’s the real power of **Infrastructure as Code (IaC)**.

---

## What this Terraform Code Does:

- Creates a **custom VPC** with subnets
- Launches **EC2 instances**
- Attaches **EBS volumes** to EC2
- Sets up **Security Groups** (firewall rules)
- Creates an **Application Load Balancer (ALB)**
- Enables **Auto Scaling** (more EC2s on demand)
- Displays useful outputs like **EC2 IP** and **ALB DNS name**

---

##  Terraform File Summary:

| File               | Description                                 |
|--------------------|---------------------------------------------|
| `main.tf`          | Connects all Terraform modules              |
| `vpc.tf`           | Creates VPC, subnets                        |
| `ec2.tf`           | Launches EC2 instances                      |
| `ebs.tf`           | Adds storage to EC2                         |
| `security_groups.tf`| Sets firewall rules                       |
| `alb.tf`           | Sets up Application Load Balancer          |
| `autoscale.tf`     | Configures Auto Scaling                     |
| `variables.tf`     | Defines variables used in code              |
| `terraform.tfvars` | Actual values for those variables           |
| `outputs.tf`       | Prints output like EC2 IP, ALB URL          |

---

##  Requirements:

- AWS account with access keys
- Terraform installed on your system
- AWS CLI configured (`aws configure`)

---

## How to Run:

```bash
terraform init     # Initialize Terraform
terraform plan     # Preview what will be created
terraform apply    # Create all AWS resources
terraform destroy  # Delete all created resources (optional)

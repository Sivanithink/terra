# ✅ Terraform AWS Assignment

This project uses **Terraform** to set up a basic AWS infrastructure.

##  What it does:

- Creates a **VPC** (your own network)
- Launches **EC2 instances** (virtual machines)
- Attaches **EBS volumes** (extra storage for EC2)
- Adds **Security Groups** (firewall rules)
- Creates an **Application Load Balancer (ALB)** (to manage traffic)
- Sets up **Auto Scaling** (automatically increases or decreases EC2s)
- Shows output like public IPs and ALB DNS name

---

## 📁 Main Files:

| File               | Description                                 |
|--------------------|---------------------------------------------|
| `main.tf`          | Entry file that connects all resources      |
| `vpc.tf`           | Creates the VPC and subnets                 |
| `ec2.tf`           | Launches EC2 instances                      |
| `ebs.tf`           | Adds storage to EC2                         |
| `security_groups.tf`| Firewall rules                             |
| `alb.tf`           | Sets up the ALB                             |
| `autoscale.tf`     | Enables Auto Scaling                        |
| `variables.tf`     | Stores variable names                       |
| `terraform.tfvars` | Stores actual values for the variables      |
| `outputs.tf`       | Prints useful output like IP and URL        |

---

## 🚀 How to Use:

1. Open terminal in this folder  
2. Run these commands one by one:

```bash
terraform init     # Sets up Terraform
terraform plan     # Shows what will be created
terraform apply    # Creates the AWS resources
terraform destroy  # (Optional) Deletes everything

# Terraform AWS Bootstrap Project

This project bootstraps the required AWS infrastructure for managing Terraform state securely.

## 📦 What It Does

- Creates an **S3 Bucket** to store Terraform state.
- Creates a **DynamoDB Table** to lock the state and avoid conflicts.

## 📁 Files

- `main.tf`: Defines the AWS S3 bucket and DynamoDB table resources.
- `variables.tf`: Input variables for bucket name, table name, etc.
- `terraform.tfvars`: Values for the variables.
- `provider.tf`: AWS provider setup.
- `outputs.tf`: Outputs created resources.

## 🚀 Getting Started

1. Ensure you have [AWS CLI configured](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html) or set up manually via `~/.aws/credentials` and `~/.aws/config`.

2. Run:

```bash
terraform init
terraform plan
terraform apply

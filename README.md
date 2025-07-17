# Terraform-custom-vpc-subnets
This project uses Terraform to provision custom VPC with multiple public subnets in AWS.

Features:
1.Creates a custom VPC
2.Creates multiple subnets using count
3.Distributes subnets across available AWS Availability Zones
4.Uses cidrsubnet() to dynamically calculate subnet CIDRs

Key Concepts:
1.count for resource replication
2.cidrsubnet() for IP range management
3.data.aws_availability_zones to fetch dynamic zone names
4.Outputs to extract useful info like subnet IDs or VPC ID
5 .gitignore for Terraform-specific best practices

main.tf: Core infrastructure logic
outputs.tf: Exports key values like VPC/Subnet IDs
.gitignore: Prevents committing .terraform/, state files, secrets

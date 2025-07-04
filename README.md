Here is a professional README.md file based on the provided Terraform code files:

**Overview**

This Terraform infrastructure configuration creates a basic AWS VPC with a public subnet. The VPC and subnet are defined with default values for the AWS region, VPC CIDR block, public subnet CIDR block, and availability zone.

**Key Resources**

* `aws_vpc.main`: Creates a VPC with the specified CIDR block and tags.
* `aws_subnet.public`: Creates a public subnet within the VPC with the specified CIDR block and availability zone.

**Variables**

* `aws_region`: The AWS region to deploy to (default: `us-west-2`).
* `vpc_cidr`: The CIDR block for the VPC (default: `10.0.0.0/16`).
* `public_subnet_cidr`: The CIDR block for the public subnet (default: `10.0.1.0/24`).
* `availability_zone`: The availability zone for the subnet (default: `us-west-2a`).

**How to Use**

1. Install Terraform on your machine if you haven't already.
2. Create a new directory for your project and navigate to it.
3. Create a file named `terraform.tf` and copy the contents of the `provider.tf`, `main.tf`, and `variables.tf` files into it.
4. Create a file named `variables.tf` in the same directory and update the default values of the variables if needed.
5. Run `terraform init` to initialize the Terraform working directory.
6. Run `terraform apply` to apply the configuration and create the AWS resources.

**Important Notes**

* This configuration assumes that you have the AWS CLI installed and configured on your machine.
* Be sure to update the `aws_region` variable to match the region you intend to deploy to.
* If you want to change the default values of the other variables, update the `variables.tf` file accordingly.
* This configuration only creates a basic VPC and public subnet. You will need to add additional resources and configurations to create a fully functional infrastructure.
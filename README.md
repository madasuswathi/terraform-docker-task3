
# DevOps Task 3: Infrastructure as Code with Terraform

## Objective
Provision a local Docker container using Terraform.

## Tools Used
- Terraform
- Docker
- Ubuntu Linux
- Git and GitHub

## Project Overview
This project uses Terraform and the Docker provider to download
the Apache HTTP Server image and create a Docker container
named `terraform-apache`.

The container maps port 8086 on the Ubuntu VM to port 80
inside the container.

## Project Structure
- `main.tf` - Terraform configuration
- `.gitignore` - Excludes local state and generated files
- `.terraform.lock.hcl` - Provider dependency lock file
- `logs/` - Execution logs

## Implementation Steps
1. Initialize Terraform using `terraform init`.
2. Format the configuration using `terraform fmt`.
3. Validate the configuration using `terraform validate`.
4. Preview changes using `terraform plan`.
5. Create resources using `terraform apply`.
6. Verify the container using `docker ps`.
7. Test Apache using `curl http://localhost:8086`.
8. Inspect resources using `terraform state list`.
9. Inspect container details using `terraform state show docker_container.apache`.
10. Remove resources using `terraform destroy`.

## Expected Outcome
- Terraform initializes and validates successfully.
- The Apache Docker image and container are provisioned.
- The Apache HTTP response is verified.
- Terraform state is inspected.
- The container and managed infrastructure are destroyed.

## Execution Evidence
Execution logs are stored in the `logs/` directory.
They provide evidence of Terraform planning, deployment,
state inspection, container verification, and cleanup.

## Learning Outcomes
- Infrastructure as Code (IaC)
- Terraform providers and resources
- Terraform plan and apply
- Resource dependencies
- Terraform state management
- Infrastructure cleanup


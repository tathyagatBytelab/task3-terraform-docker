#  Task 3 - Infrastructure as Code (IaC) with Terraform

## Objective
Provision a local Docker container using **Terraform** to understand and implement Infrastructure as Code (IaC) concepts.

## 🛠️ Tools Used
- Terraform v1.12.2
- Docker v27.5.1
- OS: Ubuntu

## 📁 Files in this Repository
```
| File                     | Purpose                                        |
|--------------------------|------------------------------------------------|
| `main.tf`                | Terraform code to provision NGINX container   |
| `terraform_logs.txt`     | Logs from `init`, `plan`, `apply`, `destroy`  |
| `terraform.tfstate`      | Terraform state file (auto-generated)         |
| `terraform.tfstate.backup` | Backup of state file                        |
| `ngnix_screenshot.png`   | Screenshot of running NGINX in browser        |
| `README.md`              | This documentation                           |

```
## 📝 Task Steps

###  1️⃣ Initialize Terraform
```bash
terraform init

###  2️⃣ Review the execution plan
'''bash
terraform plan

###  3️⃣ Apply the configuration
'''bash
terraform apply
- This will pull the nginx:latest Docker image

- It will create a container named nginx-container running on port 8090

- Accessible at: http://localhost:8090


###  4️⃣ Destroy the infrastructure after testing
'''bash
terraform destroy


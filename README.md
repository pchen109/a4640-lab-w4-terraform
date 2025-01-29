# 4640-w4-lab-start-w25
## General Setup
1. **Clone the repository** to your local machine.
2. **Ensure you have the following installed and setup**:
    - Install [Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli).
    - Install [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html).
    - Connect to AWS derver with `aws configure` with your Access Key ID and Secret Access Key. 
3. **Initialize, Format, Plan and Apply Terraform**
    - Run
    ```bash
    terraform init
    terraform fmt
    terraform plan -out=tfplan
    terraform apply tfplan
    ```
4. **Destroy the infrastructuer** (if needed):
    - Run
    ```bash
    terraform destroy
    ```
## SSH Key Pair Creation
1. **Generate a new SSH key pair**
    - Run
    ```bash
    ssh-keygen -t rsa -b 2048 -f ~/.ssh/aws_key
    ```
2. **Add the public key to the cloud-config.yaml file**

## Note
- Hostname is set to web in the cloud-config.yaml.
- Public IP and DNS will be displayed in the console after a successful terraform apply.
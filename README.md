# Dev Environment Deployment Automation

This project automates the deployment of a development environment using Terraform and Ansible.

## Prerequisites

- [Terraform](https://www.terraform.io/downloads.html) installed
- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) installed
- Access to the necessary cloud provider (e.g., AWS, Azure, GCP)

## Setup

1. Clone the repository:
    ```sh
    git clone https://github.com/louieb117/DevDeploymentAutomation.git
    cd DevDeploymentAutomation
    ```

2. Configure your Terraform variables:
    ```sh
    cp terraform.tfvars.example terraform.tfvars
    # Edit terraform.tfvars with your cloud provider credentials and settings
    ```

3. Initialize Terraform:
    ```sh
    terraform init
    ```

4. Apply Terraform configuration to provision infrastructure:
    ```sh
    terraform apply
    ```

5. Run Ansible playbooks to configure the environment:
    ```sh
    ansible-playbook -i inventory playbook.yml
    ```

## Usage

- To update the infrastructure, modify the Terraform configuration and run `terraform apply` again.
- To reconfigure the environment, modify the Ansible playbooks and run `ansible-playbook` again.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
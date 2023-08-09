# Pipeline_yam_code_to_publish_private_dns_zone_to_azure_artifacts
Using this techhub template we can publish private dns zone module to azure artifacts using yaml code

## Prerequisites

Before you can use this Terraform module, you will need to have the following installed:

- [Terraform](https://www.terraform.io/downloads.html) - v1.0.5 or later
- [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli) - v2.26.0 or later

You will also need to have an Azure azurerm_billing_enrollment_account_scope. 

## Usage

To use this Terraform module, follow these steps:

From your local, generate and Set up SSH key pair for Github.

Clone this Git repo to your local machine.

```bash
git@github.com:NashTech-Labs/Pipeline_yam_code_to_publish_private_dns_zone_to_azure_artifacts.git

```

Change into the directory containing the module.

```bash
cd module

```

Initialize Terraform in the directory.

```bash
terraform init
```
```bash
terraform plan
```
```bash
terraform apply
```


## for publishing this terraform module to the azure artifact you need to follow these steps
1. Go to the Azure DevOps
2. create the new pipeline where you need to choose the existing pipeline and specify the path of your yaml file
3. Run the pipeline with the desired version of your module(you need to change your version in the metadata.yaml)

# Add Users to IBM Cloud Access Groups module

:warning: This module is no longer maintained. Please use [terraform-ibm-iam-access-group](https://github.com/terraform-ibm-modules/terraform-ibm-monitoring-agent) for managing IBM Cloud access groups.

Module to add (already invited) users to existing IBM Cloud access groups.

## Software dependencies

The module depends on the following software components:

### Command-line tools

- terraform - v12

### Terraform providers

- IBM Cloud provider >= 1.5.3

## Module dependencies

None

## Example usage

```hcl-terraform
module "dev_tools_argocd" {
  source = "github.com/ibm-garage-cloud/terraform-ibm-add-access-group-users.git?ref=v1.0.0"

  users = "user@somewhere.com,user@elsewhere.com"
  access_groups = "group1,group2"
}
```


# Reusable Github Actions Workflows For Homelab Repos

This repo contains a collection of reusable Github Actions workflows that are used in the Knighten-Homelab collection of repos. These workflows are sets of common tasks that can be reused across multiple repositories, making it easier to maintain and update them..

## Workflows

### [Ansible Lint](.github/workflows/ansible-lint.yaml)

Runs Ansible Lint on the repo to check for best practices and potential issues in Ansible playbooks.

#### Inputs
- `runs-on`: The type of runner to use for the job. Default is `github-arc-runners`.
- `ansible-directory`: The directory containing the Ansible playbooks. Default is `ansible`.
- `ref`: The git reference to checkout. Default is current workflow execution branch.

### [Get Latest GitHub Repo Tag](.github/workflows/github-get-latest-repo-tag.yaml)

Retrieves the latest tag from the current GitHub repository.

#### Inputs
- `runs-on`: The type of runner to use for the job. Default is `github-arc-runners`.

#### Outputs
- `latest-tag`: The latest tag from the current GitHub repository.

### [Semantic Release to GitHub](.github/workflows/semantic-release-to-gh.yaml)

Runs semantic release on the repo to automatically version and publish/release the package to GitHub.

#### Inputs
- `runs-on`: The type of runner to use for the job. Default is `github-arc-runners`.


### [Terraform Apply and Deploy App Via AWX](.github/workflows/terraform-apply-and-deploy-app-via-awx.yaml)

Runs Terraform apply to create infrastructure, creates AWX resources via an Ansible playbook, and deploys the app using the AWX API.

#### Inputs
- `runs-on`: The type of runner to use for the job. Default is `github-arc-runners`.
- `infra-directory`: The directory containing the Terraform configuration files. Default is `infra`.
- `ansible-directory`: The directory containing the Ansible playbooks. Default is `ansible`.
- `environment`: The environment to deploy to. Default is `test`.
- `awx-resource-creation-playbook`: The Ansible playbook used to create AWX resources.
- `awx-deploy-template-name:`: The name of the AWX job template used to deploy the app.
- `ref`: The git reference to checkout. Default is current workflow execution branch.

#### Secrets
- `VAULT_URL`: The URL of the HashiCorp Vault instance.
- `VAULT_TOKEN`: The token used to authenticate with the HashiCorp Vault instance.

### [Terraform Destroy and Uninstall App Via AWX](.github/workflows/terraform-destroy-and-app-cleanup-via-awx.yaml)

Runs Terraform destroy to remove infrastructure, uninstalls the app using the AWX API, and deletes AWX resources.

#### Inputs
- `runs-on`: The type of runner to use for the job. Default is `github-arc-runners`.
- `infra-directory`: The directory containing the Terraform configuration files. Default is `infra`.
- `ansible-directory`: The directory containing the Ansible playbooks. Default is `ansible`.
- `environment`: The environment to deploy to. Default is `test`.
- `awx-resource-creation-playbook`: The Ansible playbook used to create AWX resources.
- `awx-deploy-template-name:`: The name of the AWX job template used to deploy the app.
- `ref`: The git reference to checkout. Default is current workflow execution branch.

#### Secrets
- `VAULT_URL`: The URL of the HashiCorp Vault instance.
- `VAULT_TOKEN`: The token used to authenticate with the HashiCorp Vault instance.

### [Terraform Lint and Security Scan](.github/workflows/terraform-lint-and-security-scan.yaml)

Runs Terraform lint and security scan (Trivy) on the repo to check for best practices and potential issues in Terraform configuration files.

#### Inputs
- `runs-on`: The type of runner to use for the job. Default is `github-arc-runners`.
- `infra-directory`: The directory containing the Terraform configuration files. Default is `infra`.
- `ref`: The git reference to checkout. Default is current workflow execution branch.

### [Execute AWX Resource Playbook](.github/workflows/awx-resource-playbook-execution.yaml)

Runs an Ansible playbook to create, delete or modify AWX resources. At a high level the awx.awx collection is installed and then the specified playbook is called with the required AWX connection and authentication info.

Note: the `environment` input variable is used to read from a variable file that is stored in  `{{ ansible-directory }}/envs`. The variable file is named `{{ environment }}.yaml` and is used to set the required variables for the playbook execution.

#### Inputs
- `runs-on`: The type of runner to use for the job. Default is `github-arc-runners`.
- `ansible-directory`: The directory containing the Ansible playbooks. Default is `ansible`.
- `environment`: The environment to deploy to. Default is `test`.
- `awx-resource-playbook`: The Ansible playbook used to create AWX resources.
- `ref`: The git reference to checkout. Default is current workflow execution branch.

#### Secrets
- `VAULT_URL`: The URL of the HashiCorp Vault instance.
- `VAULT_TOKEN`: The token used to authenticate with the HashiCorp Vault instance.

### [Launch AWX Job Template](.github/workflows/awx-launch-job-template.yaml)

Launches an AWX job template using the AWX API.

#### Inputs
- `runs-on`: The type of runner to use for the job. Default is `github-arc-runners`.
- `awx-job-template-name`: The name of the AWX job template to launch.

#### Secrets
- `VAULT_URL`: The URL of the HashiCorp Vault instance.
- `VAULT_TOKEN`: The token used to authenticate with the HashiCorp Vault instance.

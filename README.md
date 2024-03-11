# fem-eci-terraform-github

## Running `terraform plan` the first time

Run the following commands to tell Terraform that the repos were created outside the state:

```bash
$ doppler run -- terraform import 'module.repository["fem-eci-terraform-github"].github_repository.self' 'fem-eci-terraform-github'
$ doppler run -- terraform import 'module.repository["fem-eci-terraform-tfe"].github_repository.self' 'fem-eci-terraform-tfe'
```

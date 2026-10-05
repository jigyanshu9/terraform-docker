# terraform-docker
Provisions a local nginx Docker container using Terraform's Docker provider.

## Steps
1. `terraform init`
2. `terraform plan`
3. `terraform apply`
4. `terraform state list` / `terraform state show docker_container.nginx`
5. `terraform destroy`

## Notes
- Container: `tf-nginx` (nginx:latest), host port 8888 mapped to 80.
- Port 8080 was already in use by a Java service on the host, so 8888 was used.
- Logs are in `logs/`, screenshots in `screenshots/`.

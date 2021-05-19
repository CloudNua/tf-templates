# Gitlab CI Templates:

## Application CI / CD Template(s):

```
├── build.gitlab-ci.yml     # Docker Image Factory): Build and Release to Gitlab Container Registry
├── deploy.gitlab-ci.yml    # Deploy pre-build docker container via Helm Chart
├── test-py-1.gitlab-ci.yml # Python App Tests: Basic Pylint
└── test-py-2.gitlab-ci.yml # Python App Tests: Advanced analysis via Flake8, Pylint, UniTest
```

## Infrastructure CI / CD Template(s)

```
├── terraform.gitlab-ci.yml
```

### Terraform CI / CD Stages

- terraform init
- terraform validate
- terraform fmt -check
- terraform plan
- terraform apply
- terraform destroy


### Cluster Management (Applications & Services)
- Ingress
- Cert Manager (incl. letsEncryptClusterIssuer)
- GitLab Runner
- Prometheus
# Ismet Xani

### DevOps | Cloud | Infrastructure Engineering

New York, NY | [LinkedIn](https://www.linkedin.com/in/ismet-xani-003201395)

Economic Engineering graduate and LSU DevOps Engineer Certificate holder building hands-on projects in service monitoring, containerization, CI/CD, and infrastructure automation.

Seeking entry-level DevOps, Cloud Operations, Infrastructure, and Software Engineering opportunities. Authorized to work in the United States without sponsorship.

## Featured projects

### [CloudOps Observatory](https://github.com/ismet1292-wq/cloudops-observatory)

An AI-assisted Python monitoring application validated locally, in Minikube,
and in a temporary Terraform-managed AWS demonstration.

- HTTP health checks, response latency, and incident tracking.
- SQLite persistence and a service-status dashboard.
- 12 passing automated tests and GitHub Actions CI.
- Docker containers verified to run as a non-root user.
- Local Minikube deployment with persistent storage.
- Verified incident persistence after Kubernetes pod replacement.
- Public GHCR container releases with latest and commit-SHA tags.
- AWS incident recovery and history persistence after container replacement and a real host reboot.
- Verified deletion of the temporary EC2 host, disks, and host IAM resources after the demonstration.

The AWS network foundation remains; the temporary application host was removed.
This is a portfolio demonstration, not an ongoing production cloud service.
[AWS results and evidence](https://github.com/ismet1292-wq/cloudops-observatory/blob/main/docs/AWS_DEMO_RESULTS.md).

### [Dockerized Node.js application](https://github.com/ismet1292-wq/01-docker-node-app)

Node.js HTTP tests and a real Docker smoke test verify health, a non-root user,
read-only filesystem, and loopback-only publication on a disposable CI runner.

### [Terraform AWS infrastructure](https://github.com/ismet1292-wq/02-terraform-aws-infrastructure)

Eight network resources deployed and verified in AWS, with no drift in a
follow-up Terraform plan. A temporary EC2 host passed health, encrypted-disk,
IMDSv2 and SSM registration checks, then the host, disk and host IAM resources
were removed. The network remains; no application was installed in this project.
[Deployment evidence](https://github.com/ismet1292-wq/02-terraform-aws-infrastructure/blob/main/docs/DEPLOYMENT_RESULTS.md).

### [Ansible server configuration](https://github.com/ismet1292-wq/03-ansible-server-configuration)

Nginx configuration tested on a disposable Ubuntu runner. HTTP verification
passed and the immediate second run reported zero changes.

### [Role-based Ansible configuration](https://github.com/ismet1292-wq/04-ansible-production)

Reusable role, HTML and server templates, input validation, and validated reload
handlers. CI verified rendered content, escaped variable overrides, content-only
updates without reload, and unchanged repeat runs. The repository name describes
a production-style structure, not a production deployment.

### [DevOps CI/CD pipeline](https://github.com/ismet1292-wq/05-devops-cicd-pipeline)

HTTP tests gate an image build and Ansible/Compose deployment on a disposable
runner. CI verifies the running container, unchanged redeployment, rejection of
an intentionally failed release, restoration of the original image and HTTP
health, and cleanup.
It does not publish images or automatically deploy to a persistent server.

## Verified workflow evidence

Checked October 19, 2026. These links identify specific successful runs;
future commits have their own checks.

| Project | Passing run | What was exercised |
|---|---|---|
| 01 Docker Node app | [45aa587](https://github.com/ismet1292-wq/01-docker-node-app/actions/runs/39326150611) | HTTP tests, image build, runtime checks, cleanup |
| 02 Terraform AWS | [a1ef572](https://github.com/ismet1292-wq/02-terraform-aws-infrastructure/actions/runs/39324213787) | Formatting, validation and mocked safeguards; live evidence linked above |
| 03 Ansible configuration | [a30194d](https://github.com/ismet1292-wq/03-ansible-server-configuration/actions/runs/39324656571) | Nginx configuration, HTTP and unchanged second run |
| 04 Ansible role | [78639fb](https://github.com/ismet1292-wq/04-ansible-production/actions/runs/39325107122) | Templates, overrides, handlers and repeat runs |
| 05 CI/CD | [b442d6a](https://github.com/ismet1292-wq/05-devops-cicd-pipeline/actions/runs/39326542284) | Test, build, deployment, failed candidate, verified rollback and cleanup |

These projects were built and extended with AI assistance. The repository code,
workflow logs and deployment evidence establish the tested behavior; they do
not establish paid client work or independent mastery of every component.

## Technologies used in my projects

Python, Node.js, Docker, Compose, Kubernetes, Minikube, GitHub Actions, Git,
Terraform, Ansible, AWS EC2/VPC/SSM, and SQLite.

## Education

- Bachelor of Science in Economic Engineering - University "Isa Boletini" Mitrovica.
- DevOps Engineer Certificate - LSU Online & Continuing Education.

## Next milestones

- Stronger operational logging and monitoring.
- Automated release promotion beyond the disposable rollback demonstration.
- Production authentication, TLS, and security review before public hosting.

These milestones are planned, not completed.

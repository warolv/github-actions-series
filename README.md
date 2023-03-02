# A series of tutorials for GitHub Actions

![gh-tf-example](images/scale-runners/0.png)

### [Use GitHub Actions and Terraform to provision EC2 instance](tf-example.md)

In this tutorial, I will create simple and practical example of how to provision EC2 instance with Github Actions and Terraform. I will use workflow_dispatch type of workflow which is triggered manually by user, using Terraform Github action from HashiCorp.

https://youtu.be/-910lhQXJIs



### [GitOps way with Github Actions and self-hosted runner on Kubernetes](gitops-selfhosted-runner.md)

In this tutorial, I will show how to:

1. Deploy self-hosted-runner to Kubernetes and connect it with your GitHub repo.

2. Redeploy Nginx server on your k8s cluster with every change in nginx/deployment.yaml, which pushed to Github repo.

> "Every change in configuration of deployment.yaml on Github will be propagated to Nginx server."



### [Automatic scaling with Github Actions and self-hosted runners](scale-runners.md)

In this tutorial, I will show how to:

1. Deploy Actions Runner Controller (ARC) to Kubernetes and connect it with your GitHub repo.

2. Scale automatically your self-hosted runners count up to the total number of pending jobs in queue.

> "The main purpose of this guide is to describe the real use case: AWS EKS cluster which is not externally accessible, only using VPN or inside of VPC to which cluster is provisioned."
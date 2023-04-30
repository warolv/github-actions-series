# A series of tutorials for GitHub Actions

![gh-tf-example](images/scale-runners/0.png)

### 1. [Use GitHub Actions and Terraform to provision EC2 instance](tf-example.md)

In this tutorial, I will create simple and practical example of how to provision EC2 instance with Github Actions and Terraform. I will use workflow_dispatch type of workflow which is triggered manually by user, using Terraform Github action from HashiCorp.

https://youtu.be/-910lhQXJIs



### 2. [GitOps way with Github Actions and self-hosted runner on Kubernetes](gitops-selfhosted-runner.md)

In this tutorial, I will show how to:

1. Deploy self-hosted-runner to Kubernetes and connect it with your GitHub repo.

2. Redeploy Nginx server on your k8s cluster with every change in nginx/deployment.yaml, which pushed to Github repo.

> "Every change in configuration of deployment.yaml on Github will be propagated to Nginx server."

https://youtu.be/cV1LhQT1bK4



### 3. [Automatic scaling with Github Actions and self-hosted runners](scale-runners.md)

In this tutorial, I will show how to:

1. Deploy Actions Runner Controller (ARC) to Kubernetes and connect it with your GitHub repo.

2. Scale automatically your self-hosted runners count up to the total number of pending jobs in queue.

> "The main purpose of this guide is to describe the real use case: AWS EKS cluster which is not externally accessible, only using VPN or inside of VPC to which cluster is provisioned."

https://youtu.be/kBeznj8qW1U



### 4. [Github Actions with k8s and Karpenter to dynamically provision your runners on spot instances.](gh-karpenter-spots.md)

In this tutorial, I will show how to:

1. Run self-hosted runners with Github Actions on AWS spot instances.

2. Dynamically add/remove resources to your k8s cluster by Karpenter.

> "This guide is continuation of previous tutorial, please make sure you read it and have cluster with installed ARC."

### 5. [Github Actions with ChatOps to write Beautiful Python Code](gh-chatops.md)

In this tutorial, I will show how to:

1. Trigger Github Actions Workflow using PR comments like ‘/format’ (ChatOps). I will use 'slash-command-dispatch' for this.

2. Format the python code with PEP8 as part of PR and re-commit it again.

### 6. [OpenID Connect and Github Actions to authenticate with Amazon Web Services](gh-oidc.md)

In this tutorial, I will show how to:

1. Use OpenID Connect within your Github workflows to authenticate with Amazon Web Services.

> "The reason behind that is security: Avoid storing long living AWS credentials (access_key_id and secret_access_key) in Github as a secrets."

2. Improve the security of ‘EC2 provisioning’ workflow I described in first guide.

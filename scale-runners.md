# Automatic scaling with Github Actions and self-hosted runners

![scale-runners](images/scale-runners/0.png)

In this tutorial, I will show how to:

1. Deploy Actions Runner Controller (ARC) to Kubernetes and connect it with your GitHub repo.

2. To scale automatically your self-hosted runners count up to the total number of pending jobs in queue.

> "The main purpose of this guide is to describe the real use case: AWS EKS cluster which is not externally accessible, only using VPN or inside of VPC to which cluster is provisioned."

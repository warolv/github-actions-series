### Run self hosted runner with docker
docker run --name github-runner \
     -e GITHUB_OWNER=warolv \
     -e GITHUB_REPOSITORY=github-actions-series \
     -e GITHUB_PAT=YOUR_GITHUB_PAT \
     sanderknape/github-runner

### Download deployment.yaml
```
cd /tmp && mkdir git-runner && cd git-runner
curl -O https://raw.githubusercontent.com/SanderKnape/github-runner/master/deployment.yml
```

### Create secret
```
kubectl create ns github-runner
kubectl create secret generic gh-pat \
    -n github-runner \
    --from-literal=pat=YOUR_GITHUB_PAT
```

### deploy runner
```
kubectl apply -f self-hosted-runner
```

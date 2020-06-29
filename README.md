# Setup in new cluster

Update yaml files in `base` folder to point to use correct url and docker image based on nexus

# Setup in argocd
To deploy in argocd

```bash
kubectl apply -n argocd -f argocd-app/app.yaml
```


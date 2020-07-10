# Setup in new cluster

Update yaml files in `base` folder to point to use correct url and docker image based on nexus


# Deploy App to environments
 Please make sure you have folders that matches the namespaces where the application will be deployed. For i.e: `develop`, `feature`, `test`, `staging` and `prod`. These are folders that has everything related to a specific namespace in the target EKS Cluster.

# Setup in argocd through jenkins
### HELM
`helm install demo-ui2-BRANCH_NAME ./argocd-app --set branch.name=BRANCH_NAME --set destination.namespace=feature -n feature`

# Setup the ingress in a multi-environment
https://github.com/jetstack/kustomize-cert-manager-demo
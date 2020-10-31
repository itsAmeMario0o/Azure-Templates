# Relevant Items

1) Ensure a Service Principal is created - "az ad sp create-for-rbac --name <AppName>" where AppName is replaced with the name of your choosing
2) Copy the appID & password
3) Generate a SSH Key for access to Jenkins & Grafana - "ssh-keygen -t rsa"
4) Before deploying, make sure the region associted with the resource group supports the version of K8S - "az aks get-version -l <TargetRegion>"
5) When naming the variables Azure is sensitive - use lower case and don't rely on special characters for DNS. See here for details : aka.ms/aks-naming-rules

# Helm-CheatSheet

Source: [Helm Quickstart Guide](https://helm.sh/docs/using_helm/)

There are two parts to Helm:
* The Helm Client (helm)
* The Helm Server (Tiller)

### INSTALLING THE HELM CLIENT 

Source: [From the Binary Release](https://helm.sh/docs/using_helm/#installing-the-helm-client)

### INSTALLING TILLER

Source: [Easy In-Cluster Installation](https://helm.sh/docs/using_helm/#easy-in-cluster-installation)

### Using Helm

* `helm init` will initialize helm in your cluster
    * Install a particular image (version) with `--tiller-image`
    * Install to a particular cluster with `--kube-context`
    * Install into a particular namespace with `--tiller-namespace`
    * Install Tiller with a Service Account with `--service-account`
        * Service account is required for `RBAC enabled cluster`

* `helm install <chart name>` will install the desired package 
* `helm install <chart name> --namespace=<namespace name>` will install the package to a specific namespace
* `helm ls` lists all releases 
* `helm status <release's name>` re-read configuration information
* `helm repo list` chart repository list
* `helm repo add <name> <URL>` add new repo 

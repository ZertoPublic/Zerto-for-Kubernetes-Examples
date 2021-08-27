# Zerto for Kubernetes: Examples
*Starter YAMLs to use when deploying and using Zerto for Kubernetes*


Create a VPG: create/edit a YAML—e.g. vpg.yaml using the sample code in this repo—then run `kubectl create vpg -f vpg.yaml`

To use long-term retention (LTR):
1. Create the storage repository as Azure blob or Amazon S3 bucket
2. Create K8s secret for use with that repo: `kubectl create secret -f secret.yaml`
3. Define the LTR settings for the VPG with the secret name listed under CredentialsSecretReference.Id.Name
4. Create or update the VPG

Try these and more for free in the [Zerto for Kubernetes hands-on lab](https://www.zerto.com/labs) in myZerto.

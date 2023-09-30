# Helm Repo Installation Guide

In this guide, you can learn how to install and uninstall Helm charts from a GitHub repository step by step.

## Set Up Your GitHub Credentials

You need to add your GitHub username and personal access token to Helm. You can do this with the following command:

```bash
helm repo add --username <github-user-name> --password <personal-access-token> my-github-repo 'https://raw.githubusercontent.com/<github-user-name>/mygithubrepo/main'
```
## List Added Repositories
After successfully adding your repository, you can list the added repo as follows:
```bash
helm repo list
```
## Search Helm Repositories
You can search for the desired package in Helm repositories with the following command:
```bash
helm search repo my-github-repo
```
## Install the Package
To install the package, use the following command. You can replace my-release with any name you prefer:
```bash
helm install my-release my-github-repo/kubernetes-project
```
## Uninstall the Package
If you want to uninstall the Helm package, use the following command:
```bash
helm uninstall my-release
```
